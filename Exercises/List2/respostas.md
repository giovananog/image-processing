1 - 

F(0) = 9
F(1) = -1 + 2j
F(2) = 1
F(3) = -1 - 2j



2 - A compressão JPEG é obtida convertendo a imagem em blocos de 8x8 pixels, aplicando a Transformada Discreta de Cosseno (DCT), quantizando os coeficientes resultantes, e, em seguida, usando codificação RLE e codificação de Huffman para compactar os dados.

3 - Mesmo que alguns métodos de compressão insiram erros na imagem digital, eles são amplamente usados porque reduzem significativamente o tamanho do arquivo, facilitando o armazenamento e a transmissão. Esses métodos, como o JPEG, são projetados para descartar informações menos perceptíveis ao olho humano, mantendo uma qualidade visual aceitável. Além disso, a redução no tamanho do arquivo resulta em uma transferência mais rápida e eficiente, essencial para aplicações na web, dispositivos móveis e armazenamento em nuvem, justificando seu uso generalizado.

4- BABABABABABABABACABACABABABABABADABAABAABA

5-

a) 
    0 0 1 0 0 0 0 0 0 0 
    0 1 1 1 0 0 0 0 0 0 
    1 1 1 1 1 0 0 0 1 0 
    0 1 1 1 1 1 1 1 1 1
    0 1 1 1 1 1 1 1 1 1
    0 1 1 1 1 1 1 1 1 1
    1 1 1 1 1 1 1 1 1 1
    0 1 1 1 1 1 1 1 1 0
    0 0 1 1 1 1 1 1 0 0
    0 0 0 0 0 0 0 0 0 0

b) 
    0 0 0 0 0 0 0 0 0 0 
    0 0 0 0 0 0 0 0 0 0 
    0 0 1 0 0 0 0 0 0 0 
    0 0 0 0 0 0 0 0 0 0
    0 0 0 0 0 0 0 0 0 0
    0 0 0 1 1 0 0 1 0 0
    0 0 1 1 1 1 1 1 0 0
    0 0 0 0 0 0 0 0 0 0
    0 0 0 0 0 0 0 0 0 0
    0 0 0 0 0 0 0 0 0 0

c)
    0 0 0 0 0 0 0 0 0 0 
    0 0 1 0 0 0 0 0 0 0 
    0 1 1 1 0 0 0 0 0 0 
    0 0 1 0 0 0 0 0 0 0
    0 0 0 1 1 0 0 1 0 0
    0 0 1 1 1 1 1 1 1 0
    0 1 1 1 1 1 1 1 1 0
    0 0 1 1 1 1 1 1 0 0
    0 0 0 0 0 0 0 0 0 0
    0 0 0 0 0 0 0 0 0 0

d)
    0 0 0 0 0 0 0 0 0 0 
    0 0 1 0 0 0 0 0 0 0 
    0 0 1 0 0 0 0 0 0 0 
    0 0 1 1 1 0 0 0 1 0
    0 0 1 1 1 1 1 1 1 0
    0 0 1 1 1 1 1 1 1 0
    0 1 1 1 1 1 1 1 1 0
    0 0 1 1 1 1 1 1 0 0
    0 0 0 0 0 0 0 0 0 0
    0 0 0 0 0 0 0 0 0 0


6- As operações de morfologia matemática são eficazes para identificar o contorno de uma imagem binária. A dilatação expande as regiões brancas da imagem, enquanto a erosão as reduz. Ao aplicar a dilatação seguida de uma operação de diferença entre a imagem original e a imagem dilatada, ou ao aplicar a erosão seguida da mesma operação, obtemos o contorno da imagem. Isso ocorre porque essas operações modificam a forma da imagem de maneira que apenas as bordas permaneçam visíveis após a subtração da imagem dilatada ou erodida da original. Essa abordagem é eficaz para destacar e identificar as características de contorno de uma imagem binária.


7- 


8- Essa operacao pode ser feita aplicando os seguintes algoritmos na iamgme:

Dilatação: Aplicar a operação de dilatação à imagem original A usando um elemento estruturante que defina a vizinhança desejada.

Erosão: Em seguida, aplicar a operação de erosão à imagem original A usando o mesmo elemento estruturante.

Gradiente: Calcular o gradiente morfológico, que é a diferença entre a imagem dilatada e a imagem erodida.



9- A operação Watershed é uma técnica de segmentação em Morfologia Matemática que simula o preenchimento de uma superfície topográfica, onde a altitude é representada pelos níveis de cinza de uma imagem numérica. Essa operação é utilizada para segmentar regiões em uma imagem com base em mínimos locais, chamados de marcadores, e na construção de diques virtuais para evitar a junção de fluxos de "água" durante o preenchimento da superfície. 

Para implementar a operação Watershed, pode-se utilizar um algoritmo que simule o crescimento das regiões a partir dos marcadores. Esse algoritmo geralmente utiliza uma fila de prioridade ordenada de acordo com os níveis de cinza da imagem. Cada ponto é extraído da fila e agregado à região correspondente, garantindo que pontos vizinhos de duas regiões com rótulos diferentes sejam identificados como pontos de borda. Essa abordagem permite a segmentação eficiente de regiões em uma imagem com base em características locais de intensidade.


10-

11- 

12- A segmentação de contornos e a codificação de cadeia podem ser utilizadas para definir um formato de imagem simplificado ao identificar e extrair as bordas dos objetos presentes na imagem. A segmentação de contornos isola os objetos do fundo, identificando onde ocorrem mudanças abruptas de intensidade, enquanto a codificação de cadeia registra a direção dos movimentos entre pixels consecutivos ao longo do contorno. Esse método permite representar a imagem de forma compacta, armazenando apenas as direções dos contornos em vez de todos os pixels, resultando em uma representação eficiente e reduzida que captura a forma dos objetos sem os detalhes internos.
