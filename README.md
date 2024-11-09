# K-Means


## Descrição do Projeto: 
O projeto realiza a clusterização do dataset Iris utilizando o algoritmo K-Means, um método de aprendizado não supervisionado. O dataset Iris contém 150 amostras de flores, divididas igualmente entre três classes (Setosa, Versicolour, e Virginica) e possui quatro características: comprimento e largura das sépalas, e comprimento e largura das pétalas.


## Pré-processamento: 
* Carregamento e Seleção de Features: O dataset completo foi utilizado com todas as quatro características.
* Normalização: Utilizamos o StandardScaler para normalizar as variáveis, ajustando-as para uma média de 0 e desvio padrão de 1, a fim de melhorar o desempenho do K-Means.
* Definição de Clusters (K): O número de clusters foi definido como 3, correspondente às três classes do dataset.

  
## Modelo K-Means: 
* Treinamento
O modelo K-Means foi configurado para três clusters, correspondendo às três espécies de flores. A inércia e o silhouette score foram calculados para avaliar a qualidade dos clusters, onde inércia mede a soma das distâncias ao quadrado dos pontos aos seus respectivos centroides, enquanto o silhouette score avalia a coesão e separação dos clusters.

* Predição
O modelo ajustado foi utilizado para prever a qual cluster novos dados pertencem. Para facilitar a avaliação, os rótulos dos clusters foram ajustados para se alinhar com as classes conhecidas e em seguida foram calculadas a acurácia e a matriz de confusão para comparar os clusters preditos com as classes verdadeiras.


## Resultados obtidos:
* Acurácia:
O valor de acurácia alcançado foi de 0.67, o que representa uma taxa de 67% de classificação correta dos clusters em relação às classes verdadeiras. Apesar de não ser uma acurácia perfeita, este resultado é comum em cenários de clustering considerando que o K-Means não é supervisionado e não possui conhecimento prévio sobre as mesmas.


* Matriz de Confusão:
A matriz de confusão apresenta uma boa separação para as classes setosa e virginica, onde ambas foram classificadas corretamente, sem erros (50 amostras corretas).
A classe versicolor apresenta algumas dificuldades, com 4 amostras sendo incorretamente atribuídas aos clusters das outras classes.


![image](https://github.com/user-attachments/assets/ec40e286-299f-4d93-9ca3-274425f7150b)



* Visualização dos Clusters:
O gráfico mostra a distribuição dos clusters identificados pelo K-Means, destacando os centróides em vermelho.
Podem-se observar três agrupamentos distintos, com uma separação clara entre dois clusters (setosa e virginica), mas com um certo grau de mistura e sobreposição nas amostras do cluster correspondente a versicolor.


![image](https://github.com/user-attachments/assets/4d0c4de8-60bf-4918-a8ca-6977d5672648)
