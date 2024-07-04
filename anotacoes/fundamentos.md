
# Estrutura do Olho Humano

## Visão Geral

O olho humano, praticamente esférico, possui um diâmetro médio de aproximadamente 20mm e é revestido por três membranas: a córnea, cobertura externa da esclera; a coroide, situada abaixo da esclera; e a retina, a membrana mais interna que se estende por toda a porção posterior da parede ocular.

### Córnea e Esclera
- **Córnea:** Tecido resistente e transparente que cobre a superfície anterior do olho.
- **Esclera:** Membrana opaca que reveste o restante do globo ocular, sendo um prolongamento da córnea.

### Coroide
- Situa-se diretamente abaixo da esclera.
- Contém uma rede de vasos sanguíneos, atuando como a principal fonte de nutrição para o olho.
- Revestimento pigmentado reduz a quantidade de luz indesejável que entra no olho.

### Cristalino
- Composto por camadas concêntricas de células fibrosas.
- Suspenso por fibras ligadas ao corpo ciliar.
- Colorido por pigmentação levemente amarelada, intensificando-se com a idade.

### Retina
- Membrana mais interna.
- Responsável por formar imagens quando o olho está adequadamente focalizado.
- A visão de padrões é obtida pela distribuição de receptores discretos de luz ao longo da superfície da retina.

### Receptores na Retina
- **Bastonetes (Rodes):** Detectam brilho.
- **Cones:** Permitem a percepção de cores.
- Maioria dos cones no centro do olho, próximos à fovea.
- Bastonetes ausentes da área próxima à fovea, mas estendem-se por toda a retina, explicando a percepção de níveis de brilho nas bordas da visão.

---

# Formação da Imagem no Olho

Em uma câmera fotográfica, a focalização varia ajustando a distância entre a lente e o plano-imagem (filme). No olho humano, a distância entre a lente (cristalino) e o plano imagem (retina) é fixa, sendo a focalização alcançada pela variação do formato do cristalino, uma lente flexível.

- **Fibras Zonulares:** Achatam ou espessam o cristalino para focalizar objetos distantes ou próximos.

A luz estimula cones e bastonetes na retina, gerando ondas elétricas transmitidas pelo nervo óptico. Este nervo entra no cérebro, dirigindo-se à região responsável pelo processamento da formação das imagens. Cada olho envia uma imagem ao cérebro, que as funde em uma única percepção. A visão binocular oferece um amplo campo visual e a noção de profundidade.


# Fenômenos Perceptuais no Brilho

Dois fenômenos evidenciam que o brilho percebido não é uma simples função da intensidade.

1. **Estimação de Contornos:**
   - O sistema visual tende a subestimar ou superestimar os contornos entre regiões de diferentes intensidades.
   - O brilho é alterado próximo às bordas pela visão.

2. **Contraste Simultâneo:**
   - O brilho percebido de uma região não depende simplesmente de sua intensidade.
   - Na figura abaixo, todos os quadrados centrais têm o mesmo nível de cinza, mas parecem escurecer à medida que o fundo se torna mais claro.
   
   ![Exemplo de Contraste Simultâneo](link_imagem)

   - Um exemplo comum é um pedaço de papel que parece branco sobre uma mesa, mas pode parecer totalmente negro ao proteger os olhos enquanto se olha diretamente para um céu brilhante.

---


# Adaptação ao Brilho

A escala total de níveis distintos de intensidade que podem ser simultaneamente discernidos pelo olho é bastante pequena quando comparada à escala total de adaptação. Para qualquer conjunto de condições, o nível atual de sensibilidade do sistema visual é denominado **nível de adaptação ao brilho**.

A habilidade do olho para discriminar mudanças de intensidade da luz em qualquer nível específico de adaptação também é de considerável interesse. Essa capacidade destaca a notável flexibilidade e ajuste do sistema visual diante das variações nas condições de iluminação. A adaptação ao brilho é crucial para a percepção visual eficaz em ambientes que variam em termos de luminosidade.




# Sensores e Aquisição de Imagens

A maioria das imagens é gerada pela combinação de uma fonte de iluminação e a reflexão ou absorção de energia por elementos de cena, cuja imagem está sendo gerada.

![Arranjos de Sensores](link_imagem)

A figura apresenta os três principais arranjos de sensores usados para converter a energia de iluminação em imagens digitais. A energia incidente é transformada em tensão pela combinação da energia elétrica de entrada e do material do sensor, sensível a um tipo específico de energia. A forma de onda da tensão de saída é a resposta do(s) sensor(es), e uma quantidade digital é obtida de cada sensor por meio da digitalização de sua resposta.



---

# Amostragem e Quantização de Imagens

Para criar uma imagem digital, é necessário converter os dados contínuos captados para o formato digital. Esse processo envolve dois estágios: amostragem e quantização.

## Conceitos Básicos

### Ilustração do Funcionamento:

![Ilustração do Funcionamento](link_imagem)

A Figura 2.16(a) mostra uma imagem contínua \( f \) que será convertida para o formato digital. Uma imagem pode ser contínua em relação às coordenadas \( x \) e \( y \) e também em relação à amplitude. Para convertê-la para o formato digital, é necessário realizar a amostragem da função em ambas as coordenadas e na amplitude. A digitalização dos valores é chamada de amostragem, e a digitalização dos valores de amplitude é chamada de quantização.

A função unidimensional na Figura 2.16(b) é um gráfico que representa os valores de amplitude (nível de intensidade) da imagem contínua ao longo do segmento de reta AB na Figura 2.16(a). As variações aleatórias são devidas ao ruído da imagem.

Para realizar a amostragem dessa função, colhemos amostras igualmente espaçadas ao longo da linha AB, conforme mostra a Figura 2.16(c). A posição de cada amostra no espaço é indicada por uma pequena marca vertical na parte inferior da figura.

Para formar uma função digital, os valores de intensidade também devem ser convertidos (quantizados) em quantidades discretas. As amostras digitais resultantes da amostragem e da quantização são mostradas na Figura 2.16(d). Ao começar na parte superior da imagem e realizar esse procedimento linha por linha, produz-se uma imagem digital bidimensional.


---

# Representação de Imagens Digitais

Em geral, o valor da imagem em quaisquer coordenadas (x, y) é expresso por f(x, y), onde x e y são números inteiros. A seção do plano real que se expande pelas coordenadas de uma imagem é chamada de domínio espacial, com x e y sendo chamadas de variáveis espaciais e coordenadas espaciais.

Sejam M e N o número de linhas e colunas da imagem, e L o número discreto de níveis de intensidade retornado pela função f. Então, \(0 \leq x \leq M - 1\), \(0 \leq y \leq N - 1\) definem a amostragem da imagem digital, e \(0 \leq f(x, y) \leq L - 1\) define a quantização.

O número L representa os níveis discretos de intensidade da imagem:
 L = 2^k
Uma imagem com 256 valores discretos possíveis de intensidade é chamada de uma imagem de 8 bits.

O número \(b\), de bits necessários para armazenar uma imagem digitalizada, é dado por:
 b = M . N . k

Dado o tamanho da imagem (em cm, mm), o número de valores discretos que podem ser tomados depende da resolução, definida normalmente por DPI (dots per inch, pontos por polegada).


---

# Relacionamentos básicos entre pixels

## Vizinhos de um pixel

Seja p um pixel de coordenada (i, j). Os 4 vizinhos ortogonais (horizontais e verticais) de p são:
\[ N4(p) = \{(i + 1, j),(i - 1, j),(i, j + 1),(i, j - 1)\} \]

Os 4 vizinhos diagonais de p são:
\[ ND(p) = \{(i + 1, j + 1),(i - 1, j - 1),(i - 1, j + 1),(i + 1, j - 1)\} \]

Os 8 vizinhos de p são: \[ N8(p) = N4(p) \cup ND(p) \]

## Adjacência e conectividade

Seja V o conjunto de valores de intensidade usados para definir adjacência. Por exemplo, para imagem binária, \( V = \{1\} \), para tons de cinza pode ser um subconjunto de tons de cinza, e para imagens coloridas pode ser uma cor.

Dois pontos p e q têm adjacência-4 ou adjacência-8 se têm a mesma intensidade V e são 4-vizinhos ou 8-vizinhos.

Um caminho de \( p = (i_1, j_1) \) a \( q = (i_n, j_n) \) é uma sequência de pixels distintos \((i_1, j_1),(i_2, j_2), ...,(i_n, j_n)\), tal que todos os pixels \((i_x, j_x)\) e \((i_{x-1}, j_{x-1})\), para \(1 < x \leq n\), são adjacentes (4 ou 8).

Para \( S \), um subconjunto de pixels de uma imagem, \( p \) e \( q \) estão conectados em \( S \) se houver um caminho de pixels de \( p \) a \( q \) só com pixels em \( S \).

O conjunto de pixels conectados a \( p \) em \( S \) é chamado de componente conexo. Se existir apenas um componente conectado, o conjunto \( S \) é chamado de um conjunto conexo.

## Região e borda

O conjunto de pontos conexos de uma imagem é uma Região da imagem. Também chamaremos de forma.

O conjunto de pontos que não fazem parte de região é denominado fundo da imagem.

A fronteira (borda, fronteira ou contorno) de uma região é o conjunto de pontos da região que são vizinhos ao fundo da imagem (borda interna), ou o conjunto de pontos do fundo que são vizinhos à região da imagem (borda externa).

Para evitar o paradoxo da conectividade, se usamos N8 para borda, devemos usar N4 para região e vice-versa.

## Medidas de distância

Sejam \( p = (i_1, j_1) \) e \( q = (i_2, j_2) \). A distância euclidiana entre \( p \) e \( q \) é dada por:
\[ \sqrt{(i_1 - i_2)^2 + (j_1 - j_2)^2} \]

A distância city-block \( dc \) entre \( p \) e \( q \) é dada por:
\[ |i_1 - i_2| + |j_1 - j_2| \]

A distância xadrez \( dx \) entre \( p \) e \( q \) é dada por:
\[ \max(|i_1 - i_2|, |j_1 - j_2|) \]
