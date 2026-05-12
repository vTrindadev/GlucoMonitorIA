# 🩺 GlucoMonitorIA

### Sistema Inteligente de Monitoramento e Previsão Glicêmica com IA Híbrida

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Gemini API](https://img.shields.io/badge/Gemini%20API-8E75B2?style=for-the-badge&logo=googlebard&logoColor=white)
![Status](https://img.shields.io/badge/Status-Prot%C3%B3tipo%20Funcional-blue?style=for-the-badge)

---

# 🎥 Demonstração do Projeto

**[Assista ao Pitch e Demonstração da Solução](INSERIR_LINK_DO_VIDEO)**

---

# 🚀 Link do Protótipo

**[Abrir Protótipo no Google AI Studio](https://ai.studio/apps/1bbbc2b7-9f78-41e0-82ff-52f7af9cc5f5?fullscreenApplet=true)**

---

# 📌 1. Identificação do Grupo

* **Instituição:** Faculdade Engenheiro Salvador Arena (FESA)
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

Além disso, a solução demonstra a viabilidade da integração entre Inteligência Artificial preditiva, sistemas especialistas e IA generativa em aplicações futuras de Saúde 4.0.

---

# ⚙️ 4. Modelagem PEAS

| Componente | Descrição |
| :--- | :--- |
| **Performance (P)** | Alta precisão na previsão glicêmica, detecção de variações bruscas e geração de alertas confiáveis |
| **Environment (E)** | Dados simulados de glicose ao longo do tempo com eventos associados |
| **Actuators (A)** | Alertas automáticos, classificações de risco e interpretação via IA |
| **Sensors (S)** | Dados glicêmicos, horários e eventos registrados manualmente ou via dataset |

---

# 🧬 5. Arquitetura Lógica e Aprendizado

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

A IA Generativa atua exclusivamente como camada interpretativa e explicativa, não interferindo na lógica determinística do Sistema Especialista.

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
