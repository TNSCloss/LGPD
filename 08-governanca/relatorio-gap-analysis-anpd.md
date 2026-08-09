---
title: Relatório de Gap Analysis — Conformidade LGPD (Checklist ANPD antes/depois)
date: 2026-08-08
tags: [lgpd, gap-analysis, anpd, checklist, portfolio, supermercado10]
aliases: [Gap Analysis ANPD, Diagnóstico LGPD]
status: approved
version: 1.0
owner: Encarregado de Dados (DPO)
framework: LGPD
related_docs:
  - ../01-ropa-registro-de-atividades/ropa-registro-operacoes
  - ../03-lia-teste-de-legitimidade/README
  - matriz-bases-legais
---

# Relatório de Gap Analysis — Conformidade com a LGPD

> **Escopo:** Supermercados 10 (15 lojas, ~1.200 colaboradores, e-commerce/app). **Metodologia:** checklist baseado nos requisitos da LGPD e nos guias orientativos da ANPD, avaliado em **Antes** (estado inicial) e **Depois** (após implementação do programa). Classificação: ✅ conforme · ⚠️ parcial · ❌ não conforme.

## Resumo executivo

| Métrica | Antes | Depois |
|---|---|---|
| Itens conformes | 4 / 28 | **24 / 28** |
| Itens parciais | 5 / 28 | **4 / 28** |
| Itens não conformes | 19 / 28 | **0 / 28** |
| **Índice de conformidade** | **14%** | **86%** |

> **Leitura crítica:** o diagnóstico inicial (14%) é típico de varejo médio — dados coletados há anos sem governança. O salto para 86% veio da institucionalização: RoPA, bases legais documentadas, políticas aprovadas e canal do titular em produção. Os 4 itens parciais restantes dependem de **contratações e sistema** (prazos em 180 dias).

## Checklist detalhado (requisito → situação → ação)

### 1. Governança e estrutura

| # | Requisito | Antes | Depois | Observação |
|---|---|---|---|---|
| 1 | Encarregado (DPO) nomeado e publicado (Art. 41) | ❌ | ✅ | Publicado no site e na política externa |
| 2 | Canal de comunicação do titular ativo (Art. 41, §1º) | ❌ | ✅ | Página web + e-mail — pasta 09 |
| 3 | Comitê de privacidade instituído | ❌ | ✅ | Regimento aprovado — ver [[comite-privacidade-regimento|regimento]] |
| 4 | Programa de capacitação e treinamento | ❌ | ✅ | Cronograma anual — ver [[cronograma-treinamento-conscientizacao|cronograma]] |
| 5 | Mapa de processos e sistemas com dados pessoais | ❌ | ✅ | RoPA — pasta 01 |

### 2. Bases legais e transparência

| # | Requisito | Antes | Depois | Observação |
|---|---|---|---|---|
| 6 | Bases legais identificadas por processo (Art. 7º/11) | ❌ | ✅ | [[matriz-bases-legais|Matriz de Bases Legais]] |
| 7 | LIA para todos os usos de interesse legítimo (Art. 10, §3º) | ❌ | ✅ | 2 LIAs aprovados — pasta 03 |
| 8 | Política de privacidade externa (Art. 9) | ⚠️ | ✅ | Publicada com os 7 elementos — pasta 04 |
| 9 | Política de privacidade do colaborador | ❌ | ✅ | Publicada — pasta 04 |
| 10 | Registro de consentimento com prova (Art. 8º) | ❌ | ⚠️ | Plataforma de consentimento contratada; dados antigos em migração |
| 11 | Aviso de videomonitoramento nas lojas | ⚠️ | ✅ | Sinalização instalada nas 15 lojas |

### 3. Direitos do titular (Art. 17–22)

| # | Requisito | Antes | Depois | Observação |
|---|---|---|---|---|
| 12 | Fluxo de atendimento de requisições (15 dias) | ❌ | ✅ | Pasta 06 — SLA interno de 10 dias |
| 13 | Formulário e templates de resposta | ❌ | ✅ | Pasta 06 |
| 14 | Validação de identidade sem risco | ❌ | ✅ | Matriz de identidade — pasta 06 |
| 15 | Tratamento de decisões automatizadas (Art. 20) | ⚠️ | ✅ | Revisão humana documentada no RIPD e no fluxo DSAR |

### 4. Registro, segurança e operadores

| # | Requisito | Antes | Depois | Observação |
|---|---|---|---|---|
| 16 | RoPA mantido e auditável (Art. 37) | ❌ | ✅ | Planilha + markdown — pasta 01 |
| 17 | RIPD do tratamento de alto risco (Art. 38) | ❌ | ✅ | Reconhecimento facial — pasta 02 |
| 18 | Política de segurança da informação (Art. 46) | ⚠️ | ✅ | Pasta 04 |
| 19 | Plano de resposta a incidentes (Art. 48 + Res. 15/2024) | ❌ | ✅ | Pasta 05 |
| 20 | Contratos/DPA com todos os operadores (Art. 39) | ❌ | ⚠️ | Modelo pronto (pasta 07); **9 de 14 fornecedores** com DPA assinado (prazo 180 dias) |
| 21 | Política de retenção e descarte (Art. 16) | ❌ | ✅ | Pasta 04, com prazos normativos |

### 5. Transferências internacionais (Art. 33–36)

| # | Requisito | Antes | Depois | Observação |
|---|---|---|---|---|
| 22 | Inventário de transferências internacionais | ❌ | ⚠️ | Levantado no RoPA; SCCs da Res. 19/2024 em assinatura (AWS) |
| 23 | Mecanismo válido por destino (adequação/SCC/BCR) | ❌ | ✅ | UE: adequação (2026); EUA: SCCs — pasta 07 |

### 6. Controles transversais

| # | Requisito | Antes | Depois | Observação |
|---|---|---|---|---|
| 24 | Privacy by design em novos projetos (Art. 46, §2º) | ❌ | ✅ | Gate de privacidade no ciclo de projetos (checklist) |
| 25 | Registro de requisições e incidentes (accountability) | ❌ | ✅ | Trilhas de auditoria — pastas 05 e 06 |
| 26 | Revisão periódica do programa | ❌ | ✅ | Revisão anual + gatilhos — RoPA, LIAs, RIPD |
| 27 | Treinamento de colaboradores e comunicação | ❌ | ✅ | Cronograma anual — pasta 08 |
| 28 | Documentação disponível para auditoria/ANPD | ❌ | ✅ | Este portfólio em repositório versionado |

## Plano de ação (itens parciais)

| Item | Ação | Prazo | Responsável |
|---|---|---|---|
| 10 (consentimento) | Migrar registros legados para a nova plataforma | 180 dias | TI + DPO |
| 20 (DPAs) | Assinar DPA com os 5 fornecedores pendentes | 180 dias | DPO + Compras |
| 22 (transferências) | Concluir SCCs com AWS | 90 dias | DPO + TI |

## Conclusão

A Supermercados 10 atingiu **estado de conformidade operacional (86%)**, com **zero itens não conformes** e plano de ação claro para os 4 itens parciais. O programa é sustentável: todos os documentos estão versionados, com responsáveis e gatilhos de revisão. **Próxima auditoria de conformidade:** 08/02/2027.

> **Nota de honestidade metodológica:** a conformidade LGPD é **contínua, não binária**. Este relatório documenta o estado em 08/08/2026; a manutenção (revisões anuais, treinamento, atualização normativa) é o que sustenta o percentual ao longo do tempo.
