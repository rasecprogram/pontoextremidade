## Passo a Passo

### 1. Desenvolvimento do Modelo de Previsão

- Utilizei Python e Scikit-learn para criar um modelo de regressão linear simples.
- Preparei dados de exemplo para treinamento do modelo.
- Treinei o modelo usando os dados preparados.

### 2. Configuração dos Pontos de Extremidade

- Utilizei o framework Flask para configurar os pontos de extremidade.
- Defini um ponto de extremidade para fazer previsões (`/predict`).
- Configurei a rota para aceitar solicitações POST contendo dados de entrada no formato JSON.
- Implementei uma função para fazer previsões com base nos dados de entrada.

### 3. Como Usar

1. Clone este repositório em sua máquina local.
2. Certifique-se de ter Python instalado em seu ambiente.
3. Instale as dependências listadas no arquivo `requirements.txt` executando `pip install -r requirements.txt`.
4. Execute o arquivo Python `app.py` para iniciar o servidor Flask.
5. Faça solicitações POST para `http://localhost:5000/predict` com os dados de entrada no formato JSON.

Exemplo de dados de entrada:
{
"input_data": [1]
}

### 4. Exemplo de Resposta

- Após fazer uma solicitação POST para `/predict`, você receberá a previsão do modelo no formato JSON.

Exemplo de resposta:

{
"prediction": [2.0]
}
