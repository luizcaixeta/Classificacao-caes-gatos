## Classificação de Cães e Gatos com CNN: Estudo do funcionamento de uma CNN  

Este repositório contém um estudo completo sobre a construção de uma **Rede Neural Convolucional (CNN)** para classificação de imagens de cães e gatos. O projeto foi desenvoldido em um Jupyter Notebook e aborda desde o pré-processamento dos dados até a avaliação do modelo final.

### Descrição do projeto 

O objetivo deste projeto é demonstrar o funcionamento de uma CNN para classificação binária de imagens (cães vs gatos). O estudo é dividido em várias etapas, incluindo:

1. Pré-processamento de dados com **ImageDataGenerator**:
   + Utilizamos o **ImageDataGenerator** do Keras para aumentar a variabilidade dos dados de treinamento. Essa técnica é essencial para evitar overffiting e melhorar a generalização do modelo, aplicand transformações como rotação, zoom, inversão horizontal e deslocamento de imagens.
  
2. Construção do modelo de CNN:
   + O modelo foi construído camada por camada, incluindo:
     + Camadas de Convolução: para extrair características das imagens (como bordas, texturas e padrões)
     + Camadas de Pooling: para reduzir a dimensionalidade e destacar as características mais importantes.
     + Camadas Fully Connected (Dense): para realizar a classificação final.

3. Entendendo o funcionamento do kernel e feature maps:
   + Durante o processo, exploramos como os kernels (filtros) atuam sobre as imagens para gerar **feature maps**, que representam as características aprendidas pela rede.
  
4. Definição das epochs:
   + Uma **epoch** corresponde a uma passagem completa pelo conjunto de dados de treinamento. Explicamos como o número de epochs impacta o aprendizado do modelo, evitando underfitting (poucas epochs) ou overfitting (muitas epochs).
  
5. Treinamento e avaliação do modelo:
   + O modelo foi treinado e avaliado utilizando métricas como acurácia e loss, tanto para os dados de treinamento quanto para os de validação.       
