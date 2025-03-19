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
    
       ![image](https://github.com/user-attachments/assets/228e52ad-e715-4474-bf12-30f3e4ceed77)


3. Entendendo o funcionamento do kernel e feature maps:
   + Durante o processo, exploramos como os kernels (filtros) atuam sobre as imagens para gerar **feature maps**, que representam as características aprendidas pela rede.
  
   ![image](https://github.com/user-attachments/assets/d19fba71-4aa6-4acc-9ae5-ec57cb18c7b2)

  
4. Definição das epochs:
   + Uma **epoch** corresponde a uma passagem completa pelo conjunto de dados de treinamento. Explicamos como o número de epochs impacta o aprendizado do modelo, evitando underfitting (poucas epochs) ou overfitting (muitas epochs).
  
     ![image](https://github.com/user-attachments/assets/5270b7c4-c039-4413-90c0-a861236ec80d)

  
5. Treinamento e avaliação do modelo:
   + O modelo foi treinado e avaliado utilizando métricas como acurácia e loss, tanto para os dados de treinamento quanto para os de validação.
  
     Resultados:

          Acurácia no conjunto de teste: 93.00%
          Perda no conjunto de teste: 0.1696

## Como executar o projeto

1. Clone este repositório:
   ```git clone https://github.com/luizcaixeta/classificacao-caes-gatos-estudo-CNN ```

2. Execute o Jupyter Notebook:
   ```jupyter notebook notebooks/cat_and_dog.ipynb ```
