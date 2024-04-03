## Previsão de Risco Cardíaco 

Esse projeto foi realizado em sala de aula, no último semestre do Curso de Ciência de Dados. 
Foi ultilizado o algoritimo KNN (K-Nearest Neighbors) é um algoritmo de aprendizado de máquina supervisionado usado para classificação e regressão. 
É um algoritmo simples e intuitivo que funciona com base no princípio da similaridade.

## Base de Dados
(Dados Fictícios)
Colunas:
(['ID', 'Idade', 'Peso', 'Altura', 'Pressao_Sistolica',
       'Pressao_Diastolica', 'Nivel_Glicose', 'Tempo_Exercicio_Semanal',
       'Consumo_Alcool_Semanal', 'Contagem_Globulos_Brancos',
       'Contagem_Globulos_Vermelhos', 'Indice_Massa_Corporal',
       'Nivel_Colesterol', 'Frequencia_Cardiaca', 'Nivel_Estresse',
       'Horas_Sono_Dia', 'Risco'].
       
- Foram removidas as colunas ID e Risco.
- Para Target foi usado a coluna Risco
- Possui 4.000 linhas
- 65.8% de pessoas que possuem risco cardíaco, equivalente a 2632.0 linhas.
- 34.2% de pessoas que não possuem risco cardíaco, equivalente a 1368.0 linhas.
  
- Foram gerados alguns gráficos para análises.
- Matriz de Correlação: 
 ![image](https://github.com/iancaabreu/Projeto-1/assets/102169504/29ae9f7a-12d4-4b88-9271-e675c528124d)
- Gráfico de Histograma:
 ![image](https://github.com/iancaabreu/Projeto-1/assets/102169504/ccdc9a31-030f-42db-9be3-affa317fc918)
- Gráfico Boxplot:
 ![image](https://github.com/iancaabreu/Projeto-1/assets/102169504/43bd79fd-37a5-4f8e-aee6-495e9c39a83a)
- Gráfico ECDF Plots:
  ![image](https://github.com/iancaabreu/Projeto-1/assets/102169504/9b4bfe62-bb49-4a89-a32d-683142806efd)

## Colunas usadas para treinamento:
models_cols = ['Pressao_Sistolica', 'Pressao_Diastolica', 'Nivel_Glicose', 'Indice_Massa_Corporal']

## Resultado 

![image](https://github.com/iancaabreu/Projeto-1/assets/102169504/9cf0158a-e848-4dc5-9b5a-cbc44db86864)


## Funcionamento do KNN 
- Fase de Treinamento: Na fase de treinamento, o algoritmo simplesmente memoriza as características e rótulos dos dados de treinamento.
- Fase de Previsão: Quando um novo ponto de dados precisa ser classificado (ou previsto no caso de regressão), o algoritmo olha para os 'k' pontos de dados mais próximos (vizinhos) no espaço das características.
- Classificação: Para tarefas de classificação, o algoritmo atribui o rótulo de classe mais comum entre os 'k' vizinhos mais próximos.
- Regressão: Para tarefas de regressão, o algoritmo prevê a média dos valores-alvo dos 'k' vizinhos mais próximo.

## Conclusão  

A análise do projeto de previsão de risco cardíaco usando o algoritmo K-Vizinhos Mais Próximos (KNN) revelou resultados promissores. Com uma dimensão de dados de (4000, 4), o modelo foi treinado para prever com sucesso o risco cardíaco.

Ao otimizar os parâmetros do modelo KNN, determinou-se que o melhor conjunto de hiperparâmetros era {'metric': 'manhattan', 'n_neighbors': 15}, resultando em um impressionante score de validação cruzada de 0.9667. Isso sugere que o modelo KNN é altamente capaz de distinguir entre diferentes níveis de risco cardíaco com uma precisão significativa.

Em comparação com o modelo de Regressão Logística, observamos que o KNN superou significativamente em termos de desempenho, com uma pontuação de validação cruzada substancialmente mais alta.

Esses resultados indicam que o modelo KNN é altamente promissor para previsão de risco cardíaco neste conjunto de dados específico. No entanto, para uma implementação bem-sucedida em ambientes clínicos ou práticos, é essencial realizar validações adicionais, incluindo testes em conjuntos de dados independentes e considerar a interpretabilidade do modelo.






  
