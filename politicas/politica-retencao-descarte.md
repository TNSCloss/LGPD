---
title: Política de Retenção e Descarte de Dados Pessoais — Supermercado 10
date: 2026-08-08
tags: [lgpd, politica, retencao, descarte, art-16, portfolio, supermercado10]
aliases: [Política de Retenção, Política de Descarte, Retention Policy]
status: approved
version: 1.0
owner: Encarregado de Dados (DPO)
framework: LGPD
related_docs:
  - ../01-ropa-registro-de-atividades/ropa-registro-operacoes
  - politica-privacidade-externa-site
  - politica-privacidade-interna-colaboradores
---

# Política de Retenção e Descarte de Dados Pessoais

> **Base legal:** Art. 16 da LGPD — os dados pessoais devem ser **eliminados** após o término do tratamento, **salvo** nas hipóteses de conservação autorizadas (obrigação legal, estudo por órgão de pesquisa, transferência a terceiro, ou uso exclusivo do controlador sem acesso de terceiros).
> **Controladora:** Supermercados 10 Comércio de Alimentos Ltda. — CNPJ 12.345.678/0001-90

## 1. Objetivo

Definir os prazos de guarda e o método de descarte dos dados pessoais tratados pela companhia, garantindo o **princípio da necessidade** (Art. 6º, III), a **eliminação** após o fim da finalidade (Art. 16) e a segurança do descarte (Art. 46).

## 2. Princípios

1. **Retenção mínima:** guardar somente pelo tempo necessário à finalidade ou exigido em lei.
2. **Descarte seguro:** destruição irreversível, com comprovação.
3. **Revisão periódica:** prazos revisados anualmente e a cada mudança legal.
4. **Accountability:** registro das eliminações.

## 3. Tabela de Prazos de Retenção

| Dado / Documento | Prazo de Retenção | Fundamento | Descarte |
|---|---|---|---|
| **Currículos (CVs)** de candidatos não contratados | **12 meses** após o fim do processo seletivo | Prática de mercado + Art. 16 (sem retenção além da finalidade); base: OBL/LEGIT (LIA-01) | Exclusão digital segura |
| CV de candidato **contratado** | Incorporado ao prontuário; prontuário: **5 anos** pós-vínculo | CLT / Art. 16 | Exclusão digital segura |
| Dados da **relação de trabalho** (holerites, férias, rescisão) | **5 anos** após o fim do vínculo | Art. 10, II do ADCT (prescrição trabalhista) | Exclusão + certificado de eliminação |
| **Marcações de ponto** | **5 anos** | Portaria MTP 671/2021 | Exclusão digital segura |
| **ASO / exames ocupacionais** | **20 anos** | NR-7, item 7.5.7 | Destruição de prontuário em papel + exclusão digital |
| Dados **biométricos** (ponto) | Enquanto durar o vínculo; **30 dias** após desligamento | Art. 16 + minimização | Exclusão irreversível do template |
| **Notas fiscais e documentos fiscais** | **5 anos** | CTN / legislação fiscal (Art. 173) | Arquivo morto + destinação final |
| Dados de **pedidos/entregas** (pós-venda) | 6 meses após a entrega | Interesse legítimo (LIA-01) | Exclusão digital segura |
| Cadastro **Cliente 10** (fidelidade) | Enquanto ativo + **24 meses** sem interação | Execução de contrato (Art. 7º, V) | Exclusão + aviso ao titular |
| **Cookies analíticos/marketing** | Conforme [[../09-canal-do-encarregado/politica-cookies|Política de Cookies]] (até 12 meses) | Consentimento | Exclusão automática |
| **Videomonitoramento** (imagens) | **30 dias corridos** (prorrogável se investigação) | Interesse legítimo (LIA-01) | Sobrescrita automática/exclusão |
| **Logs de segurança (TI)** | 6 meses (até **12** em investigação) | Interesse legítimo (LIA-01) | Exclusão automatizada |
| **Registros de incidentes** (Art. 48) | **5 anos** | Accountability (Art. 6º, IX) | Arquivo + exclusão |
| **Registros de requisições de titulares** (DSAR) | **5 anos** | Accountability (Art. 6º, IX) | Exclusão digital segura |
| Contratos e documentos contábeis | **5 anos** após o encerramento | Art. 206 do CC (prescrição) | Arquivo + destinação |
| Dados pessoais em mídia de **backup** | Conforme o prazo do dado de origem; backups não restaurados são sobrescritos | Art. 16 | Sobrescrita/destruição física |

> **Exceções (Art. 16):** os prazos acima **podem ser superados** quando (i) houver obrigação legal/regulatória específica, (ii) houver estudo por órgão de pesquisa com anonimização, (iii) houver transferência a terceiro mediante determinação legal, ou (iv) houver uso exclusivo do controlador sem acesso de terceiros (ex.: dado em processo judicial).

## 4. Métodos de Descarte

| Meio | Método | Responsável |
|---|---|---|
| Arquivos digitais (bases, planilhas, backups) | Exclusão lógica segura + sobrescrita; certificado de eliminação | TI / DPO |
| Documentos em papel (prontuários, contratos) | **Fragmentação/destruição** com certificado; empresa certificada para documentos sigilosos | RH/Financeiro com fornecedor |
| Equipamentos (HDs, DVRs, notebooks) | **Desmagnetização/destruição física** ou formatação de baixo nível + certificado | TI |
| E-mails e anexos | Exclusão das caixas e de backups excedentes (caixas retidas conforme política de correio) | TI / usuários |
| Nuvem (arquivos em operadores) | Exclusão via API com **certificado de exclusão do operador** e confirmação de retenção zero | DPO/TI com operadores |

## 5. Processo de Eliminação

1. A área **data owner** identifica dados com prazo vencido (agendado mensalmente).
2. A eliminação é executada por TI, **documentada em registro de eliminação** (o que, quando, por quem, método).
3. O DPO audita trimestralmente amostras de eliminação.
4. Suspende-se a eliminação **apenas** em litígio, investigação ou ordem judicial (com registro do motivo).

## 6. Responsabilidades

| Papel | Responsabilidade |
|---|---|
| **Encarregado (DPO)** | Governança da política, revisão anual, auditoria de eliminação |
| **Data Owners (RH, Financeiro, Marketing, Operações, TI)** | Identificar prazos vencidos e autorizar eliminação |
| **TI** | Executar eliminação técnica e emitir certificados |
| **Comitê de Privacidade** | Aprovar exceções e mudanças de prazo — ver [[../08-governanca/comite-privacidade-regimento|regimento]] |

## 7. Revisão

Esta política é revisada anualmente ou a cada mudança legal relevante. A tabela de prazos é mantida em sincronia com o [[ropa-registro-operacoes|RoPA]]. Última revisão: **08/08/2026** · Próxima: **08/08/2027**.

> **Nota:** prazos aqui são referências para implementação; cada prazo legal citado deve ser confirmado com assessoria jurídica conforme a atividade específica.
