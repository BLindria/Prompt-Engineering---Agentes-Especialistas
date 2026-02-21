# Prompt-Engineering---Agentes-Especialistas
Este diretório contém os System Prompts (instruções de sistema) utilizados para configurar cada agente no n8n. A técnica principal aplicada aqui é o Structured Prompting, visando precisão técnica e redução de alucinações.

Técnicas Aplicadas:
Context Injection (RAG): Instruções que orientam o agente a priorizar dados recuperados do Google Sheets (SLA) antes de qualquer conhecimento prévio.
Role-Playing: Definição clara de persona para cada agente (Master, Especialista SQL, etc.), garantindo que o tom de voz e o vocabulário técnico sejam adequados ao suporte do ERP WinThor.
Zero-Shot Extraction: Capacidade do Agente Master de identificar e extrair números de rotinas sem necessidade de exemplos prévios no prompt.
Output Formatting: Uso de Markdown para que o bot retorne checklists legíveis com Bullet Points e negrito, facilitando o trabalho do analista de suporte.

Arquivos:
Master_Router.md: Lógica de decisão para roteamento de chamados.
Especialista_SLA.md: Protocolo de diagnóstico e consulta à base de checklists.
Especialista_SQL.md: Regras de ouro para geração de scripts Oracle.
Especialista_Duvidas.md: Integração com busca semântica para processos de negócio.
