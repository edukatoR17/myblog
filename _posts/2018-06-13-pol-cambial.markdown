---
layout: "post"
title: "Entenendo a política de swaps cambiais"
author: "Joao Pedro"
date: "June 13, 2018"
---

#Entendendo a política de swaps cambiais

Com a variação cambial das últimas semanas, as intervenções do Banco Central do Brasil através dos swaps cambiais voltaram para a pauta das discussões, com o BCB ofertando mais de 30 bilhões de dólares nestes instrumentos. O objetivo deste texto é desvendar o mecanismo de transmissão destes instrumentos para o espectro das taxa de câmbio BRL/USD.

Os swaps cambiais fazem parte das modernas políticas cambiais de mercado. Estas são as intervenções cambiais que o BCB executa tanto no mercado com entrega física de divisas quanto no mercado de derivativos cambiais -- que não utilizam moeda estrangeira, mas estão indexados à sua variação. O adjetivo "modernas" salienta que estas polítcas tem o objetivo de ampliar a capacidade de intervenção do Banco Central nos mercados cambiais, ao fortalecer a sua posição em moeda estrangeira e minimizar o uso efetivo das reservas ao ofertar liquidez nos mercados cambiais. Os swaps cambiais, por serem capazes de afetar as taxas de câmbio BRL/USD sem utilizar dólares, têm sido o principal instrumento de intervenção quando o BCB precisa ofertar liquidez em moeda estrangeira e conter a depreciação do real.

Fortalecer os mercados de *hedge* cambial é a principal justificativa para o uso dos swaps. Além disso, os swaps criam incentivos para que os bancos tomem empréstimos em dólares e ofereçam estes dólares no mercado cambial. Desta forma, os swaps reduzem a necessidade de aumentar as taxas básicas de juros para atrair capitais. Além disso, os swaps podem ser utilizados para coibir movimentos especulativos excessivos no mercado -- em especial quando são ofertados de maneira inesperada, em geral ao longo do dia. 

Os contratos de swap cambial envolvem uma troca de rendimentos, no qual o BCB e a contraparte trocam a variação cambial mais um cupom cambial pela taxa Selic efetiva baseada nas operações compromissadas. Os swaps tradicionais, utilizados quando o BCB quer ofertar liquidez em dólares, são aqueles nos quais o BCB assume a ponta vendida em dólar. 

A formação da taxa de câmbio futura, regulada pela condição de paridade coberta de juros, é essencial para compreender o mecanismo de transmissão dos swaps cambiais:

$$
USD^{FUT} = USD^{SPOT}*\left(\frac{1+i}{1+q}\right)
$$

No qual $i$ é a taxa de juros doméstica e $q$ é o cupom cambial, taxa de juros sintética que remunera as aplicações em dólar *onshore*. Como fica claro na equação acima, o preço de um contrato de dólar futuro, *hoje*, inclui um prêmio, equivalente ao diferencial de juros entre a taxa de juros local e o cupom cambial. 

Ao ofertar contratos de swap cambial tradicional, o BCB se compromete a pagar a variação entre a cotação do dólar no dia anterior à operação até o dia do vencimento, exclusive, acrescido de uma taxa de juros em dólar -- o cupom cambial dos swaps. Essa taxa de juros é definida pelo desconto ofericido sobre a taxa de câmbio inicial contratada. Este cupom cambial implícito é o mecanismo de transmissão dos swaps para o espectro das taxas de câmbio, já que cria oportunidades para operações de arbitragem nos mercados cambiais à vista e de derivativos. Assim, o Banco Central *pode* influenciar as cotações através dos swaps cambiais. Contudo, o efeito dos swaps nas cotações vai depender das forças de mercado que afetam as cotações do dólar e o cupom cambial. 

Caso o cupom cambial imbutido nos swaps seja maior que o cupom cambial observado nos mercados de derivativos, há um incentivo para que os agentes -- principalmente bancos -- tomem contratos de swap cambial e ofertem, simultaneamente, dólares no mercado futuro, puxando a cotação do dólar futuro para baixo. 

Para explorar as oportunidades de arbitragem entre os swaps e os mercados de derivativos, os bancos devem efetuar duas transações simultâneas:

* Assumir a ponta "comprada em dólar" em um contrato de swap cambial;
* Vender dólar futuro ou outro derivativo no qual o banco assuma a ponta vendida em dólar.

Essas duas operações vão gerar os seguintes resultados:

|Bancos| |
| ---|---|
|Swap cambial| Mercado de derivativos|
|$+\Delta E$|$-\Delta E$|
|$- i$|$+i$|
|$+ Q$|$- q$|

Onde $\Delta E$ é a variação cambial, $i$ é a taxa de juros doméstica de referência (Selic efetiva), $Q$ é o cupom cambial implítico na operação de swap cambial e $q$ é o cupom cambial implícito no contrato de dólar futuro. A janela de arbitragem existirá enquanto $Q > q$ ou enquanto durar o impacto quantitativo dos swaps sobre a oferta de dólar futuro. Por serem negociados na BM&FBovespa, os swaps podem ser utilizados diretamente como garantia na venda de contratos de dólar futuro, facilitando a distribuição da proteção oferecida pelo BCB.

O cupom cambial oferecido pelo BCB nos swaps também gera oportunidades de arbitragem no mercado à vista. Para aproveitar esta janela de arbitragem, os bancos devem efetuar quatro operações simultâneas:

* Assumir a ponta comprada em dólar em um contrato de swap cambial;
* Obter empréstimos em dólar no exterior;
* Vender os dólares no mercado doméstico;
* Investir estes recursos no mercado doméstico.

Essas operações vão gerar os seguintes resultados:

|Bancos| |
|---|---|
|Swap cambial| Mercado à vista|
|**Realizado:**| |
|$+\Delta E$||
|$- i$|$+i$ (investimento DI)|
|$+ Q$|$-$ custo de captação (dívida externa)|
|**Não realizado:**| |
| | $-\Delta E$ (dívida externa)|

Enquanto $Q >$ *custo de captação*, que gira em torno da taxa *libor* acrescida de um prêmio de risco, haverá espaço para estas operações de arbitragem. Deve-se destacar que, no caso de depreciação do real, haverá um resultado positivo realizado pelos bancos derivado das operações de swap, em paralelo a um aumento do valor em reais de seu passivo.

Assim, os swaps têm um efeito de estimular a oferta de dólares tanto no mercado à vista como no mercado de derivativos. Além disso, os bancos podem entrar em contratos de swap por motivos especulativos, visando montar posições compradas em dólar. Analiticamente:

|Canais de distribuição dos swaps| |
|---|---|
|Mercado de derivativos|$\alpha$ * Swaps, $0 \leq \alpha \leq 1-\gamma$|
|Mercado à vista|$\gamma$ * Swaps, $0 \leq \gamma \leq 1-\alpha$|
|Especulação|$(1-\alpha - \gamma)$ * Swaps|

Como os bancos irão alocar os recursos irá depender de suas preferências e da demanda por dólar no mercado à vista ou por derivativos cambiais.

A capacidade dos swaps de afetar os mercados vai depender das condições existentes nos mercados. Quanto menor for a demanda por instrumentos cambiais, mais efetivo serão os swaps em afetar as cotações. No entanto, caso a demanda por liquidez em moeda estrangeira seja muito forte, a distribuição dos swaps nos diferentes mercados ficará limitada quantitativamente pela escala da intervenção. Além disso, os bancos podem formar posições especulativas com os swaps, apostando na alta do dólar.

É importante ressaltar que em um contexto de elevada abertura financeira, as condições internacionais -- taxas de juros nos países centrais, apetite ao risco dos investidores internacionais e preço das commodities -- são determinantes para a formação das tendências cambiais no Brasil, uma vez que investidores internacionais têm uma importância muito grande. Fatores nacionais, como notícias políticas, estão mais relacionados com a volatilidade dos mercados cambiais brasileiros. O preço do *dólar* não é determinado localmente, mas a volatilidade de sua paridade com o real é exacerbada pela grande concentração dos mercados brasileiros e pela existência de um mercado de derivativos muito líquido.

Neste contexto, a utilização dos swaps cambiais para defender um patamar cambial não condizente com as condições de mercado enfrenta um importante paradoxo: o aumento da demanda por liquidez em moeda estrangeira exige o aumento da escala das intervenções para que estas sejam efetivas. Contudo, o aumento da escala das intervenções reduz a credibilidade da política cambial, se materializando em uma exigência por prêmios (Q) cada vez maiores por parte dos agentes. A forma mais eficiente de quebrar esta armadilha é impor um maior controle sobre os mercados cambiais, amarrando o mercado e reduzindo sua capacidade de apostar contra o governo, aumentando a eficiência dos swaps, como sugerido por [Pedro Rossi](https://www.cartacapital.com.br/economia/o-pais-e-refem-do-cenario-externo-e-dos-especuladores-internacionais).

Por serem liquidados em reais, os swaps aumentam o poder de fogo do BCB. No entanto, a expansão dos contratos abertos no mercado pode resultar em severas perdas no caso de depreciação do real. Em 2015, por exemplo, quando o Banco Central desistiu de intervir explicitamente no mercado cambial e deixou o mercado ajustar as taxas, a perda financeira com os swaps atingiu valores equivalentes a 1,8% do PIB brasileiro.

Finalmente, é importante entender o que se passa nas contas do BCB, ao ofertar estes contratos. Para isso, é preciso dar um passo atrás e relembrar que o efeito monetário do acúmulo de reservas internacionais foi compensado pela emissão de operações compromissadas. Ao ofertar swaps cambiais tradicionais, o BCB assume a ponta vendida em dólar. Na prática, ele oferece ao mercado a valorização patrimonial de parte de suas reservas. Em troca, o BCB recebe o renndimento da taxa de juros associada às operações compromissadas, cobrindo o custo de carregamento das reservas cambiais que estão servindo de *hedge* para os swaps. Desta forma, a política de swaps implica nos seguintes resultados para o BCB:

|Banco Central| |
|---|---|
|Swap cambial| Reservas internacionais|
|**Realizado:**| |
|$-\Delta E$| |
|$+ i$|$- i$ (Custo de carregamento / Operações compromissadas)|
|$- Q$|$+i*$|
|**Não realizado:**| |
| |$+\Delta E$|

Observando apenas os swaps cambiais, o resultado do BCB será igual a diferença entre a variação cambial e a taxa Selic efetiva no período. Contudo, quando tomamos as operações cambiais no seu conjunto, fica claro que o prejuízo do BCB no caso de depreciação cambial é coberto por ganhos de capital nas reservas internacionais. Além disso, o BCB cobre, com os swaps, o custo de carregamento das reservas internacionais que estão "cobrindo" os swaps. Este tipo de avaliação mais abrangente orienta as regras da operação de equalização cambial entre o BCB e o Tesouro, na qual as operações cambiais envolvem tanto as operações com reservas como com derivativos, e os resultados das duas contas são liquidados antes da transferência para o Tesouro ser efetuada.

No entanto, deve-se destacar a dinâmica entre os resultados realizados e não realizados. Com os swaps, o BCB monetiza parte dos seus ganhos patrimoniais nas reservas para entregar como rendimento ao setor privado no caso de depreciação cambial. Estes valores são distribuídos pelos diferentes mercados, reduzindo o impacto da depreciação cambial sobre a situação patrimonial do setor privado. Contudo, por serem liquidados no mercado, as perdas nos contratos de swaps expandem as reservas bancárias e precisam ser compensados pela emissão de operações compromissadas. Estas irão render juros, que serão realizados e compensados, reforçando o círculo vicioso entre juros e operações compromissadas.
