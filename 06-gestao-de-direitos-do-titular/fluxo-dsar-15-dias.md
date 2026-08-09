---
title: Fluxo de Atendimento de Requisições do Titular (DSAR — 15 dias)
date: 2026-08-08
tags: [lgpd, dsar, direitos, art-18, fluxo, portfolio, supermercado10]
aliases: [Fluxo DSAR, Fluxo de Direitos do Titular, Data Subject Request]
status: approved
version: 1.0
owner: Encarregado de Dados (DPO)
framework: LGPD
related_docs:
  - formulario-requisicao-titular
  - templates-resposta-direitos
  - matriz-validacao-identidade
---

# Fluxo de Atendimento de Requisições do Titular (DSAR)

> **Base legal:** Art. 18 da LGPD. **Prazo de resposta:** **15 dias** (prazo indicado pela ANPD). Requisições são gratuitas e não podem ser condicionadas a pagamento (Art. 18, §2º).

## Tempos do fluxo (SLA interno)

| Etapa | SLA interno |
|---|---|
| T0 — Recebimento + registro | mesmo dia |
| T0 + 1 dia | Validação de identidade |
| T0 + 3 dias | Localização dos dados (varredura nos sistemas) |
| T0 + 7 dias | Decisão jurídica (aplicabilidade/exceções) |
| T0 + 10 dias | Redação e revisão da resposta |
| T0 + **15 dias** | **Entrega da resposta ao titular** (dentro do prazo da ANPD) |

```mermaid
flowchart TD
    A([TITULAR faz requisição<br/>formulário no site / e-mail / SAC]) --> B[T0: REGISTRO no sistema DSAR<br/>DPO atribui nº de protocolo<br/>confirma recebimento ao titular]
    B --> C[T0+1d: VALIDAÇÃO DE IDENTIDADE<br/>ver matriz-validacao-identidade]
    C --> D{Identidade validada?}
    D -->|Não| E[T0+3d: pedir documentos adicionais<br/>suspende prazo até resposta]
    D -->|Sim| F[T0+3d: LOCALIZAÇÃO dos dados<br/>varredura em CRM, ERP, RH, logs,<br/>operadores (via DPA)]
    F --> G[T0+7d: ANÁLISE JURÍDICA<br/>verificar exceções Art.18 §3º/§4º<br/>e obrigação legal de conservação]
    G --> H[T0+10d: REDAÇÃO da resposta<br/>template por direito<br/>ver templates-resposta-direitos]
    H --> I[T0+15d: ENTREGA ao titular<br/>meio seguro e confidencial]
    I --> J[REGISTRO final no DSAR<br/>+ monitoramento de satisfação]
    J --> K([FIM])
    C --> L[Titular identificado é o<br/>próprio solicitante?<br/>representante legal?]
    L --> C
```

## Decisões de negócio

| Situação | Ação |
|---|---|
| Requisição de **acesso** | Enviar relatório completo de dados em formato legível (Art. 19, II) |
| **Exclusão** (Art. 18, IV e VI) | Eliminar em todos os sistemas, salvo obrigação legal de conservação (Art. 16) |
| **Portabilidade** (Art. 18, V) | Fornecer em formato estruturado e interoperável (CSV/JSON) |
| Dado **anônimo ou fora do escopo** (Art. 18, §4º) | Informar que não se aplica, com justificativa |
| **Exceção legal** (Art. 18, §3º) — ex.: obrigação de conservar | Responder negando com fundamento e indicando o prazo de conservação |
| Solicitação **abusiva/repetitiva** (Art. 18, §5º) | Documentar e recusar com justificativa; sem cobrança automática |

## Trilha de auditoria (Art. 6º, IX)

Cada requisição gera um registro com: protocolo, titular, direito solicitado, canais, validação de identidade, sistemas consultados, resposta enviada, prazo cumprido e tratativa de exceção. Retenção: **5 anos**.

## Quem responde

| Papel | Responsabilidade |
|---|---|
| **Encarregado (DPO)** | Centraliza o atendimento, valida identidade e qualidade, responde ao titular |
| **SAC / Lojas** | Recebem requisições e encaminham ao DPO no mesmo dia |
| **Data Owners (RH, Marketing, Finanças, TI)** | Localizam os dados e executam correção/exclusão/portabilidade |
| **Operadores** | Executam a requisição conforme o **DPA** (contrato — pasta 07), com SLA de 10 dias |

## Métricas do processo (KPIs)

- % de requisições respondidas **dentro de 15 dias** (meta ≥ 95%)
- Tempo médio de resposta (meta ≤ 8 dias)
- Requisições por tipo de direito (acesso/exclusão/correção/portabilidade)
- % de requisições resolvidas integralmente

> **Ferramentas:** este fluxo integra o [[formulario-requisicao-titular|Formulário de Requisição]], os [[templates-resposta-direitos|templates de resposta]] e a [[matriz-validacao-identidade|matriz de validação de identidade]].
