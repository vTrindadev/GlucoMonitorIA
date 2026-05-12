# 🩺 GlucoMonitorIA

### Sistema Inteligente de Monitoramento e Previsão Glicêmica com IA Híbrida

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Gemini API](https://img.shields.io/badge/Gemini%20API-8E75B2?style=for-the-badge&logo=googlebard&logoColor=white)
![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-success?style=for-the-badge)

---

### 🎥 Demonstração do Projeto
**[Assista ao Pitch e Demonstração da Solução](INSERIR_LINK_DO_VIDEO)**

### 🚀 Link do Protótipo
**[Abrir Protótipo no Google AI Studio](INSERIR_LINK_DO_PROTOTIPO)**

---

# 📌 1. Identificação do Grupo

* **Instituição:** Faculdade Engenheiro Salvador Arena (FSA)
* **Curso:** Engenharia de Controle e Automação
* **Grupo:** Grupo B

## 👨‍💻 Integrantes

| Nome | RA |
|---|---|
| Felipe Silva Bertani | 062230043 |
| Maycon Alves | 062220038 |
| Rafael Cirelli | 062220022 |
| Victor César Trindade Pereira | 062220012 |

---

# 🏥 2. Área Problema Selecionada

* [X] **Saúde 4.0:** Robótica Assistiva (Controladores Inteligentes / IA)
* [ ] Smart Grid: Eficiência Energética e Descarbonização
* [ ] Agtech: Automação de Precisão e Visão Computacional
* [ ] Logística Autônoma: Coordenação de AGVs e Otimização de Rotas

---

# 🧠 3. Diagnóstico e Definição do Agente

## Contexto

O GlucoMonitorIA está inserido no contexto de Saúde Digital (Digital Health), utilizando Inteligência Artificial para monitoramento, análise e previsão glicêmica. O sistema simula um cenário real de engenharia aplicada à saúde, permitindo transformar dados fisiológicos em informações úteis para suporte à decisão.

A solução possui potencial aplicação futura em dispositivos não invasivos de monitoramento contínuo, alinhando automação, IA e sistemas inteligentes voltados à Saúde 4.0.

---

## Problema

Pacientes e sistemas de monitoramento enfrentam dificuldades na interpretação de dados glicêmicos ao longo do tempo, principalmente devido às rápidas variações causadas por alimentação, atividade física, repouso e outros eventos fisiológicos.

Essas oscilações podem gerar riscos de:
- Hipoglicemia
- Hiperglicemia
- Decisões inadequadas no acompanhamento glicêmico

---

## Impacto

O uso de um agente inteligente permite:
- Detectar tendências glicêmicas
- Gerar alertas automáticos
- Interpretar padrões complexos
- Melhorar o suporte à decisão
- Simular aplicações reais de IA na saúde

O sistema transforma dados brutos em informações interpretáveis e explicáveis, aumentando a confiabilidade da análise.

---

# ⚙️ Modelagem PEAS

| Componente | Descrição |
| :--- | :--- |
| **Performance (P)** | Alta precisão na previsão glicêmica, detecção de variações bruscas e geração de alertas confiáveis |
| **Environment (E)** | Dados simulados de glicose ao longo do tempo com eventos associados |
| **Actuators (A)** | Alertas automáticos, classificações de risco e interpretação via IA |
| **Sensors (S)** | Dados glicêmicos, horários e eventos registrados manualmente ou via dataset |

---

# 🧬 4. Arquitetura Lógica e Aprendizado

O **GlucoMonitorIA** utiliza uma arquitetura híbrida dividida em três camadas principais:

---

## 🔹 1. Módulo Preditivo — Rede Neural Artificial (RNA)

O sistema utiliza uma **Rede Neural Artificial do tipo MLPRegressor** para prever a próxima glicose do usuário com base em dados históricos.

A RNA aprende padrões glicêmicos e tendências temporais, permitindo antecipar possíveis alterações futuras.

---

## 🔹 2. Módulo de Controle — Sistema Especialista

Após a previsão da RNA, um Sistema Especialista baseado em regras determinísticas realiza a classificação do risco glicêmico.

Exemplo:
- Glicose abaixo de 70 mg/dL → Hipoglicemia
- Glicose acima de 180 mg/dL → Hiperglicemia

Essa camada garante confiabilidade técnica e rastreabilidade das decisões.

---

## 🔹 3. Camada Interpretativa — Gemini API

A API do Gemini atua como camada interpretativa.

Sua função é:
- Explicar os resultados
- Traduzir informações técnicas
- Gerar feedback humanizado
- Auxiliar na interpretação dos dados

Importante:
A IA Generativa NÃO interfere na lógica de decisão do sistema.

---

# 🏗️ Arquitetura do Sistema

```text
Entrada de Dados
        ↓
Pré-processamento (ETL)
        ↓
Rede Neural Artificial
        ↓
Previsão da Próxima Glicose
        ↓
Sistema Especialista
(Classificação de Risco)
        ↓
Gemini API
(Interpretação Inteligente)
        ↓
Alertas e Recomendações
```

---

# 🤖 5. Justificativa da Abordagem

A abordagem escolhida para o núcleo inteligente do projeto foi a utilização de **Redes Neurais Artificiais (RNA)**.

## Por que essa abordagem foi escolhida?

### 🔹 Natureza do Problema

A previsão glicêmica envolve padrões não lineares e múltiplas variáveis fisiológicas, tornando métodos tradicionais menos eficientes para capturar tendências complexas.

---

### 🔹 Capacidade de Generalização

A RNA possui alta capacidade de aprendizado com dados históricos, identificando relações complexas entre:
- Variação glicêmica
- Eventos fisiológicos
- Tendências temporais

---

### 🔹 Escalabilidade

A arquitetura permite integração futura com:
- Sensores reais
- Dispositivos IoT
- Aplicações mobile
- Monitoramento em tempo real

---

# 🔄 6. Pipeline ETL

## Extração
- Importação de datasets
- Inserção manual de dados

## Transformação
- Limpeza de dados
- Tratamento de inconsistências
- Cálculo de variação glicêmica (`diff`)
- Estruturação dos dados

## Carga
- Preparação para treinamento e inferência da IA

---

# 📊 7. Evidências Visuais e Desempenho

## 📉 Curva de Loss da Rede Neural

O gráfico abaixo demonstra a redução do erro da RNA durante o treinamento.

<img width="859" height="472" alt="image" src="https://github.com/user-attachments/assets/4d0ad3ea-bc24-4cfd-a02e-71dc01df70c6" />

---

## 📈 Métricas Obtidas

| Métrica | Resultado |
|---|---|
| MAE Médio | 8.85 |
| RMSE Médio | 11.75 |
| R² Médio | 0.90 |

Os resultados demonstram boa capacidade preditiva do modelo em dados simulados.

---

# 🛠️ 8. Tecnologias Utilizadas

| Tecnologia | Função |
|---|---|
| Python | Linguagem principal |
| Pandas | Manipulação de dados |
| NumPy | Operações matemáticas |
| Scikit-Learn | Machine Learning |
| MLPRegressor | Rede Neural Artificial |
| Google Gemini API | IA Generativa |
| Matplotlib | Visualização de dados |
| Google Colab | Ambiente de desenvolvimento |

---

# 📂 9. Estrutura do Repositório

```text
📦 GlucoMonitorIA
 ┣ 📂 assets/images
 ┣ 📂 data
 ┣ 📂 notebooks
 ┣ 📂 scripts
 ┣ 📄 requirements.txt
 ┣ 📄 README.md
```

---

# ▶️ 10. Instruções para Execução

## 1. Clone o repositório

```bash
git clone URL_DO_REPOSITORIO
```

## 2. Acesse a pasta do projeto

```bash
cd GlucoMonitorIA
```

## 3. Instale as dependências

```bash
pip install -r requirements.txt
```

## 4. Abra o notebook principal

Execute os arquivos `.ipynb` utilizando:
- Google Colab
- Jupyter Notebook

---

## ⚠️ Configuração da API Gemini

Insira sua `GOOGLE_API_KEY` na célula de configuração da API para habilitar a camada interpretativa.

---

# 🚀 11. Futuras Implementações

- Dashboard Web/Mobile
- Cadastro individual de usuários
- Histórico inteligente
- Alertas em tempo real
- Integração com sensores físicos
- Integração IoT
- Dispositivo não invasivo
- Explicabilidade avançada (XAI)

---

# 🤖 12. Apêndice de IA

## Ferramentas Utilizadas
- Gemini
- ChatGPT

## Aplicação da IA
As ferramentas de IA generativa auxiliaram em:
- Estruturação do código
- Organização do pipeline
- Revisão textual
- Sugestão de métricas
- Desenvolvimento da arquitetura do sistema

## Validação
Todos os resultados e métricas foram analisados e validados tecnicamente pelo grupo.

---

# 📚 Instituição

Faculdade Engenheiro Salvador Arena  
Engenharia de Controle e Automação  
Projeto de Inteligência Artificial — 2026

---
© 2026 — GlucoMonitorIA
