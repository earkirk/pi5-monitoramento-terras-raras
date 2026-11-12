Markdown
# Monitoramento Ambiental de Mineração de Terras Raras

MVP desenvolvido para o **Projeto Integrador V** do curso de Ciência de Dados da **FATEC Baixada Santista - Rubens Lara**.

## Sobre o Projeto
Pipeline automatizado de sensoriamento remoto e aprendizado de máquina para identificar e quantificar em hectares o impacto ambiental (supressão vegetal e exposição de solo) em áreas de mineração de terras raras a céu aberto, com estudo de caso na região de Araxá - MG.

## Tecnologias Utilizadas
* **Python** & **Streamlit** (Interface web interativa)
* **Google Earth Engine** (`ee` e `geemap`) (Processamento geoespacial em nuvem)
* **Imagens Sentinel-2** (Análise multiespectral com índices NDVI, NDWI e SWIR)
* **Random Forest** (Classificação supervisionada de cobertura do solo)

## Como Executar Localmente
1. Clone este repositório:
   ```bash
   git clone [https://github.com/earkirk/pi5-monitoramento-terras-raras.git](https://github.com/earkirk/pi5-monitoramento-terras-raras.git)
Instale as dependências:

Bash
pip install -r requirements.txt
Configuração das Credenciais (Google Earth Engine):

Crie uma Conta de Serviço (Service Account) vinculada a um projeto ativo no Google Cloud Console com a API do Google Earth Engine habilitada.

Baixe o arquivo de chave privada no formato JSON, renomeie-o para credentials.json e coloque-o na pasta raiz do projeto.

No arquivo app.py, substitua o parâmetro project='pi5-fatec-507412' (na função initialize_gee) pelo ID do seu próprio projeto no Google Cloud.

Execute a aplicação:

Bash
streamlit run app.py
