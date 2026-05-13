# 🩺 GlucoMonitorIA

### Sistema Inteligente de Monitoramento e Previsão Glicêmica com IA Híbrida

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Gemini API](https://img.shields.io/badge/Gemini%20API-8E75B2?style=for-the-badge&logo=googlebard&logoColor=white)
![Status](https://img.shields.io/badge/Status-Prot%C3%B3tipo%20Funcional-blue?style=for-the-badge)

---
# 📌 1. Identificação do Grupo

- **Instituição:** Faculdade Engenheiro Salvador Arena (FESA)
- **Curso:** Engenharia de Controle e Automação
- **Grupo:** Grupo B

## 👨‍💻 Integrantes

| Nome | RA | LinkedIn
|---|---|---|
| Felipe Silva Bertani | 062230043 | xxx |
| Maycon Alves | 062220038 | xxx |
| Rafael Cirelli | 062220022 | xxx |
| Victor César Trindade Pereira | 062220012 | xxx |

---

# 🎥 Demonstração do Projeto

**[Assista ao Pitch e Demonstração da Solução](https://youtu.be/O3UhvLzB4JM?si=Ws_bcqc0UH3HcbHy)**

---

# 🚀 Link do Protótipo

**[Abrir Protótipo no Google AI Studio](https://ai.studio/apps/1bbbc2b7-9f78-41e0-82ff-52f7af9cc5f5?fullscreenApplet=true)**

---

# 🏥 2. Área Problema Selecionada

- [X] **Saúde 4.0:** Robótica Assistiva (Controladores Inteligentes / IA)
- [ ] Smart Grid: Eficiência Energética e Descarbonização
- [ ] Agtech: Automação de Precisão e Visão Computacional
- [ ] Logística Autônoma: Coordenação de AGVs e Otimização de Rotas

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

O **GlucoMonitorIA** utiliza uma arquitetura híbrida dividida em três camadas principais.

---

## 🔹 1. Módulo Preditivo — Rede Neural Artificial (RNA)

O sistema utiliza uma **Rede Neural Artificial do tipo MLPRegressor** para prever a próxima glicose do usuário com base em dados históricos.

A RNA aprende padrões glicêmicos e tendências temporais, permitindo antecipar possíveis alterações futuras.

---

## 🔹 2. Módulo de Controle — Sistema Especialista

Após a previsão da RNA, um Sistema Especialista baseado em regras determinísticas realiza a classificação do risco glicêmico.

### Exemplos:

- Glicose abaixo de 70 mg/dL → Hipoglicemia
- Glicose acima de 180 mg/dL → Hiperglicemia

Essa camada garante confiabilidade técnica e rastreabilidade das decisões.

---

## 🔹 3. Camada Interpretativa — Gemini API

A API do Gemini atua como camada interpretativa.

### Funções da IA Generativa:

- Explicar os resultados
- Traduzir informações técnicas
- Gerar feedback humanizado
- Auxiliar na interpretação dos dados

> A IA Generativa atua exclusivamente como camada interpretativa e explicativa, não interferindo na lógica determinística do Sistema Especialista.

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

# 🤖 6. Justificativa da Abordagem

A abordagem escolhida para o núcleo inteligente do projeto foi a utilização de **Redes Neurais Artificiais (RNA)**.

## 🔹 Natureza do Problema

A previsão glicêmica envolve padrões não lineares e múltiplas variáveis fisiológicas, tornando métodos tradicionais menos eficientes para capturar tendências complexas.

---

## 🔹 Capacidade de Generalização

A RNA possui alta capacidade de aprendizado com dados históricos, identificando relações complexas entre:

- Variação glicêmica
- Eventos fisiológicos
- Tendências temporais

---

## 🔹 Escalabilidade

A arquitetura permite integração futura com:

- Sensores reais
- Dispositivos IoT
- Aplicações mobile
- Monitoramento em tempo real

---

# 🔄 7. Pipeline ETL

## Extração

- Coleta de leituras glicêmicas
- Registro de horários e eventos fisiológicos
- Entrada manual de dados para monitoramento

## Transformação

- Limpeza de dados
- Tratamento de inconsistências
- Cálculo de variação glicêmica (`diff`)
- Estruturação dos dados para aprendizado da RNA

## Carga

- Preparação dos dados para treinamento
- Normalização das variáveis
- Envio das entradas para inferência da IA

---

# 📊 8. Evidências Visuais e Desempenho

## 📉 Curva de Aprendizado da Rede Neural

O gráfico abaixo demonstra a redução do erro da RNA durante o treinamento.

<img width="868" height="472" alt="image" src="https://github.com/user-attachments/assets/db21bb84-d475-41f2-ac13-1a7948eeea8e" />

---

## 🤖 Pipeline Final Integrado

<img width="1795" height="730" alt="image" src="https://github.com/user-attachments/assets/7c8515fa-301e-4d8a-9589-4a60cc43302e" />

O pipeline executa automaticamente:

- leitura dos dados;
- previsão da RNA;
- classificação do sistema especialista;
- interpretação via Gemini;
- geração de alertas simulados.

---

# 📈 Métricas Obtidas

Para validação do modelo, foi aplicada a técnica de validação cruzada K-Fold com k=5, permitindo avaliar a estabilidade e a capacidade de generalização da Rede Neural Artificial em diferentes divisões dos dados.

## Resultados médios obtidos:

- **MAE médio:** 10.36 → representa o erro médio absoluto entre o valor previsto e o valor real da glicose.
- **RMSE médio:** 12.57 → mede o erro quadrático médio, penalizando erros maiores.
- **R² médio:** 0.89 → indica que o modelo conseguiu explicar aproximadamente 89% da variação dos dados.

## Desvio padrão:

- **MAE std:** 0.61
- **RMSE std:** 0.66
- **R² std:** 0.02

Os baixos valores de desvio padrão indicam comportamento consistente entre diferentes execuções da validação cruzada.

Dessa forma, o modelo pode ser considerado robusto e adequado para prever tendências glicêmicas em cenários simulados de monitoramento inteligente.

---

# 🛠️ 9. Tecnologias Utilizadas

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

# 📂 10. Estrutura do Repositório

```text
📦 GlucoMonitorIA
 ┣ 📂 assets
 ┃ ┗ 📂 images
 ┣ 📂 data
 ┣ 📂 notebooks
 ┣ 📂 scripts
 ┣ 📄 requirements.txt
 ┣ 📄 README.md
```

---

# ▶️ 11. Instruções para Execução

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

# ✅ 12. Refinamento e Validação Final

Nesta etapa, o sistema foi refinado para garantir integração completa entre todas as camadas da solução.

O pipeline final executa automaticamente:

```text
Leitura dos Dados → Rede Neural → Sistema Especialista → Gemini API → Alertas Simulados
```

## Funcionalidades implementadas

- Integração completa entre os módulos
- Tratamento de exceções com `try/except`
- Validação de dados de entrada
- Pipeline automatizado
- Organização do código em blocos funcionais
- Simulação de acionamento de atuadores
- Estruturação do repositório para entrega no GitHub

## Validação

O sistema foi validado utilizando:

- divisão treino/teste;
- validação cruzada K-Fold;
- análise da curva de loss;
- métricas MAE, RMSE e R².

Os resultados demonstraram comportamento estável e boa capacidade de generalização da RNA.

---

# 🚀 13. Futuras Implementações

- Dashboard Web/Mobile
- Cadastro individual de usuários
- Histórico inteligente
- Alertas em tempo real
- Integração com sensores físicos
- Integração IoT
- Dispositivo não invasivo
- Explicabilidade avançada (XAI)

---

# 🤖 14. Apêndice de IA

## Ferramentas Utilizadas

- Gemini
- ChatGPT
- Claude

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
