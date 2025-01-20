# Previsão de Falhas em Máquinas com IoT Data

Este projeto utiliza dados de sensores IoT para prever falhas em máquinas, ajudando a implementar manutenção preditiva. O objetivo é reduzir o tempo de inatividade e os custos operacionais.

---

## **1. Descrição do Problema**
Máquinas industriais frequentemente enfrentam falhas que podem interromper as operações. Usando dados de sensores coletados ao longo do tempo, podemos criar modelos preditivos para identificar possíveis falhas antes que ocorram.

---

## **2. Estrutura do Projeto**

### **2.1. Dataset**
- **Fonte:** NASA Turbofan Engine Degradation Simulation Dataset ou dados semelhantes do Kaggle.
- **Descrição:** Dados de sensores coletados em intervalos de tempo, incluindo variáveis como temperatura, pressão, vibração, entre outros.
- **Objetivo:** Prever a ocorrência de falhas em máquinas com base em padrões detectados nos sensores.

### **2.2. Ferramentas e Tecnologias**
- **Linguagem:** Python
- **Bibliotecas:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, TensorFlow/PyTorch (opcional para redes neurais).

### **2.3. Estrutura de Diretórios**
```plaintext
├── data
│   ├── raw_data.csv   # Dados brutos
│   ├── processed_data.csv # Dados processados
├── notebooks
│   ├── 01_exploratory_analysis.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_model_training.ipynb
├── models
│   ├── xgboost_model.pkl
│   ├── lstm_model.h5
├── app
│   ├── app.py         # API para predições
├── README.md          # Documentação do projeto
```

---

## **3. Etapas do Projeto**

### **3.1. Análise Exploratória de Dados (EDA)**
- Carregamento do dataset.
- Análise estatística (média, mediana, variância).
- Visualização de correlações entre sensores.

### **3.2. Pré-processamento**
- Tratamento de valores ausentes.
- Normalização/padronização dos dados.
- Criação de variáveis derivadas (ex.: taxas de variação).
- Divisão do dataset em conjuntos de treino e teste.

### **3.3. Modelagem Preditiva**
- **Modelos utilizados:**
  - Random Forest
  - XGBoost
  - Redes Neurais (LSTM para séries temporais).
- **Avaliação:**
  - Acurácia
  - F1-Score
  - Matriz de confusão
  - ROC/AUC

### **3.4. Visualização de Resultados**
- Gráficos de desempenho dos modelos.
- Visualização de importância das features.

### **3.5. API para Predições em Tempo Real**
- Implementação de uma API usando Flask ou FastAPI.
- Endpoint para upload de dados e retorno da predição.

---

## **4. Resultados Obtidos**
- **Modelo com melhor desempenho:** [Especificar modelo].
- **Métricas:**
  - Acurácia: [Valor]
  - F1-Score: [Valor]
  - AUC: [Valor]
- **Gráficos:** [Incluir exemplos no repositório]

---

## **5. Como Executar o Projeto**

### **5.1. Clonar o Repositório**
```bash
https://github.com/usuario/nome-do-repositorio.git
```

### **5.2. Instalar Dependências**
```bash
pip install -r requirements.txt
```

### **5.3. Executar a Análise**
1. Navegue até a pasta `notebooks` e abra os arquivos Jupyter.
2. Execute as etapas na ordem:
   - 01_exploratory_analysis.ipynb
   - 02_preprocessing.ipynb
   - 03_model_training.ipynb

### **5.4. Executar a API**
```bash
cd app
python app.py
```

---

## **6. Próximos Passos**
- Adicionar visualização interativa usando Streamlit.
- Expandir para outros datasets de IoT.
- Implementar pipeline automatizado para treinamento e deploy do modelo.

---

## **7. Contribuição**
Contribuições são bem-vindas! Abra uma issue ou envie um pull request para melhorar o projeto.

---

## **8. Licença**
Este projeto está licenciado sob a Licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## **9. Contato**
**Autor:** Yan Furlan  
**E-mail:** [yangabrielfurlan@gmail.com](mailto:yangabrielfurlan@gmail.com)  
**LinkedIn:** [LinkedIn](https://www.linkedin.com/in/yan-furlan-455ab820b/)

