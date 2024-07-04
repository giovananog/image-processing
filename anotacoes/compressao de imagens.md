# Compressão de Imagens

## Fundamentos

A imagem digital gera uma enorme quantidade de dados. A compressão de imagem trata o problema de reduzir a quantidade de dados necessários para representar uma imagem digital. Teve início antes do computador digital, com a transmissão de vídeo, e vem crescendo desde o surgimento do computador.

Redundância de dados é o tema central da compressão de imagens. Sejam \( n_1 \) e \( n_2 \) o espaço necessário para armazenamento do mesmo dado usando codificações diferentes. Seja CR, a taxa de compressão dada por:
\[ CR = \frac{N1}{N2} \]
A redundância (RD) é dada por:
\[ RD = 1 - \frac{1}{CR} \]

Para compressão, três redundâncias básicas podem ser exploradas:
- Redundância de codificação
- Redundância de interpixel
- Redundância psicovisual

## Critério de Fidelidade

Pode existir perda na compressão da imagem. Apesar das medidas matemáticas, a melhor avaliação será sempre a percepção humana.

## Modelos de Compressão

O processo usado para reduzir o tamanho físico da imagem, para otimizar transmissão e armazenamento, está associado a duas fases: a codificação e a decodificação. A ideia básica é representar os elementos da imagem com maior frequência usando uma quantidade menor de bits.

### Características da Compressão

Na decodificação, a imagem obtida pode ser exatamente igual ou apresentar alguma alteração (perda). A codificação e decodificação podem ser realizadas com perda ou sem perda. A perda de informação pode comprometer a qualidade da imagem, dificultando a interpretação do seu conteúdo. Há aplicações em que uma compressão com perda é intolerável, como na compressão de dados de um cliente de banco.

### Compressão sem Perdas (Lossless)

- Reversível
- Imagem reconstruída é igual à imagem original
- Apresenta baixas taxas de compressão (< 3:1)
- Aplicações: imagens médicas e de satélite

### Compressão com Perdas (Lossy)

- Irreversível
- Imagem reconstruída = imagem original + ruído
- Taxas de compressão elevadas
- Diversas aplicações: web, etc.

### Características

- **Adaptabilidade:** Refere-se à característica do processo/algoritmo de se adaptar aos dados de entrada.
  - **Não Adaptativos:** Baseiam-se em dicionários estáticos definidos a priori em função de estatísticas de frequência de dados. Usam um dicionário de codificação/compressão que associa os símbolos originais a códigos de menor tamanho.
  - **Adaptativos:** Não se baseiam em dicionários pré-definidos, construindo o dicionário em função dos dados de entrada.
  - **Semi-Adaptativos:** Em geral, é efetuado em dois passos: no primeiro, é efetuada uma estatística de entrada, gerando um dicionário; na segunda fase, é efetuada a codificação/compressão propriamente dita.

## Métodos de Compressão

### Árvore de Huffman

O algoritmo de Huffman é um método para compactar um texto/imagem de forma ótima, sobre certos critérios. O texto/imagem em questão é composto de símbolos/pixels \( S = \{s1, s2, ..., sn\} \), \( n > 1 \), dos quais se conhece a frequência \( f_i \) de ocorrência de cada símbolo/pixel no texto/imagem, ou seja, \( s_i \) acontece \( f_i \) vezes dentro do texto/imagem para \( 1 \le i \le n \).

### Codificação LZW

A técnica, chamada codificação de Lempel-Ziv-Welch (LZW), atribui palavras código de tamanho fixo a sequências de símbolos fonte de tamanho variável. Uma importante característica da codificação LZW é que ela não requer conhecimento antecipado da probabilidade de ocorrência dos símbolos que serão codificados. LZW não requer nenhuma informação a priori dos dados de entrada, comprime e descomprime numa única passada, permitindo implementação simples e rápida execução.

### Codificação JPEG

#### Características

- Padrão de Compressão de Imagens Estáticas
- Compressão Com Perdas (baseline)
- Taxa de Compressão Indeterminada A Priori
- Baseada em:
  - Transformada DCT
  - Quantização
  - Codificação R.L.E.
  - Codificação Entrópica (Huffman)

#### Transformada DCT

Objetivos do DCT:
- Descorrelacionar os elementos da imagem
- Representar a imagem em termos de componentes de frequência espacial para posterior processamento, de acordo com as características da visão humana
- Simplificar o processamento (valores reais)

#### Codificação R.L.E

Características:
- Gera códigos de comprimento variável
- Útil para aumentar a compressão
- O código binário tem a forma PREFIXO:MANTISSA, onde o PREFIXO e MANTISSA têm tamanhos variáveis e são obtidos consultando tabelas de codificação de Huffman predefinidas.
