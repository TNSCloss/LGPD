---
title: LIA-02 — Teste de Legitimidade: Marketing Direto a Clientes
date: 2026-08-08
tags: [lgpd, lia, art-10, interesse-legitimo, marketing, portfolio, supermercado10]
aliases: [LIA-02, Teste de Legitimidade Marketing, Direct Marketing LIA]
status: approved
version: 1.0
owner: Encarregado de Dados (DPO)
framework: LGPD
related_docs:
  - ../01-ropa-registro-de-atividades/ropa-registro-operacoes
  - lia-1-prevencao-fraude
---

# LIA-02 · Teste de Legitimidade (LIA) — Marketing Direto a Clientes Existentes

> **Enquadramento legal:** Art. 7º, IX + Art. 10, §3º da LGPD. Este LIA cobre o envio de comunicações de marketing (e-mail, SMS, push) **exclusivamente a clientes com relacionamento vigente**. Para **não-clientes** (leads), a base legal é o **consentimento** (Art. 7º, I) — nunca interesse legítimo.

---

## 1. Finalidade Legítima

| Pergunta | Resposta |
|---|---|
| Qual é a finalidade? | Comunicar ofertas, novidades e benefícios do programa "Cliente 10" a clientes que **já possuem cadastro e relacionamento** com a companhia. |
| A finalidade é legítima e específica? | **Sim.** É o interesse legítimo do controlador em fidelizar e informar sua base ativa de clientes (Art. 7º, IX) — prática de mercado, previsível para quem se cadastrou. |
| Existe expectativa razoável? | **Sim.** O cliente que se cadastra no programa ou compra no e-commerce razoavelmente espera receber comunicações institucionais e promocionais da marca, desde que respeitados o opt-out e a frequência. |
| Documentação | RoPA — processo "Marketing — Campanhas de comunicação". |

> **Delimitação crítica:** este LIA **não autoriza** (i) envio a não-clientes, (ii) compra de bases, (iii) telemarketing ativo, nem (iv) perfilamento sensível. Tudo isso exigiria consentimento (Art. 7º, I / Art. 11, I).

---

## 2. Necessidade

| Pergunta | Resposta |
|---|---|
| Os dados são limitados ao necessário? (Art. 6º, III) | **Sim.** Apenas e-mail/telefone/SMS + preferências de contato declaradas. **Nunca** dados de saúde, financeiros ou de terceiros. |
| É possível alcançar a finalidade com menos dados? | **Sim, e já praticado:** segmentação apenas por canal de contato e histórico de compras agregado (pseudonimizado para analytics). |
| Os dados já existem no controlador (sem aquisição externa)? | **Sim.** Base própria de clientes ativos. |
| **Conclusão de necessidade** | **O tratamento é necessário; a base é própria; não há coleta adicional.** |

---

## 3. Balanceamento

### 3.1 Interesse do controlador

- Fidelização e recorrência de compra (custo de aquisição de cliente é 5–7x maior que o de retenção).
- Comunicação institucional (informação de qualidade e segurança alimentar).

### 3.2 Impacto sobre os direitos e liberdades do titular

- **Risco principal:** incômodo, cansaço e perda de controle sobre a comunicação (spam percebido).
- **Risco de perfilamento:** inexistente no escopo (sem decisão automatizada que afete o titular).

### 3.3 Juízo de proporcionalidade

| Fator | Análise |
|---|---|
| Severidade da interferência | **Baixa** — comunicação não invasiva, facilmente ignorável |
| Expectativa razoável do titular | Atendida: cadastro voluntário + transparência na política |
| Benefício esperado | Alto: informação relevante, ofertas, programa de fidelidade |
| Medidas menos intrusivas | Não aplicável — o próprio meio (e-mail/SMS) já é o menos intrusivo |

**RESULTADO DO BALANCEAMENTO: o interesse legítimo PREVALECE para clientes com relacionamento ativo**, **condicionado** ao respeito imediato do opt-out e à transparência. Para não-clientes, o balanceamento seria inverso: **prevalece o direito à privacidade** → base legal passa a ser consentimento.

---

## 4. Salvaguardas

| Salvaguarda | Aplicação |
|---|---|
| **Opt-out em 100% das comunicações** | Link de descadastro em todo e-mail; "SAIR" em SMS; baixa em até 48h — a forma mais crítica de salvaguarda |
| **Gestão central de preferências** | Centro de preferências de contato no app/site |
| **Segmentação sem sensibilidade** | Nunca usa dados sensíveis para segmentar |
| **Frequência controlada** | Máximo de X e-mails/semana por cliente, com monitoramento de reclamação |
| **Transparência (Art. 10, §2º)** | Política de privacidade informa a base legal de interesse legítimo |
| **Canal do titular** | Direito de oposição a qualquer momento (Art. 18) — ver pasta 06 |
| **DPA com operadores** | Contratos com plataformas de e-mail/SMS e agências |
| **Registro do consentimento** | Trilha de auditoria para a base de leads (consentimento) |

---

## 5. Decisão e Monitoramento

**DECISÃO:** utilizar **Art. 7º, IX (interesse legítimo)** para marketing direto **apenas a clientes com relacionamento ativo**, com opt-out imediato e sem segmentação sensível.

- [x] LIA revisado em 08/08/2026
- [ ] Revisar quando: reclamações ao canal do titular, mudança de segmentação, incidente, guia ANPD ou revisão anual (08/08/2027)

**Indicadores de monitoramento:** taxa de descadastro (>5% no trimestre → revisar frequência), reclamações no canal do titular, taxa de entrega.

> **Nota de accountability:** este LIA está disponível para auditoria e para a ANPD (Art. 10, §3º). Não constitui aconselhamento jurídico.
