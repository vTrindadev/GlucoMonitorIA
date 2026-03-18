# GlucoMonitorIA

### 1. Identificação do Grupo
* **Instituição:** FACULDADE ENGENHEIRO SALVADOR ARENA
* **Curso:** ENGENHARIA DE CONTROLE E AUTOMAÇÃO
* **Grupo:** GRUPO B
* **Integrantes:**
    * FELIPE SILVA BERTANI - RA: 062230043
    * MAYCON ALELUIA - RA: 062220038
    * RAFAEL CIRELLI - RA: 062220022
    * VICTOR CÉSAR TRINDADE PEREIRA - RA: 062220012

---

### 2. Área Problema Selecionada
Selecione a trilha tecnológica do projeto (marque com um [x]):
* [X] **Saúde 4.0:** Robótica Assistiva (Controladores Inteligentes/Fuzzy)
* [ ] **Smart Grid:** Eficiência Energética e Descarbonização
* [ ] **Agtech:** Automação de Precisão e Visão Computacional
* [ ] **Logística Autônoma:** Coordenação de AGVs e Otimização de Rotas

---

### 3. Diagnóstico e Definição do Agente
Nesta seção, descrevemos o cenário de atuação e a modelagem do agente inteligente.

* **Contexto:** O sistema está inserido no setor de Saúde Digital (Digital Health) e Dispositivos Médicos Vestíveis, com forte interseção com áreas como Internet das Coisas Médicas (IoMT) e Inteligência Artificial aplicada à medicina. Esse contexto envolve o desenvolvimento de tecnologias para monitoramento contínuo de pacientes, com foco em doenças crônicas como o Diabetes Mellitus. A tendência atual do setor é migrar de métodos invasivos para soluções não invasivas, mais confortáveis e integradas ao cotidiano do usuário.
* **Problema:** O principal gargalo está na ausência de um método confiável, contínuo e totalmente não invasivo para monitoramento da glicose. As soluções atuais, como os sensores subcutâneos (CGMs), ainda apresentam limitações relacionadas ao desconforto, necessidade de substituição periódica e risco de irritação ou infecção. Além disso, medições não invasivas enfrentam desafios técnicos significativos, pois os sinais fisiológicos captados (elétricos ou ópticos) são extremamente sensíveis a ruídos causados por variáveis como temperatura, suor, pressão e movimento.
* **Impacto:** A aplicação de técnicas avançadas de aprendizado de máquina pode transformar esse cenário ao permitir a fusão inteligente de múltiplos sensores e a modelagem de relações não lineares complexas. Como resultado, espera-se alcançar um monitoramento glicêmico contínuo, preciso e totalmente não invasivo, reduzindo significativamente o desconforto do paciente e aumentando a adesão ao tratamento. Isso pode levar à diminuição de complicações associadas ao controle inadequado da glicemia, redução de custos com hospitalizações e melhoria geral na qualidade de vida de pessoas com diabetes. Além disso, abre caminho para sistemas mais avançados.

#### Modelagem PEAS (Agente Inteligente)
| Componente | Descrição |
| :--- | :--- |
| **Performance (P)** | Critérios de sucesso (ex: precisão de acerto, kWh economizados). |
| **Ambiente (E)** | Onde o agente opera (ex: armazém simulado, rede elétrica). |
| **Atuadores (A)** | Como o agente age (ex: acionamento de motores, válvulas). |
| **Sensores (S) ** | Como o agente percebe o ambiente (ex: câmeras, sensores de carga). |

---

### 4. Arquitetura de Dados e IA
Definição das fontes de dados e da inteligência por trás da solução.

* **Origem dos Dados:** [Link para dataset no Kaggle/UCI ou descrição da fonte].
* **Lógica de IA:** [Técnica utilizada: ex: Redes Neurais, Lógica Fuzzy, Busca A*].
* **Justificativa:** Por que essa técnica é ideal para este problema específico?

---

### 5. Plano de Tratamento de Dados (ETL)
O fluxo de processamento dos dados segue estas etapas:
1. **Extração:** Coleta de dados via arquivos [CSV/JSON] ou simulação.
2. **Transformação:** Limpeza de nulos, normalização e engenharia de atributos.
3. **Carga:** Disponibilização dos dados para o treinamento do modelo de IA.

---

### 6. Estrutura do Repositório
Organização simplificada para o Milestone 1:
* `/data`: Arquivos de dados originais (raw) e tratados (processed).
* `/notebooks`: Experimentos iniciais e análise exploratória.
* `/scripts`: Códigos Python (.py) contendo a lógica do agente e do ETL.
* `requirements.txt`: Lista de bibliotecas para rodar o projeto.
* `README.md`: Documentação atual do projeto.

---

### 7. Instruções para Execução
Para reproduzir o ambiente e testar o diagnóstico:
1. Clone este repositório.
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
