---
title: Registro de Operações de Tratamento de Dados Pessoais (RoPA) — Supermercado 10
date: 2026-08-08
tags: [lgpd, ropa, art-37, portfolio, supermercado10]
aliases: [RoPA, Registro de Operações, Art. 37]
status: approved
version: 1.0
owner: Encarregado de Dados (DPO)
framework: LGPD
---

# Registro de Operações de Tratamento (RoPA) — Art. 37 da LGPD

> **Controladora:** Supermercados 10 Comércio de Alimentos Ltda. — CNPJ 12.345.678/0001-90 — Av. Paulista, 1.000, São Paulo/SP
> **Encarregado de Dados:** [Nome do Encarregado] — lgpd@supermercado10.com.br
> **Versão:** 1.0 · **Data:** 08/08/2026 · **Versão em planilha:** `ropa-supermercado10.xlsx`

Este documento atende ao **Art. 37 da LGPD** (manutenção do registro das operações de tratamento de dados pessoais) e é a fonte de referência para auditoria, para o [[matriz-bases-legais|mapeamento de bases legais]] e para o [[relatorio-gap-analysis-anpd|gap analysis]] da companhia.

---

## 1. Legenda das Bases Legais

| Sigla | Base Legal | Artigo |
|---|---|---|
| **CONS** | Consentimento | Art. 7º, I / Art. 11, I |
| **OBL** | Cumprimento de obrigação legal/regulatória | Art. 7º, II |
| **CONTR** | Execução de contrato (ou preliminares) | Art. 7º, V |
| **LEGIT** | Interesse legítimo do controlador (exige LIA — Art. 10, §3º) | Art. 7º, IX |
| **CRED** | Proteção do crédito | Art. 7º, X |
| **SAUDE** | Tutela da saúde (dados sensíveis) | Art. 11, II, "f" |
| **FRAUDE** | Prevenção à fraude e segurança em autenticação (dados sensíveis) | Art. 11, II, "g" |

> **Regra de ouro:** toda base de interesse legítimo precisa de um **LIA** (Teste de Legitimidade) documentado — ver [[Github/LGPD/03-lia-teste-de-legitimidade/README|pasta 03 - LIA]]. Todo processo de **alto risco** precisa de **RIPD** (Art. 38) — ver [[Github/LGPD/02-ripd-relatorio-de-impacto/README|pasta 02 - RIPD]].

---

## 2. Processo 1 — Recursos Humanos (RH)

| Campo | Registro |
|---|---|
| **Área responsável** | Recursos Humanos |
| **Sistemas** | Sistema de RH (Senior), eSocial, folha de pagamento, relógio de ponto biométrico |
| **Titulares** | Candidatos, colaboradores, dependentes |

| Dado Pessoal | Categoria de Titular | Base Legal | Finalidade | Retenção | Compartilhamento | Medidas de Segurança |
|---|---|---|---|---|---|---|
| Nome, CPF, RG, endereço, e-mail, telefone, currículo (formação, experiência) | Candidatos | OBL + LEGIT (LIA-01) | Seleção e contratação | 12 meses após o fim do processo seletivo | Clínica de medicina do trabalho (só no exame admissional) | RBAC, backup criptografado, senha forte, trilha de auditoria, termo de confidencialidade |
| Nome, CPF, PIS, dados bancários, endereço, dependentes, escala, marcações de ponto, ASO | Colaboradores e dependentes | CONTR + OBL; dados de saúde: SAUDE | Gestão do vínculo empregatício e obrigações legais (CLT, eSocial, NR-7) | Prontuário: 5 anos pós-vínculo; ASO: 20 anos (NR-7); ponto: 5 anos | Banco (folha), seguradora de benefícios, clínica ocupacional | Criptografia em repouso, segregação de funções, acesso por necessidade, DPA com operadores |
| Dado biométrico (impressão digital) | Colaboradores | FRAUDE (autenticação no ponto) | Identificação no registro de ponto | Enquanto durar o vínculo; descarte em 30 dias após desligamento | Não compartilhado | Template irreversível/hash, sem envio a terceiros, acesso restrito RH/TI |

---

## 3. Processo 2 — Marketing

| Campo | Registro |
|---|---|
| **Área responsável** | Marketing / CRM |
| **Sistemas** | Plataforma de CRM, plataforma de e-mail/SMS, programa de fidelidade "Cliente 10", mídia digital (Meta/Google) |
| **Titulares** | Clientes do programa de fidelidade, clientes do e-commerce, leads |

| Dado Pessoal | Categoria de Titular | Base Legal | Finalidade | Retenção | Compartilhamento | Medidas de Segurança |
|---|---|---|---|---|---|---|
| Nome, CPF, e-mail, telefone, nascimento, CEP, histórico de compras, pontos | Clientes do "Cliente 10" | CONTR (programa de fidelidade) | Acúmulo/resgate de pontos e ofertas no programa | Cadastro ativo + 24 meses sem interação | Software house do programa, CRM (operadores) | Criptografia, RBAC, minimização, DPA, pseudonimização em analytics |
| E-mail, telefone, IP, cookies, preferências de contato | Clientes e leads | LEGIT (LIA-02, clientes) + CONS (não-clientes) | Campanhas, ofertas e comunicação | Enquanto válida a base legal (opt-out imediato); leads: 24 meses sem interação | Plataforma de e-mail/SMS, agência, Meta/Google (com consentimento de cookies) | Opt-out em toda comunicação, gestão de preferências, DPA, trilha de consentimento |

> **Leia também:** [[lia-2-marketing-direto|LIA-02 — Marketing Direto]].

---

## 4. Processo 3 — Vendas

| Campo | Registro |
|---|---|
| **Área responsável** | Operações de Loja / E-commerce |
| **Sistemas** | PDV, ERP, e-commerce (VTEX), app, adquirente de pagamento |
| **Titulares** | Clientes |

| Dado Pessoal | Categoria de Titular | Base Legal | Finalidade | Retenção | Compartilhamento | Medidas de Segurança |
|---|---|---|---|---|---|---|
| Nome, CPF, endereço de entrega, telefone, e-mail, itens, valor, forma de pagamento | Clientes | CONTR + OBL (NF-e) | Venda, entrega e emissão fiscal | NF-e: 5 anos (fiscal); entrega: 6 meses pós entrega | Adquirente/credenciadora, transportadora, software house (operadores) | Tokenização do PAN (nunca retido), TLS, RBAC, logs, PCI DSS via adquirente |
| Nome, CPF, e-mail, telefone, IP, cookies, navegação | Clientes do e-commerce/app | CONTR + LEGIT (segurança do serviço) | Cadastro, autenticação, carrinho, personalização | Cadastro ativo + 24 meses sem atividade; cookies conforme mapa | Nuvem, plataforma de e-commerce, CDN, analytics (operadores) | MFA para equipe, criptografia, WAF, monitoramento, DPA |

---

## 5. Processo 4 — Financeiro

| Campo | Registro |
|---|---|
| **Área responsável** | Financeiro / Crédito e Cobrança |
| **Sistemas** | ERP financeiro, sistema de cobrança, bureaus de crédito, escritório contábil |
| **Titulares** | Clientes, fornecedores, colaboradores |

| Dado Pessoal | Categoria de Titular | Base Legal | Finalidade | Retenção | Compartilhamento | Medidas de Segurança |
|---|---|---|---|---|---|---|
| Nome, CPF, telefone, e-mail, histórico de compras, valores em aberto | Clientes inadimplentes | LEGIT (LIA-01) + CONTR | Cobrança e negociação de dívidas | 5 anos após quitação/prescrição (Art. 206 CC) | Escritório de cobrança, bureaus de crédito (CRED) | Minimização, restrição de horário de contato, DPA, logs |
| Nome, CPF, renda, histórico de pagamentos, consultas a bureaus | Solicitantes de crédito | CRED + CONTR | Análise de concessão de crédito (cartão próprio) | Vigência do contrato + 5 anos após encerramento | Bureaus de crédito (controladores autônomos), IF parceira | Acesso restrito, criptografia, relatório de score (Art. 20), DPA |
| Notas fiscais, registros contábeis, dados bancários | Clientes, fornecedores, colaboradores | OBL | Cumprimento de obrigações fiscais e contábeis | 5 anos / conforme legislação | Escritório contábil, autoridades fiscais | Criptografia em repouso, RBAC, backup, trilha de auditoria |

---

## 6. Processo 5 — Tecnologia da Informação (TI)

| Campo | Registro |
|---|---|
| **Área responsável** | TI / Segurança da Informação |
| **Sistemas** | SIEM, WAF, antivírus, câmeras (DVR/NVR), help desk |
| **Titulares** | Colaboradores, clientes, visitantes |

| Dado Pessoal | Categoria de Titular | Base Legal | Finalidade | Retenção | Compartilhamento | Medidas de Segurança |
|---|---|---|---|---|---|---|
| IP, MAC, user-agent, autenticações, tráfego de rede, eventos de segurança | Colaboradores, clientes, visitantes | LEGIT (segurança) + OBL | Detecção e resposta a incidentes | 6 meses (até 12 em investigação) | SOC/provedor de segurança, nuvem (operadores) | Logs centralizados com acesso restrito, pseudonimização, SIEM com alertas |
| Imagens de vídeo | Clientes, colaboradores, visitantes | LEGIT (LIA-01, patrimônio) + FRAUDE (se biometria) | Segurança patrimonial e prevenção de furtos | 30 dias corridos (prorrogável em investigação) | Empresa de monitoramento (operador) | Sinalização nas áreas, acesso restrito, autenticação no DVR/NVR, trilha de auditoria |
| Nome, matrícula, e-mail corporativo, chamados, IP | Colaboradores | LEGIT + CONTR | Suporte e provisionamento de acesso | Registro de chamados: 12 meses | Prestadores de suporte de TI (operadores) | MFA administrativo, privilégio mínimo, segregação de funções, confidencialidade |

---

## 7. Fluxo de revisão do RoPA

A planilha e este registro são **revisados** quando:

- [ ] Novo processo ou sistema de tratamento entra em operação
- [ ] Mudança de base legal ou finalidade de tratamento existente
- [ ] Novo compartilhamento/operador contratado
- [ ] Incidente de segurança relevante (Art. 48)
- [ ] Atualização normativa da ANPD ou mudança de entendimento
- [ ] Revisão anual obrigatória (próxima: **08/08/2027**)

---

## 8. Documentos relacionados

- [[Github/LGPD/02-ripd-relatorio-de-impacto/README|RIPD — Relatório de Impacto (pasta 02)]]
- [[Github/LGPD/03-lia-teste-de-legitimidade/README|LIA — Testes de Legitimidade (pasta 03)]]
- [[matriz-bases-legais|Matriz de Bases Legais]]
- [[politica-retencao-descarte|Política de Retenção e Descarte]]
- [[relatorio-gap-analysis-anpd|Gap Analysis ANPD]]

> **Nota de transparência (Art. 6º, IX — accountability):** este registro foi elaborado com base na LGPD (Lei 13.709/2018) e nos guias orientativos da ANPD. Os prazos de retenção seguem obrigações legais aplicáveis (CLT, CTN, NR-7, Art. 206 do CC) e práticas de mercado, devendo ser validados por assessoria jurídica antes da implementação.
