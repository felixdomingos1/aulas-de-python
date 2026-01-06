
---

# **📄 README.md para o GitHub**

````markdown
# Curso de Python para Análise de Dados e Estruturas de Dados

Este repositório contém o material do curso de Python para análise de dados e estruturas de dados, organizado para **1 mês**, com **2 aulas por semana** e **2 horas por aula**.

---

## 📌 Objetivo do Curso

- Aprender Python do zero  
- Compreender estruturas de dados: listas, tuplas, dicionários, pilhas, filas e conjuntos  
- Introdução a bibliotecas para análise de dados: NumPy e Pandas  
- Realizar análises de datasets reais e visualizar informações  
- Preparar alunos para projetos de dados simples

---

## 🛠️ Pré-requisitos

- Computador com Ubuntu 24.04 (ou outro sistema)  
- Git instalado: [Instruções Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)  
- Editor de código (recomendado: [VS Code](https://code.visualstudio.com/))  
- Conexão com internet para instalar Python e bibliotecas

---

## 1️⃣ Instalação do Python e Ambiente

### Passo 1: Atualizar pacotes
```bash
sudo apt update
sudo apt upgrade -y
````

### Passo 2: Instalar Python 3 e pip

```bash
sudo apt install python3 python3-pip python3-venv -y
```

Verificar versões:

```bash
python3 --version
pip3 --version
```

### Passo 3: Criar ambiente virtual

```bash
mkdir ~/python-data
cd ~/python-data
python3 -m venv venv
source venv/bin/activate
```

> ⚠️ Sempre que for trabalhar nos exercícios, ative o ambiente com `source venv/bin/activate`.

---

## 2️⃣ Instalação das Bibliotecas

```bash
pip install numpy pandas matplotlib seaborn jupyterlab
```

* **NumPy** → operações matemáticas e vetores/matrizes
* **Pandas** → manipulação de tabelas (DataFrames)
* **Matplotlib / Seaborn** → visualização de gráficos
* **JupyterLab** → notebooks interativos

---

## 3️⃣ Estrutura do Curso

| Semana | Aula | Tópico                       | Conteúdo Principal                                   | Exercícios                                                       |
| ------ | ---- | ---------------------------- | ---------------------------------------------------- | ---------------------------------------------------------------- |
| 1      | 1    | Introdução e Tipos de Dados  | Python, variáveis, int, float, str, bool, operadores | Criar variáveis, calcular média de números                       |
| 1      | 2    | Estruturas Básicas           | Listas, tuplas, dicionários, conjuntos, compreensão  | Lista de notas, dicionário com nomes/id, conjunto sem duplicatas |
| 2      | 3    | Condicionais e Funções       | if, else, elif, funções com return                   | Verificar par/ímpar, calcular média, retornar maior número       |
| 2      | 4    | Loops                        | for, while, break, continue, pass                    | Somar lista, contagem regressiva, iterar dicionário              |
| 3      | 5    | Pilhas, Filas, Conjuntos     | Stack, Queue, set operations                         | Implementar pilha, fila, operações com conjuntos                 |
| 3      | 6    | NumPy                        | Arrays, indexação, slicing, operações vetorizadas    | Array 1-10, média, soma, operações entre arrays                  |
| 4      | 7    | Pandas – DataFrames e Séries | Ler CSV, selecionar colunas/linhas, filtros          | Ler CSV alunos, média de notas, filtrar alunos                   |
| 4      | 8    | Agrupamento e Visualização   | groupby, gráficos de barra, linha e pizza            | Agrupar alunos, gráficos de médias, gráficos de aprovação        |

---

## 4️⃣ Como Executar os Exercícios

1. Ativar o ambiente virtual:

```bash
cd ~/python-data
source venv/bin/activate
```

2. Abrir JupyterLab:

```bash
jupyter-lab
```

3. Abrir o notebook correspondente à aula (ex.: `01_fundamentos.ipynb`)
4. Executar as células uma a uma (`Shift + Enter`)
5. Salvar progresso e enviar resultados se necessário

---

## 5️⃣ Recursos Extras

* [Python Oficial](https://www.python.org/)
* [Jupyter Notebook](https://jupyter.org/)
* [NumPy Documentation](https://numpy.org/doc/)
* [Pandas Documentation](https://pandas.pydata.org/docs/)
* Dataset de prática: [Titanic CSV](https://www.kaggle.com/c/titanic/data)

---

## 6️⃣ GitHub: Estrutura de Pastas

```
python-data/
├── 01_fundamentos.ipynb
├── 02_estruturas_basicas.ipynb
├── 03_condicionais_funcoes.ipynb
├── 04_loops.ipynb
├── 05_pilhas_filas_conjuntos.ipynb
├── 06_numpy.ipynb
├── 07_pandas_dataframe_series.ipynb
├── 08_agrupamento_visualizacao.ipynb
└── README.md
```

---

> 🎯 **Dica:** Faça commit de cada notebook após finalizar a aula e suba para o GitHub. Isso ajuda os alunos a acompanhar e ter exemplos prontos para estudo.

---

## 7️⃣ Comandos Git para subir as aulas

```bash
cd ~/python-data
git init
git add .
git commit -m "Adicionar material do curso de Python - Aula 1 a 8"
git branch -M main
git remote add origin [<URL_DO_REPOSITORIO>](https://github.com/felixdomingos1/aulas-de-python)
git push -u origin main
```

> Substitua `[<URL_DO_REPOSITORIO>](https://github.com/felixdomingos1/aulas-de-python)` pela URL do teu repositório GitHub.
