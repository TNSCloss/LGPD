---
title: Matriz de Bases Legais — Supermercado 10 (Art. 7º e Art. 11)
date: 2026-08-08
tags: [lgpd, bases-legais, art-7, art-11, matriz, portfolio, supermercado10]
aliases: [Matriz de Bases Legais]
status: approved
version: 1.0
owner: Encarregado de Dados (DPO)
framework: LGPD
related_docs:
  - ../01-ropa-registro-de-atividades/ropa-registro-operacoes
  - ../03-lia-teste-de-legitimidade/README
---

# Matriz de Bases Legais (Art. 7º e Art. 11 da LGPD)

> Mapeamento de **cada processo de tratamento** do [[ropa-registro-operacoes|RoPA]] para uma das bases legais do Art. 7º (dados pessoais) e Art. 11 (dados sensíveis). Documenta o princípio da finalidade (Art. 6º, I) e a accountability (Art. 6º, IX).

## As 10 bases do Art. 7º (e as do Art. 11)

| # | Base | Uso no Supermercado 10 |
|---|---|---|
| **I** | Consentimento | Marketing para **não-clientes**; cookies analíticos/marketing; personalização com biometria (Art. 11, I) |
| **II** | Obrigação legal/regulatória | NF-e, folha/ponto/eSocial, arquivamento fiscal, registros exigidos |
| **III** | Políticas públicas | Não aplicável (ente privado sem execução de política pública) |
| **IV** | Estudos por órgão de pesquisa | Não aplicável (sem projetos atuais — se vier a ocorrer, exigirá revisão) |
| **V** | Execução de contrato | Vendas, programa de fidelidade, vínculo empregatício, cobrança da dívida contratual |
| **VI** | Exercício regular de direitos em processo judicial/administrativo/arbitral | Defesa em ações trabalhistas, cíveis e reclamações ANPD |
| **VII** | Proteção da vida/incolumidade física | Situações de emergência em loja (uso emergencial, documentado) |
| **VIII** | Tutela da saúde (profissionais/serviços de saúde) | Exames ocupacionais pela clínica (dados sensíveis — Art. 11, II, "f") |
| **IX** | **Interesse legítimo** | Videomonitoramento, logs de segurança, cobrança, marketing a clientes — **com LIA** (Art. 10, §3º) |
| **X** | Proteção do crédito | Análise de crédito e consultas a bureaus |

**Art. 11 (sensíveis):** I (consentimento — biometria para personalização) e II, "f"/"g" (saúde ocupacional; biometria para autenticação/segurança).

## Matriz de mapeamento processo → base legal

| Processo (RoPA) | Base(s) legal(is) | Tipo de dado | Documento de suporte |
|---|---|---|---|
| RH — Recrutamento e seleção | II + IX | Pessoais | LIA-01 |
| RH — Gestão de colaboradores | V + II | Pessoais | RoPA |
| RH — Saúde ocupacional (ASO) | **II, "f" (11)** | Sensíveis | RoPA |
| RH — Biometria no ponto | **II, "g" (11)** | Sensíveis | RoPA |
| Marketing — Fidelidade "Cliente 10" | V | Pessoais | RoPA |
| Marketing — Campanhas (clientes) | **IX** | Pessoais | **LIA-02** |
| Marketing — Campanhas (não-clientes/leads) | I | Pessoais | Registro de consentimento |
| Marketing — Cookies | I | Pessoais | Política de Cookies |
| Vendas — Checkout e NF-e | V + II | Pessoais | RoPA |
| Vendas — Pagamento (adquirente) | V | Pessoais | DPA + PCI DSS |
| Vendas — E-commerce/app | V + IX | Pessoais | LIA-01 |
| Financeiro — Cobrança | IX + V | Pessoais | **LIA-01** |
| Financeiro — Análise de crédito | **X** + V | Pessoais | RoPA |
| Financeiro — Fiscal/contábil | II | Pessoais | RoPA |
| TI — Logs e monitoramento | IX + II | Pessoais | **LIA-01** |
| TI — Videomonitoramento | IX (II, "g" se biometria) | Pessoais | **LIA-01** |
| TI — Suporte/help desk | IX + V | Pessoais | LIA-01 |
| Segurança — Reconhecimento facial (entrada) | **II, "g" (11)** + **I (11)** | Sensíveis | **RIPD-2026-001** |

## Regras de negócio da matriz

1. **Um processo pode ter mais de uma base** para fluxos distintos — o RoPA detalha linha a linha.
2. **Interesse legítimo nunca fica "solto":** sempre referenciado a um LIA aprovado.
3. **Dados sensíveis (Art. 11)** só com base própria — nunca com base do Art. 7º.
4. **Bases não usadas são declaradas** ("não aplicável"), demonstrando que a análise foi feita.
5. Revisão anual da matriz (próxima: **08/08/2027**) e a cada mudança de fluxo.

> **Nota:** esta matriz é material de implementação; a aplicação a caso concreto deve ser validada por assessoria jurídica.
