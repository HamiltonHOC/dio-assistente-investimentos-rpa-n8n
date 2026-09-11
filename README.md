#  Assistente de Investimentos com RPA e IA Generativa (n8n + Python)
Projeto desenvolvido como entrega final do Bootcamp **Santander 2026 - Automação com n8n** na [DIO](https://dio.me).
---
##  Objetivo do Projeto
Construir um pipeline de automação e RPA que:
1. **Coleta dados de clientes** de uma página web simulando um ambiente corporativo/financeiro via Python.
2. **Processa e orquestra as informações** através de um workflow completo no **n8n**.
3. **Cruza os perfis de investidores** (Conservador, Moderado e Arrojado) com uma base de produtos financeiros.
4. **Gera mensagens e recomendações personalizadas** com auxílio de Inteligência Artificial Generativa.
---
##  Arquitetura da Solução
```text
[ Página Web de Clientes ] 
            │
            ▼ (Web Scraping com Python)
     [ Script RPA ]
            │
            ▼ (Disparo via Webhook HTTP POST)
    [ Workflow no n8n ]
            │
     ┌──────┴──────────────────────────┐
     ▼                                 ▼
[ Base de Investimentos (CSV) ]   [ Agente de IA / LLM ]
     │                                 │
     └──────────────┬──────────────────┘
                    ▼
      [ Mensagens Personalizadas ]
⚙️ Componentes do Sistema
RPA com Python (BeautifulSoup e Requests):

Extrai automaticamente a lista de clientes, saldos e perfis de investidor de páginas HTML.
Converte os dados em formato JSON estruturado e envia diretamente para o n8n através de um Webhook.
Orquestração no n8n:

Webhook Trigger: Escuta os eventos e inicia a automação em tempo real.
Tratamento de Dados: Filtra os clientes e cruza cada perfil com as melhores opções da carteira de investimentos.
Integração com IA: Envia o contexto do cliente para o modelo de linguagem gerar uma consultoria personalizada.
Geração de Valor:

Produção automática de relatórios e mensagens consultivas sem necessidade de intervenção humana manual.
 Tecnologias Utilizadas
n8n: Orquestrador de fluxos low-code/no-code.
Python: Automação de extração (RPA / Web Scraping).
IA Generativa (LLMs): Personalização e geração inteligente de comunicação.
GitHub: Documentação, versionamento e entrega do projeto.

Desenvolvido por Hamilton Castro
Estudante de Produção Criativa com IA & Participante do Bootcamp Santander 2026 (DIO)



