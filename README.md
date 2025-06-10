# MLP_CLASSIFIER
REVISÃO DE DESEMPENHO ESCOLAR UTILIZANDO REDES NEURAIS  ARTIFICIAIS (MLP) 
Este repositório contém o projeto desenvolvido para prever o desempenho escolar de estudantes utilizando Redes Neurais Artificiais (MLP). O objetivo é classificar se um estudante será aprovado ou reprovado com base em diversas características.

🎯 Objetivo
O principal objetivo deste projeto é construir um modelo de Machine Learning capaz de prever o desempenho final de estudantes (aprovado/reprovado) em uma disciplina, utilizando dados demográficos, sociais, familiares e de desempenho acadêmico prévio. A nota de corte para aprovação foi definida como G3 ≥ 10.

📊 Conjunto de Dados
O dataset utilizado, student-por.csv, é uma adaptação do conjunto de dados de desempenho de estudantes de Português, originalmente disponível no UCI Machine Learning Repository. Ele contém 33 atributos, incluindo:
Características da Escola: school, address, famsize, Pstatus
Características Pessoais: sex, age, Medu, Fedu, Mjob, Fjob, reason, guardian, traveltime, studytime, failures, schoolsup, famsup, paid, activities, nursery, higher, internet, romantic
Características de Relacionamento Social: famrel, freetime, goout, Dalc, Walc, health
Desempenho Anterior e Faltas: absences, G1, G2
Variável Alvo: G3 (nota final, convertida para classificação binária: 1 para aprovado, 0 para reprovado)

🧠 Metodologia
O projeto segue as seguintes etapas:
Carregamento e Análise Exploratória de Dados (EDA): Leitura do dataset e primeiras análises estatísticas e visuais para entender a distribuição dos dados e identificar possíveis relações.
Pré-processamento de Dados: Tratamento de variáveis categóricas (one-hot encoding), normalização de variáveis numéricas e divisão do dataset em conjuntos de treino e teste.
Balanceamento de Classes: Aplicação de técnicas de oversampling (utilizando RandomOverSampler do imblearn) para mitigar o problema de desbalanceamento entre as classes de aprovados e reprovados.
Modelagem: Construção e treinamento de um modelo de Rede Neural Perceptron Multicamadas (MLPClassifier do sklearn).
Avaliação do Modelo: Avaliação do desempenho do modelo utilizando métricas como acurácia, precisão, recall, F1-score e matriz de confusão.

🛠️ Tecnologias Utilizadas
Python
Bibliotecas:
pandas e numpy para manipulação e análise de dados.
matplotlib.pyplot e seaborn para visualização de dados.
scikit-learn (sklearn) para pré-processamento, modelagem (MLPClassifier) e avaliação.
imbalanced-learn (imblearn) para balanceamento de classes.

🚀 Como Executar o Projeto
Para replicar e executar este projeto, siga os passos abaixo:
Clone o Repositório:
bash
git clone [LINK_DO_SEU_REPOSITORIO]
cd [NOME_DO_SEU_REPOSITORIO]

Crie um Ambiente Virtual (Opcional, mas Recomendado):
bash
python -m venv venv
source venv/bin/activate  # No Windows: .venv\Scripts\activate

Instale as Dependências:
bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn jupyter

Execute o Jupyter Notebook:
bash
jupyter notebook script.ipynb
Isso abrirá o Jupyter Notebook no seu navegador, onde você poderá executar as células e ver o projeto em ação.

📄 Arquivos do Projeto
script.ipynb: O Jupyter Notebook contendo todo o código do projeto, desde a análise exploratória até a avaliação do modelo.
student-por.csv: O conjunto de dados utilizado para o treinamento e teste do modelo.
PREVISÃODEDESEMPENHOESCOLARUTILIZANDOREDESNEURAISARTIFICIAIS(MLP).pdf: O relatório detalhado do projeto (se aplicável, caso contrário, remova esta linha).

🤝 Contribuição
Sinta-se à vontade para explorar o código, sugerir melhorias ou relatar problemas. Contribuições são sempre bem-vindas!
