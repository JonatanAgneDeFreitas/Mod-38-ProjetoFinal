**Por:** [Jonatan Agne de Freitas](https://www.linkedin.com/in/jonatan-agne-de-freitas/)<br>

# 🧠 Aplicação de Scoring de Crédito com Streamlit

Este projeto é uma aplicação web interativa desenvolvida com **Streamlit**, que permite realizar a **escoragem de crédito** de forma simples e eficiente.

O usuário pode carregar um arquivo `.csv` contendo os dados a serem avaliados, e a aplicação utiliza um modelo de machine learning treinado — salvo como `model_final.pkl` — para calcular um **score de crédito** individual para cada registro. O resultado pode ser visualizado diretamente na interface e baixado como novo arquivo CSV com os scores.

A aplicação já inclui o carregamento do modelo, pré-processamento dos dados via pipeline e interface amigável para facilitar o uso mesmo por pessoas não técnicas.

---

[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=Streamlit&logoColor=white)]()

### . Instale as dependências

```bash
pip install -r requirements.txt
```

---

## 📤 Como usar a aplicação

1. Faça upload de um arquivo `.csv` com os dados a serem escorados.
2. O modelo será carregado e aplicado aos dados.
3. Os scores serão exibidos na tela e você poderá baixar um novo `.csv` com a coluna `score`.

---

## 📌 Observações Técnicas

- O pipeline de pré-processamento inclui uma classe customizada chamada `AplicarPCA`.
- A aplicação utiliza `predict_proba` para calcular a probabilidade da classe positiva.
- Certifique-se de que o formato do `.csv` enviado seja compatível com o modelo treinado.

---
