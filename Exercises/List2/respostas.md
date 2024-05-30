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



9- 