![Logos Ilum, CNPEM, MEC, MCTI e Governo Federal](https://github.com/user-attachments/assets/063a52e7-6fc5-47c8-b220-d91f73956f38)

<h1 align='center'> Predição do tempo de síntese de materiais Organometálicos - Projeto Final de Aprendizado de Máquina </h1>

## Desenvolvedores
[<img src="https://avatars.githubusercontent.com/u/172425156?v=4" width=115>](https://github.com/leticiaalmnunes)
[<img src="https://avatars.githubusercontent.com/u/172425353?v=4" width=115>](https://github.com/Rafaela-Luz)
[<img src="https://avatars.githubusercontent.com/u/172425104?v=4" width=115>](https://github.com/ThomasHannemann)

* Letícia Almeida Nunes, Ilum Escola de Ciência, Centro Nacional de Pesquisa em Energia e Materiais
* Rafaela Beatriz Silva Luz, Ilum Escola de Ciência, Centro Nacional de Pesquisa em Energia e Materiais
* Thomas Wolff Hannemann, Ilum Escola de Ciência, Centro Nacional de Pesquisa em Energia e Materiais

## ÍNDICE
* [Desenvolvedores](#desenvolvedores)
* [Índice](#índice)
* [Descrição do projeto](#descrição-do-projeto)
  - [Motivação e objetivo principal](#motivação-e-objetivo-principal)
* [Como reproduzir o trabalho](#como-reproduzir-o-trabalho)
  - [Arquivos](arquivos)
* [Informações técnicas](#informações-técnicas)
* [Contribuições](#contribuições)
* [Agradecimentos](#agradecimentos)

## Descrição do projeto
**Projeto final em grupo da discilplina Aprendizado de Máquina do 2º semestre da turma 2024 do bacharelado em Ciência e Tecnologia da Ilum Escola de Ciência (CNPEM).**

A partir do conhecimento adquirido ao longo da disciplina ministrada pelo Professor Daniel Cassar, os *Arautos do Crepúsculo* (Grupo 6) desenvolveram um modelo de aprendizado supervisionado que visa, a partir de algumas características da síntese de um MOF, predizer o seu tempo.

### Motivação e objetivo principal
A duração da síntese é uma variável interessante para predizer, pois, sabendo o tempo que o material leva para ser sintetizado ou o controlando a partir da alteração das demais variáveis (e.g. temperatura e aditivos) é possível administrar melhor os recursos e as demais atividades que devem ser realizadas no laboratório.

## Como reproduzir o trabalho
Os *notebooks Jupyter* e demais arquivos presentes no repositório contêm todas as intruções e os dados necessários para que o trabalho seja reproduzido. Seguindo os cadernos na ordem que estão numerados, o leitor não terá qualquer dificuldade de acompanhar o processo.

Outrossim, caso não possua armazenamento, tempo ou um HPC para rodar todos os cadernos, os arquivos neles gerados também estão todos aqui no repositório.

### Arquivos
- **RAC_treino:** Conjunto de dados original obtido na plataforma [Kaggle](https://www.kaggle.com/datasets/marquis03/metal-organic-frame-materials-prediction/data).

- **RAC_treino_split:** Conjunto de dados usados para os treinos do modelo.
- **RAC_teste_split:** Conjunto de dados usados para os testes do modelo. <br><br>

- **RAC_treino_var:** Dados de treino com os atributos pré-selecionados por limiar da variância.
- **RAC_teste_var:** Dados de teste com os atributos pré-selecionados por limiar da variância.

- **RAC_treino_VIF:** Dados de treino com os atributos selecionados por VIF para o modelo Regressor k-NN.
- **RAC_teste_VIF:** Dados de teste com os atributos selecionados por VIF para o modelo Regressor k-NN.

- **RAC_treino_arvore:** Dados de treino com os atributos selecionados por RFE para o modelo Árvore de decisão.
- **RAC_teste_arvore:** Dados de teste com os atributos selecionados por RFE para o modelo Árvore de decisão.

- **RAC_treino_floresta:** Dados de treino com os atributos selecionados por RFE para o modelo Floresta aleatória.
- **RAC_teste_floresta:** Dados de teste com os atributos selecionados por RFE para o modelo Floresta aleatória. <br><br>

- **Caderno 0 - Relatório:** Relatório contendo a descrição de todo o processo executado nos cadernos seguintes.
- **Caderno 1 - Split de Dados:** Separação dos dados em treino e teste.
- **Caderno 2 - Seleção de atributos:** Seleção dos atributos para cada modelo por VIF e RFE.
- **Caderno 3.0 - Baseline:** Modelo baseline para avaliação dos demais.
- **Caderno 3.1 - Regressor k-NN:** Modelo Regressor k-NN.
- **Caderno 3.2 - Árvore de decisão:** Modelo Árvore de decisão.
- **Caderno 3.3 - Floresta aleatória:** Modelo Floresta aleatória.
- **Caderno 4 - Comparação dos modelos:** Comparando as métricas de performance dos modelos treinados.
- **Caderno 5 - Modelo final:** Caderno contendo apenas o modelo selecionado para ser utilizado.
- **RMSE_x_Modelo.png**: Gráfico com a métrica de performance por modelo.

## Informações técnicas
* Linguagem de programação
  - Python 3.9
* Software
  - Jupyter Notebook
* Bibliotecas
  - Pandas
  - Scikit-Learn
  - Optuna

## Contribuições
HANNEMANN, Thomas: Split dos dados, Regressor k-NN e Floresta Aleatória.
<br><br>
LUZ, Rafaela: Seleção de atributos, relatório e organização dos arquivos.
<br><br>
NUNES, Letícia: Árvore de decisão, relatório, README.
<br><br>

## Agradecimentos
Agrademos ao professor Daniel Cassar por nos instruir com tamanho bom humor e pela paciência para tirar nossas dúvidas constantes. Agradecemos também à professora Valéria Spolon pelos esclarecimentos acerca da síntese dos materais organo-metálicos e aos veteranos que nos ensinaram a usar o HPC.
