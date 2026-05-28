# Mission Control AI - Projeto Hélios

**Integrantes:**
* Cristhian Henrique  Clementino - RM: 574117
* Diego de Oliveira Brandão - RM: 569773

## Descrição do Projeto
Sistema de monitoramento conversacional para missão espacial. Utiliza inteligência artificial para analisar dados simulados de telemetria (temperatura, energia e comunicação). O sistema conta com uma camada lógica de verificação em código que emite alertas autônomos quando os parâmetros entram em situação crítica, integrando esses dados ao contexto da IA para emissão de diretrizes técnicas seguras.

## Tecnologias Utilizadas
* **Linguagem:** Python
* **Ambiente:** Google Colab
* **Inteligência Artificial:** API da OpenAI (Modelo: gpt-4o-mini)
* **Bibliotecas:** `random`, `os`, `google.colab.userdata`, `openai`

## Demonstração

**1. Status Operacional Normal** Causado pela geração aleatória de parâmetros de telemetria dentro dos limites de segurança (ex: Temperatura a 50°C, Energia a 80%, Comunicação estável). A camada lógica do Python atesta a normalidade antes de qualquer input.  
![Dados da missão normais](assets/print1_normal.png)

**2. Alerta Crítico do Sistema** Causado pela geração de parâmetros operacionais em estado de risco (ex: Temperatura > 85°C ou Energia < 20%). O código intercepta o desvio e exibe avisos automáticos de falha no terminal.  
![Alerta crítico do sistema](assets/print2_alerta.png)

**3. Diagnóstico e Resposta da IA** Causado pela inserção de um comando do usuário solicitando o status das falhas detectadas. A IA processa o *system prompt* em conjunto com a telemetria atual e fornece recomendações técnicas para mitigação.  
![Resposta e análise da IA 1](assets/print3_ia_resposta.png)

**4. Retenção de Contexto (Conversa Contínua)** Causado pelo envio de uma pergunta de seguimento em relação à resposta anterior (ex: "Detalhe a primeira recomendação"). Demonstra a retenção do histórico do terminal e a capacidade da IA de manter o contexto da missão sem precisar receber os dados novamente.  
![Resposta e análise da IA 2](assets/print4_ia_conversa.png)

## Como Executar
O sistema foi projetado para rodar no Google Colab.

1. Acesse o Notebook: [Colab](https://colab.research.google.com/drive/1-58xQpilfYQpavSF1xEUkRroNlVKkhtk?usp=sharing)
2. Execute todas as células em ordem. 
3. O terminal interativo será iniciado no output da última célula. Para encerrar, digite 'sair'.

## Vídeo de Demonstração
[Assistir ao vídeo](Link do YouTube aqui)
