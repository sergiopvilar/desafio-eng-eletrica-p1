# Introdução

O desperdício de energia é algo que deve ser constantemente considerado durante a fase de projeto de um circuito elétrico não importa o seu tamanho. O teorema da máxima transferência de potência é um ponto chave nesse quesito pois ele nos ajuda a alcançar o máximo de aproveitamento de um circuito, evitando o desperdício de energia ao seu máximo.

Neste experimento podemos observar a relação entre a máxima transferência de potência, eficiência, potência dissipada e a resistência equivalente em um circuito.

## Desenvolvimento

# Objetivos

## Objetivo geral

Este trabalho tem como objetivos principais o uso do laboratório virtual com a temática da Engenharia Elétrica, proporcionando a análise experimental com diversas variáveis, permitindo assim a aplicação de conhecimentos básicos da Engenharia Elétrica através do uso de recursos computacionais na análise do problema e suas possíveis soluções.


## Objetivos específicos

- Aplicação de conhecimentos básicos das unidades curriculares do curso de Engenharia Elétrica
- Uso de laboratório virtual disponibilizado pela instituição a fim de familiarização com o ambiente de laboratório
- Análise da relação entre Eficiência, Transferência de Potência, Potência Dissipada e Resistência Equivalente em um circuito

# Procedimento Experimental

Através do uso do laboratório virtual, disponibilizado pela instituição para a construção deste relatório, foi possível a viabilização de diversos experimentos em relação ao uso do Potenciômetro em um circuito.

Com base no roteiro do experimento, fez-se diversas alterações de resistência no Potenciômetro chegando aos seguintes dados:

\begin{table}[!htp]\centering
\caption{Medições no Laboratório Virtual}\label{tab: }
\scriptsize
\begin{tabular}{ccccc}\toprule
\textbf{Medição} &\textbf{Res. Potenciômetro ($\Omega$)} &\textbf{Tensão Resistor R2 (V)} &\textbf{Tensão Potenciômetro (V)} \\\midrule
1 &8 &1.32 &1.06 \\
2 &16 &1.09 &1.73 \\
3 &24 &0.93 &2.22 \\
4 &32 &0.81 &2.58 \\
5 &40 &0.76 &2.86 \\
6 &48 &0.63 &3.08 \\
7 &56 &0.58 &3.25 \\
8 &64 &0.53 &3.41 \\
9 &72 &0.49 &3.52 \\
10 &80 &0.45 &3.63 \\
11 &88 &0.42 &3.73 \\
12 &96 &0.41 &3.81 \\
\bottomrule
\end{tabular}
\end{table}

# Resultados

A partir dos dados obtidos nas medições conforme demonstrado acima, pode-se chegar aos valores de Corrente do Circuito, Resistência Equivalente do Circuito e Potência Dissipada no Circuito.

### Corrente Elétrica do Circuito

Com base na equação da tensão da fonte, podemos chegar aos valores de Corrente Elétrica do Circuito usando a seguinte equação:

\begin{equation}
\mathbf{i} = \frac{Vf}{Rp}
\end{equation}

Onde:

- _i_ é a Corrente Elétrica do Circuito
- _Vf_ é a Tensão da Fonte
- _Rp_ é a Resistência do Potenciômetro

### Resistência Equivalente

Para calcular a Resistência Equivalente do Circuito, também conhecida como Resistência de Thévenin \cite{48845}, somamos a Resistência do Potenciômetro com a Resistência do segundo Resistor, equivalente a 10\Omega.

Utilizando a forma a seguir podemos chegar ao resultado para cada variação de Resistência do Potenciômetro:

\begin{equation}
\mathbf{Req} = Rp\times10\Omega
\end{equation}

Onde:

- _Req_ é a Resistência Equivalente do Circuito
- _Rp_ é a Resistência do Potenciômetro

### Potência Dissipada

Para chegarmos à Potência Dissipada temos o quociente da tensão ao quadrado pela resistência:

\begin{equation}
\mathhbf{P} = \frac{Vˆ2}{R}
\end{equation}

Onde:

- _P_ é a Potência Dissipada
- _V_ é a Tensão
- _R_ é a Resistência

Portanto, para chegarmos à Potência Dissipada do Circuito, temos o somatório das potências dissipadas de todo o circuito:

\begin{equation}
\mathbf{Pot_{Dissipada}} = \sum \frac{Vi^{2}}{Ri} = \frac{V1^{2}}{R1} + \frac{V2^{2}}{R2} + \frac{Vp^{2}}{Rp}
\end{equation}

### Eficiência

Para chegarmos à Eficiência na Transferência de Potência, precisamos calcular o quociente da Resistência Equivalente pela Resistência Equivalente somada à Resistência Interna da Fonte.

\begin{equation}
\mathhbf{\eta } = \frac{Req}{Req + R}
\end{equation}

Onde:

- _Req_ é a Resistência Equivalente
- _R_ é a Resistência Interna da Fonte

## Tabela de Resultados

\begin{table}[!htp]\centering
\caption{Resultados obitdos a partir dos cálculos descritos previamente}\label{tab: }
\scriptsize
\begin{tabular}{ccccccccc}\toprule
\textbf{Medição} &\textbf{Res. Potenciômetro ($\Omega$)} &\textbf{Corrente (A)} &\textbf{Res. R2 ($\Omega$)} &\textbf{Req} &\textbf{Eficiência ($\eta$)} &\textbf{Pot. Disspada} \\\midrule
1 &8 &1.1250 &10 &18 &0.4737 &4.3647 \\
2 &16 &0.5625 &10 &26 &0.5652 &4.3559 \\
3 &24 &0.3750 &10 &34 &0.6296 &4.3418 \\
4 &32 &0.2813 &10 &42 &0.6774 &4.3236 \\
5 &40 &0.2250 &10 &50 &0.7143 &4.3122 \\
6 &48 &0.1875 &10 &58 &0.7436 &4.2873 \\
7 &56 &0.1607 &10 &66 &0.7674 &4.2723 \\
8 &64 &0.1406 &10 &74 &0.7872 &4.2598 \\
9 &72 &0.1250 &10 &82 &0.8039 &4.2461 \\
10 &80 &0.1125 &10 &90 &0.8182 &4.2350 \\
11 &88 &0.1023 &10 &98 &0.8305 &4.2257 \\
12 &96 &0.0938 &10 &106 &0.8413 &4.2180 \\
\bottomrule
\end{tabular}
\end{table}

## Gráfico da Potência Dissipada em função da Eficiência

A partir dos dados obtidos nas medições foi possível através dos devidos cálculos chegarmos aos valores de Eficiência e Potência dissipada no circuito para cada variante de resistência do Potenciômetro e assim montar o seguinte gráfico:

\begin{figure}[htbp]
\caption{\label{fig:grafic}Gráfico da Potência Dissipada em função da Eficiência}
\begin{center}
\includegraphics[width=1.0\textwidth]{/trabalho/imagens/grafico.png}
\end{center}
\end{figure}

Ao exportar os dados das medições e seus respectivos resultados noformato CSV foi possível produzir o gráfico acima através da ferramenta RStudio na versão 1.3.959 em conjunto com a biblioteca ggplot2 na versão 3.3.1. \cite{geom_bar}

## Perguntas e Respostas

### Para que valor de eficiência foi observada a menor potência dissipada? Pode-se afirmar que esse ponto é o de maior transferência de potência?

**R:** Para eficiência de 0,8413𝛈, obtemos a potência de 4,2180W. Não podemos afirmar que esse é o ponto de maior transferência de potência pois elas são inversamente proporcionais, ou seja, quanto maior for a eficiência, menor será o trabalho realizado.

### Analisando a resistência interna e externa. Quando a transferência de potência apresentará seu valor máximo? Justifique.

**R:** Quando o valor da resistência equivalente for o mais próximo possível do valor da resistência interna, pois quando a resistência equivalente for menor que 17\Omega, a eficiência e a potência dissipada serão diretamente proporcionais, mas quando a Resistência equivalente for maior que 17\Omega, a eficiência e a potência dissipada serão inversamente proporcionais. Ou seja, a resistência equivalente do circuito é igual a resistência interna da fonte de alimentação.

### Como o resistor R1 atua no circuito? Se não fosse colocado este resistor no circuito o valor encontrado para máxima transferência de potência seria o mesmo? Justifique.

**R:** O resistor R1 atua no circuito como resistência interna da fonte, limitando a carga distribuída para o circuito. O valor da máxima transferência de potência não seria o mesmo, pois não haveria limite de carga para a fonte causando sobreaquecimento.

# Conclusão

<!--Fonte: \citeonline{limarka}-->
