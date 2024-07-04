---

exercicio 1

O processo que explica o tempo que é levado antes de conseguir enxergar bem o suficiente para encontrar um lugar vago no cinema escuro é o chamado de Adaptação ao Brilho



---

exercicio 2

L - niveis de intensidade (8192)
k - profundidade em bits (?)

formula: L = 2^k

portanto, 8192 = 2^k
          log2 (8192) = log2 (2^k)
          log2 (8192) = klog2 (2)
          log2 (8192) = k
          k = 13 bits



---

exercicio 3

L = 2^k   =>    256 = 2^k   =>   k = 8 bits
          
tamanho total de bits de armazenamento da imagem:

 b = N.M.k  =>  b = 1024.1024.8  =>  b = 8.388.608 bits

 

 ---

 exercicio 4

 componentes com vizinhança-4: 4
 componentes com vizinhança-8: 1


 ---

 exercicio 5

"Uma imagem pode ser contínua em relação às coordenadas ( x ) e ( y ) e também em relação à amplitude. Para convertê-la para o formato digital, é necessário realizar a amostragem da função em ambas as coordenadas e na amplitude. A digitalização dos valores é chamada de amostragem, e a digitalização dos valores de amplitude é chamada de quantização."

a frase está descrevendo o processo de converter uma imagem analógica em uma forma digital, onde você seleciona pontos específicos na imagem (amostragem) e atribui valores discretos a esses pontos para representar sua intensidade (quantização), enquanto a imagem original tem uma ampla gama de tons possíveis (amplitude).



---

exercicio 6

p = (1, 1)
q = (6, 6)


. distancia euclidiana:
        \sqrt((1-6)^2 + (1-6)^2) = 5\sqrt(2)

. distancia city-block:
        |1-6| + |1-6|  = 10

. distancia xadrez: 
        max(|1-6|, |1-6|) = 5




---

exercicio 7

borda interior: 
        0 0 0 0 0 0 0 0
        0 1 1 1 1 1 0 0
        0 1 1 1 1 1 0 0
        0 0 1 1 1 0 0 0
        0 0 1 1 1 1 0 0
        0 0 1 1 1 1 0 0
        0 1 1 0 0 1 0 0
        0 0 0 0 0 0 0 0

---


exercicio 9


7 3 6 7 7 6 6 7
7 3 7 3 0 3 7 6
6 6 5 6 3 3 7 6
7 0 5 6 7 0 0 7
3 0 6 3 6 3 5 3
7 6 3 3 5 3 6 6
5 7 6 6 3 5 7 5
6 7 6 6 0 6 5 6



---

exercicio 10


T[8] = [0, 3, 5, 6, 6, 6, 7, 7]
        0  1  2  3  4  5  6  7



---

exercicio 11


matriz:
            9 5 7 5 3 4
            0 2 6 4 2 5
            4 1 2 4 6 2
            2 3 6 3 0 0
            7 8 3 4 5 4
            0 5 2 9 8 7

MN = 36
k = 10

            r_k      n_k  
            r0 = 0    4
            r1 = 1    1
            r2 = 2    6 
            r3 = 3    4 
            r4 = 4    6 
            r5 = 5    5 
            r6 = 6    3
            r7 = 7    3 
            r8 = 8    2
            r9 = 9    2 
            


---

exercicio 12

M.N = 1330
k = 8

r_k       n_k   nK/MN   s_k    s_k arred.
r0 = 0    120    0.09   0.63      1
r1 = 1    200    0.15   1.68      2
r2 = 2    350    0.26    3.5      4
r3 = 3    400    0.30    5.6      6
r4 = 4    100    0.08   6.16      6
r5 = 5     80    0.06   6.58      7
r6 = 6     50    0.04   6.86      7
r7 = 7     30    0.02    7.0      7


nova distribuicao:

    N´ıvel de cinza(k)  0   1   2   3   4   5   6   7
    Nro. pixels(nk)     0  120 200  0 350  0  500 160




