# GlucoMonitorIA

### 1. Identificação do Grupo
* **Instituição:** FACULDADE ENGENHEIRO SALVADOR ARENA  
* **Curso:** ENGENHARIA DE CONTROLE E AUTOMAÇÃO  
* **Grupo:** GRUPO B  
* **Integrantes:**
    * FELIPE SILVA BERTANI - RA: 062230043  
    * MAYCON ALVES - RA: 062220038  
    * RAFAEL CIRELLI - RA: 062220022  
    * VICTOR CÉSAR TRINDADE PEREIRA - RA: 062220012  

---

### 2. Área Problema Selecionada
* [X] **Saúde 4.0:** Robótica Assistiva (Controladores Inteligentes / IA)
* [ ] **Smart Grid:** Eficiência Energética e Descarbonização  
* [ ] **Agtech:** Automação de Precisão e Visão Computacional  
* [ ] **Logística Autônoma:** Coordenação de AGVs e Otimização de Rotas  

---

### 3. Diagnóstico e Definição do Agente

* **Contexto:**  
O sistema está inserido no setor de Saúde Digital (Digital Health), com foco em monitoramento inteligente de glicose. A solução simula um cenário real de engenharia onde dados fisiológicos são analisados para suporte à decisão, com potencial aplicação futura em dispositivos não invasivos.

* **Problema:**  
A dificuldade está em interpretar corretamente dados de glicose ao longo do tempo, considerando variações, eventos (refeição, atividade física) e mudanças rápidas, que podem gerar riscos como hipo ou hiperglicemia.

* **Impacto:**  
A utilização de um agente inteligente permite transformar dados brutos em informações úteis, gerando alertas e suporte à decisão. Isso reduz riscos, melhora o acompanhamento e simula aplicações reais em sistemas de automação na área da saúde.

---

### Modelagem PEAS (Agente Inteligente)

| Componente | Descrição |
| :--- | :--- |
| **Performance (P)** | Alta precisão na classificação do estado glicêmico; detecção de variações bruscas; geração de alertas confiáveis; rastreabilidade das decisões. |
| **Ambiente (E)** | Dados simulados de glicose ao longo do tempo, com eventos associados (alimentação, atividade, repouso). |
| **Atuadores (A)** | Geração de alertas e recomendações via sistema; saída interpretativa por IA. |
| **Sensores (S)** | Dados de glicose, horário e eventos inseridos manualmente ou via dataset. |

---

### 4. Arquitetura de Dados e IA

* **Origem dos Dados:**  
https://www.kaggle.com/datasets/imtkaggleteam/diabetes  

* **Lógica de IA:**  
O sistema utiliza uma abordagem híbrida:
- Sistema Especialista (regras SE/ENTÃO) para classificação determinística  
- Análise heurística baseada em variação de glicose  
- IA Generativa (Gemini) para interpretação dos resultados  

* **Justificativa:**  
A separação entre decisão técnica e interpretação garante maior confiabilidade. O sistema especialista realiza o cálculo de forma determinística, enquanto a IA generativa atua como camada interpretativa, agregando contexto e insights sem interferir na lógica de controle.

---

### 5. Plano de Tratamento de Dados (ETL)

1. **Extração:** Dados carregados via dataset ou inserção manual  
2. **Transformação:** Limpeza, cálculo de variação (`diff`) e estruturação dos dados  
3. **Carga:** Dados preparados para análise pelo sistema especialista  

---

### 6. Estrutura do Repositório

* `/data`: Dados brutos e tratados  
* `/notebooks`: Análise exploratória e testes  
* `requirements.txt`: Dependências do projeto  
* `README.md`: Documentação  

---

### 7. Instruções para Execução

1. Clone o repositório  
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
