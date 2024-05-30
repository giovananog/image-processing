### Segmentação de Imagens

#### Definição
Segmentar uma imagem é dividí-la em suas regiões constituintes, visando extrair informações relevantes. As principais descontinuidades extraídas incluem pontos isolados, linhas e bordas.

#### Operações

- **Pontos:** Detectar pontos isolados envolve a aplicação de uma máscara específica e a convolução em toda a imagem. Um ponto é detectado se o valor absoluto da soma dos pixels sob a máscara for maior que um limiar.
  
- **Linhas:** A detecção de linhas pode ser feita com máscaras horizontais, verticais e diagonais, onde os valores de uma máscara determinam a orientação da linha.
  
- **Bordas:** A detecção de bordas é essencial para identificar descontinuidades em imagens em tons de cinza. As bordas representam o limite entre regiões com propriedades de cinza diferentes. Mudanças abruptas nos níveis de cinza indicam bordas e podem ser detectadas usando derivadas de primeira e segunda ordem.

#### Limiarização
A limiarização é um método de segmentação que envolve a conversão de uma imagem em tons de cinza em uma imagem binária, onde os pixels são classificados como pertencentes a uma região ou não, com base em um valor limiar.

#### Watershed

##### Definição
A transformação Watershed é uma ferramenta fundamental de segmentação em Morfologia Matemática. Ela pode ser compreendida como o preenchimento de uma superfície topográfica simulada por uma imagem numérica, iniciando a partir de mínimos locais (marcadores) e construindo diques para evitar a junção de fluxos de água.

##### Algoritmo
O processo de identificação do contorno inicia atribuindo um marcador a cada região a ser contornada. Um algoritmo baseado em fila de prioridade simula o crescimento das regiões, onde cada ponto é extraído da fila e agregado à região correspondente. Pontos que são vizinhos de duas regiões com rótulos diferentes são identificados como pontos de borda.
