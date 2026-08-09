---
title: DPA — Acordo de Processamento de Dados (Operador — Art. 39)
date: 2026-08-08
tags: [lgpd, dpa, contrato, art-39, operador, portfolio, supermercado10]
aliases: [DPA, Acordo de Processamento, Contrato Operador]
status: approved
version: 1.0
owner: Encarregado de Dados (DPO)
framework: LGPD
related_docs:
  - clausula-transferencia-internacional
  - ../01-ropa-registro-de-atividades/ropa-registro-operacoes
  - ../05-plano-de-resposta-a-incidentes/playbook-resposta-incidente
---

# Acordo de Processamento de Dados (DPA) — Modelo para Operadores

> **Base legal:** Art. 39 da LGPD — o operador trata dados **somente conforme as instruções do controlador**. Este DPA é anexo obrigatório a todo contrato com fornecedor que trate dados pessoais em nome do Supermercado 10.
> **Como usar:** substitua os `[...]` pelos dados do fornecedor e do serviço. Mantenha os Anexos 1 e 2 sempre preenchidos.

---

**DPA nº [XXXX/2026]**

**CONTROLADOR:** Supermercados 10 Comércio de Alimentos Ltda., CNPJ 12.345.678/0001-90, Av. Paulista, 1.000, São Paulo/SP, doravante **Controlador**.

**OPERADOR:** [Razão social], CNPJ [CNPJ], [endereço], doravante **Operador**.

**SERVIÇO CONTRATADO:** [descrição do serviço — ex.: plataforma de e-mail marketing]

---

## CLÁUSULA 1 — Objeto e instruções

1.1. O Operador processa dados pessoais **exclusivamente** em nome e sob as instruções documentadas do Controlador, para a finalidade do Anexo 1, em conformidade com a LGPD (Lei 13.709/2018) e com esta instrução de tratamento.

1.2. É vedado ao Operador utilizar os dados para finalidade própria, incompatível ou diversa (Art. 6º, I e III). **Proibido o uso secundário** — incluindo treinamento de modelos de IA com dados do Controlador, salvo autorização expressa por escrito.

## CLÁUSULA 2 — Obrigações do Operador

2.1. Tratar dados conforme as instruções do Anexo 1 e do RoPA do Controlador;
2.2. **Garantir confidencialidade** (obrigação de sigilo contratual a todos os que acessarem);
2.3. Adotar as **medidas de segurança** do Anexo 2, no mínimo, e as exigidas pelo Art. 46;
2.4. **Notificar o Controlador em até 24h** da ciência de incidente de segurança, com os elementos do Art. 48;
2.5. **Auxiliar o Controlador** no atendimento aos direitos dos titulares (Art. 18), inclusive execução de exclusão/correção/portabilidade, com SLA de 10 dias;
2.6. **Apoiar o Controlador em RIPDs** (Art. 38) e em comunicações à ANPD (Art. 48);
2.7. Manter **registro das operações** (Art. 37) relativas ao serviço prestado;
2.8. Observar os **prazos de retenção** do Anexo 1 e **eliminar** os dados ao fim do serviço, salvo obrigação legal.

## CLÁUSULA 3 — Suboperadores e transferência

3.1. O Operador pode contratar suboperadores **somente com autorização prévia por escrito** do Controlador e sob os mesmos termos deste DPA (lista atualizada mantida no Anexo 3).
3.2. Transferências internacionais seguem o mecanismo legal aplicável (adequação ANPD ou SCCs da Res. CD/ANPD nº 19/2024), conforme [[clausula-transferencia-internacional|cláusula padrão de transferência]].

## CLÁUSULA 4 — Direitos de auditoria

4.1. O Controlador (ou auditor por ele indicado) poderá auditar o Operador quanto à conformidade com este DPA, mediante aviso prévio de [15] dias e sem custo ao Controlador, observada a confidencialidade.
4.2. O Operador disponibilizará informações e evidencias (relatórios de segurança, certificações, registros) solicitadas para fins de verificação e para atendimento à ANPD.

## CLÁUSULA 5 — Incidentes de segurança

5.1. Ao tomar ciência de incidente, o Operador deve:
- comunicar ao Controlador em **até 24h**, com avaliação preliminar (dados afetados, volume, medidas);
- **não comunicar** à ANPD ou a terceiros em nome do Controlador, salvo solicitação expressa;
- cooperar integralmente com a investigação, preservando evidências conforme [[Github/LGPD/05-plano-de-resposta-a-incidentes/README|Plano de Resposta a Incidentes]].

## CLÁUSULA 6 — Vigência, término e eliminação

6.1. Este DPA vigora enquanto durar o contrato de serviço.
6.2. Ao término, o Operador deve, conforme instrução do Controlador: **(i)** devolver os dados; e **(ii)** **eliminá-los** de todos os sistemas, incluindo backups, emitindo **certificado de eliminação** em até 30 dias — salvo obrigação legal de conservação, hipótese em que mantém apenas o mínimo legal e comunicará o Controlador.

## CLÁUSULA 7 — Responsabilidade

7.1. O Operador responde solidariamente (Art. 42, §1º) pelos danos decorrentes de tratamento em **desconformidade com a LGPD ou com as instruções** do Controlador, inclusive perante a ANPD e titulares.
7.2. O Controlador responde pelos danos decorrentes de suas próprias instruções.

## CLÁUSULA 8 — Disposições gerais

8.1. Alterações a este DPA exigem instrumento escrito assinado.
8.2. Foro: São Paulo/SP.
8.3. Este DPA é complementar e não substitui o contrato principal.

---

## ANEXO 1 — Instruções de Tratamento

| Item | Detalhe |
|---|---|
| Serviço/finalidade |  |
| Categorias de dados |  |
| Categorias de titulares |  |
| Operações permitidas | [coleta, armazenamento, uso, processamento, compartilhamento com o Controlador, eliminação] |
| Prazo de retenção |  |
| Base legal indicada |  |
| Data de início |  |

## ANEXO 2 — Medidas de Segurança Mínimas (Art. 46)

- [ ] Criptografia em trânsito (TLS 1.2+) e em repouso (AES-256)
- [ ] Controle de acesso baseado em função (RBAC) e MFA para administradores
- [ ] Gestão de vulnerabilidades e atualizações de segurança
- [ ] Registro e monitoramento de acessos (logs com retenção mínima de 6 meses)
- [ ] Procedimento de resposta a incidentes e notificação ao Controlador (24h)
- [ ] Teste/avaliação de segurança (pentest ou certificação ISO 27001/SOC 2, com periodicidade)
- [ ] Minimização e pseudonimização quando aplicável
- [ ] Garantia de eliminação segura ao fim do serviço (certificado)

## ANEXO 3 — Lista de Suboperadores autorizados

| Suboperador | Serviço | Localização | Transferência internacional? |
|---|---|---|---|
|  |  |  |  |

---

**Assinaturas** — [Nome/CPF] (Controlador) · [Nome/CPF] (Operador) — [data]
