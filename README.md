
Treinei modelos de aprendizado de máquina para classificar três tipos de animais: gatos, cachorros e leões, utilizando o dataset "Animals" disponível no Kaggle (https://www.kaggle.com/datasets/antobenedetti/animals). 

Foram utilizadas diferentes quantidades de imagens para gerar os modelos e avaliar seu desempenho. Utilizei em especial fotos da minha cachorra para os testes. Abaixo, apresento um resumo dos procedimentos e resultados.

Dataset Completo contém:

- 2675 imagens de leões

- 2627 imagens de cachorros

- 2737 imagens de gatos

# **Parâmetros de Treinamento**

Todos os modelos foram treinados utilizando os seguintes parâmetros:

Epochs: 50

Batch Size: 16

Learning Rate: 0.001

# **Modelos Gerados**

1. *Modelo com 10 Imagens de Leões, Cachorros e Gatos*: 

Arquivo: ``model-10-images.tm``

2. *Modelo com 100 Imagens de Leões, Cachorros e Gatos*:

Arquivo: ``model-100-images.tm``

3. *Modelo com 400 Imagens de Leões, Cachorros e Gatos*: arquivo model-490-images.tm

Arquivo: ``model-400-images.tm``

# **Resultados dos Modelos**

*Modelo com 10 Imagens de Leões, Cachorros e Gatos*

O modelo treinado com apenas 10 imagens por tipo de animal apresentou resultados significativamente inferiores. Embora tenha conseguido classificar corretamente algumas imagens, a precisão foi baixa e, em alguns casos, a classificação foi incorreta. Por exemplo, ao submeter uma foto da minha cachorra, o modelo a identificou erroneamente como um leão. Este resultado evidencia a importância de ter um conjunto de dados suficiente para treinar modelos de aprendizado de máquina de forma eficaz.

*Modelo com 100 Imagens de Leões, Cachorros e Gatos*

O modelo treinado com 100 imagens por tipo de animal apresentou resultados razoáveis. Ao submeter uma foto da minha cachorra, o modelo a classificou corretamente como cachorro com 90% de certeza. No entanto, ainda houve uma incerteza, com 9% de certeza sendo atribuída à classe leão e 1% à classe gato. Isso indica que, embora o modelo tenha uma boa capacidade de classificação, ele ainda pode ser aprimorado para reduzir a incerteza residual.

*Modelo com 400 Imagens de Leões, Cachorros e Gatos*

Após o treinamento com 400 imagens, a imagem invertida da minha cachorra foi classificada com 22% como cachorro, 1% como gato e 77% como leão. Isso sugere que o modelo continua tendo dificuldades em reconhecer corretamente, possivelmente devido a características específicas da imagem ou a limitações na capacidade do modelo em generalizar para casos diversos.

# **Conclusão**

Os resultados destacam a importância da quantidade e diversidade de dados de treinamento para alcançar alta precisão e confiabilidade em modelos de aprendizado de máquina. Embora o dataset "Animals" do Kaggle tenha permitido a criação de modelos para a identificação de gatos, cachorros e leões, ainda há espaço para melhorias, especialmente em modelos treinados com conjuntos de dados menores, onde a incerteza pode ser mais proeminente.
