# Fundamentos das Transformações de Intensidade e Filtragem Espacial

Os processos no domínio espacial que discutiremos neste capítulo podem ser expressos por:

\[ g(x, y) = T[f(x, y)] \]

onde \( f(x, y) \) é a imagem de entrada, \( g(x, y) \) é a imagem de saída, e \( T \) é um operador em \( f \) definido em uma vizinhança do ponto \( (x, y) \).

## Algumas Funções Básicas de Transformação de Intensidade

Os valores dos pixels antes e depois do processamento serão representados por \( r \) e \( s \), respectivamente. \( s = T(r) \), onde \( T \) é uma transformação que mapeia um valor de pixel \( r \) em um valor de pixel \( s \).

### Negativo de Imagem

O negativo de uma imagem com níveis de intensidade na faixa [0, \( L – 1 \)] é obtido utilizando a transformação de negativo mostrada na figura abaixo e, dada pela expressão:

\[ s = L – 1 – r \]

### Transformações Logarítmicas

A forma geral da transformação logarítmica é:

\[ s = c \log(1 + r) \]

onde \( c \) é uma constante e considera-se que \( r \geq 0 \). O formato da curva logarítmica mostra que essa transformação mapeia uma faixa estreita de baixos valores de intensidade de entrada em uma faixa mais ampla de níveis de saída.

### Processamento de Histograma

O histograma de uma imagem digital com níveis de intensidade no intervalo [0, \( L – 1 \)] é uma função discreta \( h(r_k) = n_k \), onde \( r_k \) é o k-ésimo valor de intensidade e \( n_k \) é o número de pixels da imagem com intensidade \( r_k \).

Um histograma normalizado é dado por \( p(r_k) = r_k / MN \) para \( k = 0, 1, 2, \ldots, L – 1 \). De modo geral, \( p(r_k) \) é uma estimativa da probabilidade de ocorrência do nível de intensidade \( r_k \) em uma imagem. A soma de todos os componentes de um histograma normalizado é igual a 1.
