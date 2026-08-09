---
title: Modelo de Registro de Incidente de Segurança (LGPD Art. 48)
date: 2026-08-08
tags: [lgpd, incidente, art-48, modelo, registro, portfolio, supermercado10]
aliases: [Registro de Incidente, Modelo de Registro de Incidente]
status: approved
version: 1.0
owner: Encarregado de Dados (DPO)
framework: LGPD
related_docs:
  - playbook-resposta-incidente
  - modelo-comunicacao-anpd-titulares
---

# Modelo de Registro de Incidente

> Preencher **um arquivo por incidente**, a partir da detecção (T0). Revisar ao longo de todo o ciclo. Arquivo: `registro-INCIDENTE-XXXX.md`. Retenção: **5 anos** (accountability — Art. 6º, IX).

---

## 1. Identificação do incidente

| Campo | Preenchimento |
|---|---|
| Nº do incidente | INC-2026-001 |
| Data/hora de detecção (T0) |  |
| Como foi detectado |  (pessoa/sistema/terceiro — descrever) |
| Quem detectou |  |
| Severidade inicial | [ ] CRÍTICA [ ] ALTA [ ] MÉDIA [ ] BAIXA |
| Enquadramento final | [ ] Incidente de segurança com dados pessoais [ ] Operacional |

## 2. Descrição do incidente

**O que aconteceu (relato cronológico):**

```

```

**Sistemas/processos afetados:**

**Causa provável (hipótese inicial):**

## 3. Dados pessoais envolvidos

| Categoria de dados | Sensível? (Art. 5º, II) | Volume estimado (titulares) | Fonte |
|---|---|---|---|
|  |  |  |  |

**Exemplos:** nome/CPF/e-mail · dados financeiros (PAN) · biométricos · saúde · credenciais.

## 4. Linha do tempo da resposta

| Data/Hora | Ação | Responsável |
|---|---|---|
| T0 + | Comunicação ao CISO/DPO | |
| T0 + | Contenção (isolar/revoGar acessos) | |
| T0 + | Preservação de evidências | |
| T0 + | Avaliação de risco aos titulares | |
| T0 + | Decisão de notificação (sim/não + motivo) | |
| T0 + | Notificação ANPD (preliminar) | |
| T0 + | Notificação aos titulares | |
| T0 + | Comunicação complementar ANPD | |
| T0 + | Encerramento | |

## 5. Avaliação de risco aos titulares (Art. 48)

| Fator | Resposta |
|---|---|
| Dados sensíveis? |  |
| Dados criptografados? (chave segura?) |  |
| Nº de titulares afetados |  |
| Há evidência de acesso/uso indevido? |  |
| Consequências prováveis |  |
| **Risco relevante?** | [ ] SIM — notificar ANPD/titulares [ ] NÃO — justificar: |

## 6. Notificação à ANPD

| Campo | Valor |
|---|---|
| Notificação necessária? | [ ] Sim [ ] Não |
| Protocolo preliminar (plataforma ANPD) |  |
| Data da preliminar (≤ 3 dias úteis) |  |
| Protocolo complementar |  |
| Data da complementar (≤ 20 dias úteis) |  |
| Resumo do que foi comunicado |  |

## 7. Notificação aos titulares

| Campo | Valor |
|---|---|
| Titulares notificados? | [ ] Sim [ ] Não (justificar) |
| Meio de comunicação |  |
| Nº de titulares alcançados |  |
| Cópia da comunicação | anexar |

## 8. Remediação e causa raiz

**Causa raiz confirmada:**

**Ações corretivas:** (listar e responsabilizar)

**Controles adicionados/reforçados:**

## 9. Encerramento

| Campo | Preenchimento |
|---|---|
| Data de encerramento |  |
| Parecer do Encarregado (DPO) |  |
| Aprovado por |  |
| Lições aprendidas (arquivo próprio) |  |
| RoPA/RIPD atualizado? | [ ] Sim [ ] Não |
| Anexos | evidências, comunicações, relatório forense |

---

> **Uso:** este modelo integra o [[playbook-resposta-incidente|Playbook]] e o [[fluxograma-resposta-incidente|fluxograma]]. A comunicação oficial deve usar o [[modelo-comunicacao-anpd-titulares|Modelo de Comunicação à ANPD e Titulares]].
