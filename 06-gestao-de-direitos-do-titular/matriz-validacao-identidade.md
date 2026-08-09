---
title: Matriz de Validação de Identidade (DSAR — sem criar novo risco)
date: 2026-08-08
tags: [lgpd, dsar, identidade, validacao, art-18, portfolio, supermercado10]
aliases: [Matriz de Validação de Identidade]
status: approved
version: 1.0
owner: Encarregado de Dados (DPO)
framework: LGPD
related_docs:
  - fluxo-dsar-15-dias
  - formulario-requisicao-titular
---

# Matriz de Validação de Identidade nas Requisições (DSAR)

> **O dilema:** validar identidade é obrigatório para **não vazar dados de A para B** — mas pedir demais (ex.: senha, cópia de documento completo) cria **novo risco de privacidade** e viola a minimização (Art. 6º, III). Esta matriz equilibra os dois.

## Princípios

1. **Proporcionalidade ao risco:** quanto mais sensível o dado solicitado, mais forte a validação.
2. **Nunca pedir senha** ou dados de autenticação (se pedirmos, viramos alvo de phishing).
3. **O que não for necessário, não pedir** — e o que for pedido, descartar após a validação.
4. **Registrar** o método usado em cada requisição (trilha de auditoria).

## Níveis de validação

| Nível | Exige | Quando usar | Exemplo |
|---|---|---|---|
| **1 — Baixo** | E-mail/WhatsApp cadastrado + resposta de confirmação (token simples) | Dados não sensíveis, baixo impacto | Correção de e-mail, opt-out de marketing |
| **2 — Médio** | Nível 1 **+** dado do próprio cadastro (ex.: nº do último pedido, loja de compra, CPF + data de nascimento) | Dados pessoais comuns, relatório de acesso | Acesso ao relatório completo, portabilidade |
| **3 — Alto** | Nível 2 **+** confirmação por canal cruzado (e-mail E WhatsApp/SMS) ou **prova de identidade autenticada** (gov.br nível prata/ouro, biometria facial liveness) | Dados sensíveis, correção/exclusão de dados de saúde ou financeiros | Exclusão de dados de saúde; portabilidade de histórico financeiro |
| **4 — Representante legal** | Nível alto + **procuração/curatela** + conferência do documento do representante | Qualquer requisição feita por terceiro | Curador, procurador, advogado |

## Tabela decisória por direito

| Direito (Art. 18) | Nível mínimo | Observação |
|---|---|---|
| Confirmação de tratamento | 1 |  |
| Acesso | 2 | Relatório completo exige nível 2 |
| Correção | 2 | Se envolver dado sensível: nível 3 |
| Anonimização/bloqueio/eliminação | 2 |  |
| Portabilidade | 2–3 | Financeiro/saúde: nível 3 |
| Eliminação (consentimento) | 2 |  |
| Info. sobre compartilhamento | 2 |  |
| Info. sobre negar consentimento | 1 | Informativo |
| Revogação de consentimento | 1 | Baixo risco (beneficia o titular) |
| Revisão de decisão automatizada | 3 | Pode envolver dados sensíveis |

## Critérios de falha e tratamento

| Situação | Tratamento |
|---|---|
| Token não confirmado em 7 dias | Arquivar requisição como não validada; avisar o titular; reabrir mediante nova solicitação |
| Dados cadastrais não conferem | Pedir documento complementar (nível acima); **suspender prazo** até validação (documentado) |
| Suspeita de **fraude de identidade** | Não atender; escalar para segurança; registrar no fluxo de incidentes (pasta 05) |
| Representante sem procuração válida | Não atender até regularização |

## Boas práticas de segurança no processo

- **Descartar** documentos de identidade e provas após a validação (ou guardar por 60 dias em cofre, conforme política de retenção — [[politica-retencao-descarte|Política de Retenção]]).
- **Canal seguro:** envio de resposta por e-mail/WhatsApp com confirmação de leitura; nunca por chamada telefônica aberta.
- **Treinamento do SAC:** scripts prontos, sem improviso e sem perguntar senha.
- **Monitoramento:** % de requisições rejeitadas por falha de identidade e % de ataques detectados — indicadores do processo.

> Esta matriz integra o [[fluxo-dsar-15-dias|Fluxo DSAR]] e usa o [[formulario-requisicao-titular|Formulário de Requisição]].
