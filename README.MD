# Disruptive Architectures IOT e IA

Vídeo: URL_AQUI

## Tabela de conteúdos

- [Justificativas](#justificativas)
- [Como executar](#como-executar)
- [Integrantes](#integrantes)

## Justificativas

- **Pré-processamento de dados:** Para a normalização dos dados, o dataset é modificado em tempo de execução, gerando um novo arquivo contendo os dados normalizados (para visualização do usuário em quais foram os dados que foram modificados). Lembrando que, os dados são carregados em memória então o dataset permanecerá intacto mesmo após as modificações exercidas.\
  Dentro do próprio notebook pode ser encontrado a seção da **definição do dicionário de dados**, que contém os detalhes de cada atributo que compõe o dataset sendo que, apenas a coluna **id** foi desconsiderada da análise final e todas as outras que os valores não excedem os limites de **0.0** e **1.0** são normalizadas.
- **Escolha do algoritmo utilizado:** Para este projeto, foi definido o algoritmo de análise KNN (k-nearest neighbors) como algoritmo de aprendizagem de máquina e classificação.\
  Como o dataset em questão é simples, e o algoritmo necessita poucas entradas (as amostras de treinamento, a amostra de teste - para definir se o algoritmo chega na mesma classe que a amostra possui e o K procurado) para a aprendizagem e treinamento do modelo, optamos por seguir com ele.
- **Atributos categóricos e não categóricos:** Como o dataset em questão não possui os detalhes para definir qual o peso de cada atributo em relação a análise final do algoritmo, foi definido que a normalização de cada atributo deve estar entre os valores **0.0** e **1.0**, sendo assim, nenhum dos atributos tem um peso maior que o outro.\
  Quanto a escolha da normalização, podem ser conferidos no próprio notebook onde são definidas as chaves contendo as posições de cada coluna do dataset (iniciando na posição 0 - por se tratar de um vetor) contendo os seguintes **parâmetros**:

  - **vmin:** define o valor mínimo para normalização dos dados;
  - **vmax:** define o valor máximo para normalização dos dados;
  - **remove (opcional) [Padrão: ignorar]:** caso esteja habilitado, remove a coluna da análise;
  - **decimal (opcional) [Padrão: 2 casas decimais]:** aponta a quantidade de casas decimais a ser utilizado;
  - **normalize (opcional) [Padrão: normalizar]:** indica se a coluna deve ter o valor modificado para uma escala normalizada ou o valor deve ser mantido sem alterações.

- **Métricas adotadas para avaliar a performance do modelo criado:** Ainda no que tange a normalização, em cada um dos atributos foi definido o seu respectivo valor mínimo (identificado) e o valor máximo (identificado).\
  Como o dataset possui ao total **132 amostras**, foi realizado o cálculo de raiz quadrada e definida que o k seria o valor de número **11** para minimizar a chance de a amostra analisada e o valor identificado da classe ser ambíguo em ambas.\
  Foi definido também que a separação de amostras seria 70% (treinamento) e 30% (teste), por ser uma convenção na análise do algoritmo de aprendizagem.\
  O Percentual de acerto e de erro pode ser conferido na execução do notebook.

## Como executar

Para realizar os testes, é necessário:

- Ter python instalado na máquina e:
  - Jupyter Notebook (pode ser instalado com o [pip](https://jupyter.org/install#installation-with-pip-1)) ou;
  - Visual Studio Code (com as extensões do [python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) e [jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter), ambas da própria Microsoft).

Após isso, clone este repositório com `git clone https://github.com/RANGO-Corp/IOT.git` ou baixe o zip diretamente e o extraia.

Em seguida, abra o diretório onde se encontra este projeto baixado e execute-o com:

- se estiver no jupyter: `jupyter notebook analysis.ipynb`
- ou se estiver no Visual Studio Code, apenas abra o projeto.

Logo em seguida, execute cada uma das células executáveis para definir as funções e visualizar o resultado final.

## Integrantes

| Turma | 2TDST                                |
| :---: | ------------------------------------ |
|  RM   | Integrante                           |
|       |                                      |
| 84198 | Daiane Estenio dos Santos            |
| 84717 | Jacó Magalhães I Sen Chen            |
| 85568 | João Victor Pessoa Queiroz           |
| 85398 | Luís Fernando Pedro Paulino da Silva |
