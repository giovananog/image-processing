# Representação

Uma vez que a imagem tenha sido segmentada, os pixels são representados e descritos em um formato apropriado para o processamento subsequente. A representação envolve duas coisas:
1. Através de suas características externas (fronteira): Quando existe interesse na forma (geometria) do objeto.
2. Através de suas características internas (os pixels que compõem a região): Quando existe interesse na análise da cor ou textura.

A próxima tarefa é descrever a região baseada na representação escolhida. As características selecionadas como descritores devem ser as menos afetadas por variações como mudança de tamanho, rotação, translação, etc. Deve-se buscar assinaturas da imagem.

## Esquema de Representação

Um dos esquemas de representação que pode ser utilizado é o Código da Cadeia (Chain Code):
- É usado na representação de fronteira.
- Essa representação baseia-se na conectividade de 4 ou 8 segmentos.
- A cadeia resultante é longa.
- Qualquer ruído na fronteira pode causar erros.
- Depende do ponto inicial.

## Rastreamento de Contorno

Considere b0, o ponto superior esquerdo da imagem, com o valor 1. 
1. Obtenha c0, o vizinho à esquerda de b0. Examine os 8-vizinhos de b0 a partir de c0. Seja b1 o primeiro vizinho igual a 1 e c1 o ponto de fundo anterior a b1.
2. Considere b = b1 e c = c1.
3. Sejam n1, n2, ..., n8 os 8-vizinhos de b a partir de c. Encontre o primeiro nk igual a 1.
4. Considere b = nk e c = nk−1.
5. Repita os passos 3 e 4 até b = b0 e o próximo ponto do contorno for b1.
