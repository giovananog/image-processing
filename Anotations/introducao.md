## Definição de Imagem

Uma imagem é conceituada como uma função bidimensional, expressa por `f(x, y)`, onde `x` e `y` representam as coordenadas espaciais no plano. A amplitude da função `f` em qualquer par de coordenadas `(x, y)` é designada como intensidade ou nível de cinza da imagem nesse ponto. Quando `x`, `y` e os valores de intensidade de `f` são quantidades finitas e discretas, a imagem é categorizada como digital. O termo "pixel" é frequentemente utilizado para representar os elementos de uma imagem digital.

## Tipos de Processamento de Imagens

### Nível Baixo
Operações primitivas, como pré-processamento de imagens para redução de ruído, realce de contraste e nitidez. Neste nível, tanto a entrada quanto a saída são imagens.

### Nível Médio
Engloba tarefas como segmentação (divisão da imagem em regiões ou objetos), descrição desses objetos para adaptá-los a uma forma adequada para o processamento computacional e classificação (reconhecimento) de objetos individuais. As entradas geralmente são imagens, mas as saídas são atributos extraídos dessas imagens.

### Nível Alto
Inclui a atribuição de significado a um conjunto de objetos reconhecidos, como na análise de imagens e, no extremo dessa linha, a realização das funções cognitivas normalmente associadas à visão.

---

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

representacao de imagens digitais 

em geral, o valor da imagem em quaisquer coordenadas (x, y) é expresso por f (x, y), odnde  x e y sao numeros inteiros. a secao do plano real que se expande pela scoordenads de uma iamgem é chamada de dominio espaial, com x e y sendo chamadas de variaveis espaciais e coorddenadas espaciais.

