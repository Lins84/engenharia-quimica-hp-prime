# HP Prime Thermodynamics Suite 🧪🔥

Uma coleção completa de aplicativos em PPL (HP Prime Programming Language) para Engenharia Química e Termodinâmica.

## 📦 Conteúdo do Pacote

Este repositório contém 4 aplicativos independentes:

1.  **TERMO_TITANIUM**: Cálculos P-V-T para substâncias puras.
    * **Modelos:** Gás Ideal, Van der Waals, RK, SRK, Peng-Robinson, Virial (Pitzer-Curl).
    * **Extras:** Calcula Propriedades Derivadas (Fator Z, Compressibilidade, Expansividade).
    * **Solver:** Calcula Temperatura (T) via Newton-Raphson para todas as equações cúbicas.

2.  **TERMO_LIQ_PRO**: Focado em Líquidos Saturados/Comprimidos.
    * **Modelos:** Rackett (Estimado via Yamada-Gunn), Rackett (com Vc real) e COSTALD (Hankinson-Thomson).
    * **Função:** Calcula Volume dado T, ou Temperatura dado V (Solver Reverso).

3.  **TERMO_MIX**: Misturas Binárias.
    * **Modelos:** SRK e Peng-Robinson.
    * **Método:** Regras de Mistura de van der Waals (1-fluid) com parâmetro de interação binária ($k_{ij}$).
    * **Saída:** Volume molar e Fator Z da mistura.

4.  **TERMO_GEN_PLUS**: Assistente para Gráficos Generalizados.
    * **Método:** Lee-Kesler.
    * **Função:** Calcula propriedades Pseudocríticas (Regra de Kay) para misturas e entrega $Tr$ e $Pr$ prontos para leitura em gráficos.

## 🚀 Como Instalar

1.  Baixe o "HP Connectivity Kit" no seu computador.
2.  Abra o arquivo `.ppl` deste repositório que deseja instalar.
3.  Copie todo o código texto.
4.  No Connectivity Kit, clique com o botão direito em "Programas" > "Novo Programa".
5.  Dê o nome exato do App (ex: `TERMO_TITANIUM`).
6.  Cole o código no editor e salve (ícone de disquete ou envie para a calculadora).

## 📖 Como Usar

Ao abrir qualquer um dos apps, você verá um menu principal.
* **Variáveis:** Os apps usam variáveis globais (`EXPORT`) para que os dados persistam entre cálculos (ex: se você digitou a Tc da água uma vez, ela fica salva para o próximo cálculo).
* **Solvers:** Para cálculos complexos (como Volume em PR ou Temperatura em SRK), o app usa o método de Newton-Raphson. Se o cálculo demorar 1 segundo, é normal.

## ⚠️ Aviso
Estes programas foram desenvolvidos para fins educacionais e de engenharia prática. Sempre verifique os resultados críticos.

---
*Desenvolvido em colaboração com Especialista HP Prime.*
