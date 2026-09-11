# 🤖 Assistente de Investimentos com RPA e IA Generativa (n8n + Python)

Projeto desenvolvido como entrega final do Bootcamp **Santander 2026 - Automação com n8n** na [DIO](https://dio.me).

---

## 🎯 Objetivo do Projeto
Construir uma solução completa de automação e Robotic Process Automation (RPA) combinando **Python** para raspagem/coleta de indicadores financeiros e o **n8n** como orquestrador do fluxo, integrando com Modelos de Linguagem (IA Generativa) para análise preditiva e geração de relatórios automatizados por e-mail/notificação.

---

## 🏗️ Arquitetura da Solução

O fluxo de automação é composto por quatro etapas integradas:

```text
[ Script Python / Web Scraping ] 
               │
               ▼ (Payload JSON via Webhook)
      [ n8n Workflow ]
               │
               ▼ (Prompt estruturado)
     [ IA Generativa (LLM) ]
               │
               ▼ (Resumo Executivo & Recomendações)
[ Disparo de E-mail / Relatório ]
