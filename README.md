# FTL BOOTCAMP - ANGOLA - GRUPO Nº 17 - Projecto Final
# Motor de Insights para Planeamento Turístico Sustentável
# Ano: 2025  
# Equipa: Abel Chimbua Wanda, Bruno Yonng Leopoldo, Dorivaldo Albano Manuel, Eliano Ricardo Tavares, José Arão, Liliane Patrícia Neto, Mário Délcio da Silva


# Descrição
O Motor de Insights é uma plataforma de apoio à decisão e gestão desenvolvida para o **Ministério do Turismo de Angola**, que integra:
**Análise de dados turísticos**, **Previsões inteligentes** com *Machine Learning*, e uma **interface interativa web** para gestores públicos e analistas.
O sistema combina um **notebook analítico** (para geração e treino de modelos) com uma **versão web administrativa** desenvolvida em **Streamlit**, permitindo exploração, previsões e relatórios sobre o turismo sustentável em Angola.

# Objetivos Principais
- Centralizar e analisar dados turísticos nacionais.  
- Prever fluxos de visitantes e tendências sazonais.  
- Apoiar o planeamento económico e ambiental.  
- Promover a sustentabilidade no setor do turismo.

# Estrutura do Projeto
<img width="828" height="584" alt="Captura de Tela (42)" src="https://github.com/user-attachments/assets/45aaf46e-1baa-44dd-931c-fb0421f5b394" />

                      

# Instalação e Requisitos

### Dependências Principais
- Python ≥ 3.13  
- Pandas, Numpy: Para manipulação de dados.    
- Scikit-learn: Para modelagem preditiva (Random Forest, Regressão Linear)  
- Streamlit: para interface web interativa  
- Joblib: para facilitar e acelerar tarefas intensivas  
- Prophet / Statsmodels: para previsões temporais
- Matplotlib / Plotly: para visualização de dados  

Se quiser instalar todas as dependências de uma vez:
No seu cmd coloque o seguinte comando:
pip install -r requirements.txt

# Como executar o Projecto:
## 1º Faça download/fork do projecto na sua máquina;

## 2º Rodar o Python notebook, encontra-se em:
notebooks/motor-insights-turismo-angola.ipynb

## Instrução:
1. Abre o Jupyter Notebook ou VSCode.  
2. Executa todas as células em ordem.  
3. O notebook vai fazer o seguinte:
   - Gerar o dataset sintético ( em: data/raw/dados_sinteticos.csv);
   - Treinar o modelo RandomForest;
   - Avaliar as métricas (MAE, RMSE, R²);
   - Salvar o modelo em: src/Motor_de_Insights_Streamlit/models/modelo_sintetico.pkl.

Após a execução, o modelo e o dataset ficam prontos para uso no app Streamlit.

## 3º Executar a Aplicação Web (Streamlit)

### Passos:
1. No terminal, entra na pasta principal do projeto:
   cd src/Motor_de_Insights_Streamlit

2. Executa o app com este comando:
   streamlit run app.py
   
3. O Streamlit abrirá automaticamente no navegador (por padrão em:  
   http://localhost:8501)

##Para acessar a Área Administrativa
## Credenciais de Acesso

| Usuário     | Palavra-passe |
|--------------|----------------|
| admin        | @dorivalldo     |
| analista     | @brunoyonng     |
| analista1    | @lilianeneto    |

Os acessos e logouts ficam registados em `src/Motor_de_Insights_Streamlit/logs.csv.

# Funcionalidades Principais
✅ **Área Pública**
- Curiosidades turísticas, gastronomia e cultura.  
- Indicadores gerais (visitantes totais, taxa de ocupação média).  
- Links úteis para: (Governo de Angola, INE, PNUD, UNWTO).  

✅ **Área Administrativa (após login)**
- **Painel de Controlo** — métricas e indicadores principais.  
- **Explorar Dados** — filtro e visualização por província.  
- **Previsões** — previsão de visitantes futuros (modelo RandomForest).  
- **Comparar Províncias** — análise comparativa temporal.  
- **Sustentabilidade** — visualização de índices ambientais e mobilidade.  
- **Gerar Relatórios** — exportação (demo, pronto para PDF/DOCX/PPTX).  
- **Logs** — registo de sessões de utilizadores.

# Tecnologias Utilizadas
| Categoria | Tecnologias |
|------------|-------------|
| Linguagem  | Python |
| Análise de Dados | Pandas, NumPy, Scikit-learn |
| Visualização | Matplotlib, Streamlit Charts |
| Modelo de IA | RandomForestRegressor |
| Armazenamento | CSV, PKL (Joblib) |
| Interface Web | Streamlit |
| Documentação | Markdown / Notebook (Jupyter) |

# Fases de Desenvolvimento

| Fase | Descrição                           |         Resultado                           |
|------|-------------------------------------|---------------------------------------------|
| 1    | Planeamento e definição do problema | Estrutura conceptual                        |
| 2    | Levantamento de requisitos          | Variáveis e indicadores turísticos          |
| 3    | Modelo conceptual e tecnológico     | Fluxo de dados e arquitetura                |
| 4    | Preparação dos dados                | Criação de dataset sintético                |
| 5    | Modelagem e validação               | Modelos preditivos e métricas de desempenho |
| 6    | Implementação                       | Protótipo web interativo (Streamlit).       |

# Licença
Este projeto foi desenvolvido com fins académicos e de demonstração.  
Todos os dados sintéticos são simulados para uso educacional e não representam valores oficiais.
Este protótipo une ciência de dados, sustentabilidade e gestão pública — transformando informações em decisões inteligentes para o turismo angolano.

# Referências
Adepoju, A., & Akinsola, O. (2021). Digital transformation and tourism development in Sub-Saharan Africa. African Journal of Sustainable Development, 11(3), 45–62. 
Gunter, U., & Önder, I. (2022). Forecasting tourism demand with machine learning models: An empirical comparison. Tourism Management, 91, 104489. 
Hu, Y., & Song, H. (2023). Smart tourism governance and data-driven decision making. Journal of Sustainable Tourism, 31(4), 621–640. 
World Bank. (2023). International tourism, number of arrivals (Angola). World Development Indicators. 
UNDP. (2022). Digital transformation for sustainable development: Policy guidance for Africa. New York: United Nations Development Programme.

# 🌍 Motor Insights Turismo Angola — Documentação de Ferramentas e Decisões Técnicas

## 🧩 Ferramentas e Tecnologias Adicionais

Durante a expansão do projeto **Motor Insights Turismo Angola**, novas ferramentas e bibliotecas foram integradas para fortalecer a estrutura do Dashboard e otimizar o desempenho, a usabilidade e a visualização dos dados.

Estas ferramentas não estavam previstas na versão inicial, mas foram adicionadas com base em necessidades técnicas identificadas durante o desenvolvimento.

### 🧠 Frameworks e Bibliotecas Adicionadas

| Ferramenta | Função | Motivo da Escolha |
|-------------|---------|-------------------|
| **Django** | Backend robusto para gestão de APIs e autenticação | Necessário para suportar múltiplos módulos, utilizadores e segurança avançada, além de fácil integração com IA em Python |
| **Django REST Framework (DRF)** | Criação de endpoints REST para fornecer dados ao frontend | Permite separar o backend da interface e possibilita integração com futuros aplicativos móveis |
| **TailwindCSS** | Framework CSS moderno e leve | Tornou o layout responsivo e mais fácil de manter, com design sustentável e compatível com dark mode |
| **Chart.js** | Visualização de dados estatísticos e preditivos | Leve, interativo e ideal para dashboards web; mais simples de integrar que Plotly no frontend puro |
| **Leaflet.js** | Mapa interativo de Angola e indicadores regionais | Escolhido pela sua leveza, open-source e facilidade de integração com GeoJSON; ideal para destacar indicadores sustentáveis por província |
| **WeasyPrint** | Geração de relatórios PDF | Suporta HTML/CSS, permitindo converter o dashboard e análises em relatórios prontos para impressão e partilha institucional |
| **Prophet e Scikit-learn** | Modelos de previsão de visitantes e sustentabilidade | Usados para construir previsões temporais rápidas e precisas, alinhadas com a visão de IA aplicada ao turismo |
| **Whitenoise + Gunicorn** | Deploy e entrega estática eficiente | Garantem desempenho otimizado no servidor e simplificam o processo de deploy em serviços cloud como Render ou Railway |

### 💡 Justificativa geral

O uso dessas ferramentas foi guiado por três fatores principais:
1. **Sustentabilidade técnica:** foco em código limpo, leve e escalável.  
2. **Interoperabilidade:** permitir que a plataforma se integre a APIs, dashboards externos e bases de dados.  
3. **Inovação e usabilidade:** entregar uma experiência moderna e interativa, acessível a gestores, turistas e analistas.

---

## 🔍 Evolução da Arquitetura

A versão inicial do projeto tinha foco em notebooks de Machine Learning e geração de relatórios técnicos.

Com a nova arquitetura:
- **Frontend** passou a ser modular (HTML + Tailwind + Chart.js + Leaflet);
- **Backend** tornou-se mais inteligente, com Django/DRF e modelos de IA integrados;
- **APIs** foram estruturadas para comunicação fluida entre as camadas;
- **Relatórios PDF e previsões automáticas** passaram a ser gerados dinamicamente.

Essa mudança foi necessária para transformar o protótipo em uma **plataforma completa de insights turísticos sustentáveis**.

# 🏗️ Arquitetura Atualizada do Projeto — Motor Insights Turismo Angola

O projeto **Motor Insights Turismo Angola** evoluiu de um conjunto de notebooks de análise e previsões para um **ecossistema integrado** de análise, visualização e gestão de dados de turismo sustentável.

## ⚙️ Camadas Principais

### Backend (Núcleo Analítico)
- Framework: **Django** + **Django REST Framework**
- Módulos:
  - `core/` → lógica de IA, previsão e indicadores de sustentabilidade
  - `api/` → endpoints REST para o frontend
  - `ml_engine.py` → motor de predição (Prophet, Scikit-learn)
- Razão: necessário para permitir integração com múltiplos frontends e usuários autenticados, com segurança e escalabilidade.

### Frontend (Dashboard Interativo)
- Framework: **HTML + TailwindCSS + Chart.js + Leaflet**
- Funções:
  - Dashboard principal com KPIs, gráficos e mapa de Angola.
  - Visualização de previsões e tendências sustentáveis.
- Razão: arquitetura modular permite manutenção independente e personalização de cada módulo.

### Relatórios e Exportações
- Biblioteca: **WeasyPrint**
- Permite gerar relatórios PDF com design responsivo, exportando gráficos e métricas diretamente da interface.

### Inteligência Artificial
- Frameworks: **Prophet** e **Scikit-learn**
- Uso: previsão de visitantes, desempenho de sustentabilidade e impacto ambiental.
- Razão: ferramentas maduras, com alta precisão e fácil integração com Django.

## 📈 Fluxo de Dados

[Dataset CSV / API Externa]
        ↓
     ML Engine (Prophet / Sklearn)
        ↓
     Django REST API
        ↓
     Frontend (Chart.js / Leaflet)
        ↓
   Exportação (WeasyPrint PDF)

---

## 🔎 Decisão de Adotar Novas Ferramentas

| Necessidade | Solução Adotada | Benefício |
|--------------|----------------|------------|
| Melhorar visual e usabilidade | TailwindCSS | Layout moderno e acessível |
| Mapa interativo por província | Leaflet.js | Leve e totalmente open source |
| Backend robusto com autenticação | Django | Segurança e escalabilidade |
| Geração de relatórios automáticos | WeasyPrint | Exportação profissional de insights |
| Previsões mais estáveis | Prophet / Sklearn | Modelos de IA facilmente atualizáveis |

---

## 🌍 Sustentabilidade do Código

As novas ferramentas seguem o princípio de **sustentabilidade digital**:
- Baixo consumo de recursos;
- Código reutilizável e bem documentado;
- Compatibilidade com ambientes open-source e de baixo custo (Render, Railway, etc.);
- Alinhamento com os **Objetivos de Desenvolvimento Sustentável (ODS)** na dimensão tecnológica.
