# Disruptive Architectures IOT e IA

Vídeo: URL_AQUI

## Tabela de conteúdos

- [Justificativas](#justificativas)
- [Como executar](#como-executar)
- [Integrantes](#integrantes)

## Justificativas

- **Pré-processamento de dados:** Para a normalização dos dados, foi utilizado o próprio notebook desconsiderando apenas a coluna de id visto que ela não auxiliaria na identificação da classe das amostras.

- **Escolha do algoritmo utilizado:** Para este projeto, foi definido o algoritmo de análise KNN para definição e classificação das amostras. Pelo dataset ser simples e conter poucos dados, não necessitando de um algoritmo complexo para análise dos mesmos.

- **Atributos categóricos e não categóricos:** Quanto aos dados e a escolha da normalização, podem ser conferidos no próprio notebook onde são definidas as chaves contendo as posições de cada coluna do dataset (iniciando na posição 0 - por se tratar de um vetor) contendo os seguintes parâmetros:

  - **vmin:** define o valor mínimo para normalização dos dados;
  - **vmax:** define o valor máximo;
  - **remove (opcional):** caso esteja habilitado, remove a coluna da análise;
  - **decimal (opcional):** aponta a quantidade de casas decimais a ser utilizado (padrão: 2 casas decimais)
  - **normalize (opcional):** indica se a coluna deve ter o valor modificado para uma escala normalizada (padrão) ou o valor deve ser mantido sem alterações.

- **Métricas adotadas para avaliar a performance do modelo criado:**

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
