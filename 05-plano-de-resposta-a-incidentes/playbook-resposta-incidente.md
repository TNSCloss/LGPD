---
title: Playbook — Resposta a Incidentes de Segurança e Privacidade (LGPD Art. 48)
date: 2026-08-08
tags: [lgpd, incidente, art-48, playbook, portfolio, supermercado10]
aliases: [Playbook de Incidentes, Manual de Resposta a Incidentes]
status: approved
version: 1.0
owner: Encarregado de Dados (DPO)
framework: LGPD
related_docs:
  - fluxograma-resposta-incidente
  - modelo-registro-incidente
  - modelo-comunicacao-anpd-titulares
---

# Playbook de Resposta a Incidentes de Segurança e Privacidade

> **Base legal:** Art. 48 da LGPD (notificação de incidentes) e **Res. CD/ANPD nº 15/2024** (procedimentos e prazos de comunicação: **3 dias úteis** para notificação preliminar e **20 dias úteis** para comunicação complementar).
> **Público:** CISO, Encarregado (DPO), TI, Jurídico, Comunicação, Gestores de loja.

---

## Fase 0 — PREPARAÇÃO (antes do incidente)

- [x] Comitê de Incidentes nomeado (CISO, DPO, TI, Jurídico, Comunicação) — ver [[comite-privacidade-regimento|Regimento do Comitê]]
- [x] Canais 24x7 divulgados e testados (quadrimestralmente)
- [x] **Runbook técnico** de contenção para os cenários conhecidos (ransomware, vazamento de banco, furto de notebook, phishing, DDoS)
- [x] Modelos de comunicação pré-aprovados pelo jurídico (este playbook)
- [x] Contratos com **forense digital** e **comunicação** de prontidão
- [x] Teste anual do playbook (simulado de mesa)

---

## Fase 1 — DETECÇÃO E TRIAGEM (T0 a T0+4h)

**Objetivo:** confirmar se há incidente de segurança e se envolve dados pessoais.

1. Qualquer pessoa detecta e comunica pelos canais 24x7 (nunca punição por reportar).
2. CISO registra no [[modelo-registro-incidente|Registro de Incidente]] e abre o time de resposta.
3. **Triagem inicial:**
   - Confidencialidade, integridade ou disponibilidade afetadas?
   - Envolve **dados pessoais** (nome, CPF, e-mail, dados financeiros, biométricos, de saúde)?
   - Qual sistema/operador, volume e categorias?
4. Classificação de severidade:

| Severidade | Critério | Exemplo |
|---|---|---|
| **CRÍTICA** | Vazamento de dados sensíveis em massa ou pagamento | Banco de clientes do e-commerce vazado |
| **ALTA** | Vazamento de dados pessoais, porém com criptografia/baixo volume | Notebook criptografado perdido com planilha |
| **MÉDIA** | Disponibilidade afetada sem vazamento | Ransomware criptografando backups |
| **BAIXA** | Incidente operacional sem dados pessoais | Phishing reportado e bloqueado sem acesso |

---

## Fase 2 — CONTENÇÃO E PRESERVAÇÃO (T0+4h a T0+24h)

**Objetivo:** conter o dano **sem destruir evidências**.

1. **Isolar** sistemas comprometidos (desconectar da rede — preservar imagem do disco primeiro).
2. **Não apagar** logs, não formatar, não reinstalar até orientação forense.
3. Revogar acessos comprometidos; resetar senhas; bloquear contas.
4. Notificar **operadores** envolvidos (exigência contratual do DPA) e solicitar evidências.
5. Acionar forense digital se severidade ALTA/CRÍTICA.
6. Registrar **linha do tempo** no registro de incidente.

> **Comunicação interna:** somente o porta-voz designado (Jurídico/Comunicação) fala sobre o incidente. Colaboradores não devem se manifestar publicamente.

---

## Fase 3 — AVALIAÇÃO DE RISCO AOS TITULARES (T0+24h)

**Objetivo:** decidir se o incidente é de **notificação obrigatória** (Art. 48).

Avaliar, para cada item:

| Fator | Pergunta | Influência |
|---|---|---|
| Natureza dos dados | Sensíveis (biométricos, saúde, financeiros)? | ↑↑ risco |
| Volume | Nº de titulares afetados | ↑ risco |
| Contexto | Dados expostos a terceiros ou apenas acessados? | ↑ se expostos |
| Salvaguardas | Dados **criptografados** com chave segura? | ↓↓ risco |
| Mitigação aplicada | Contenção rápida e eficaz? | ↓ risco |
| Danos potenciais | Fraude, discriminação, dano reputacional | ↑ risco |

> **Prudência:** em dúvida entre notificar ou não, **notifica-se** (o custo da não-notificação — multa + reputação — supera o da notificação).

---

## Fase 4 — NOTIFICAÇÃO À ANPD E AOS TITULARES

### 4.1 Notificação preliminar à ANPD (até 3 dias úteis)

Formulário da plataforma ANPD (`notificacao.anpd.gov.br`) com:

- Descrição resumida do incidente, data e forma de detecção
- Categorias e quantidade de titulares afetados
- Categorias de dados pessoais envolvidas
- **Medidas técnicas adotadas** (contenção, mitigação, criptografia aplicada)
- **Riscos** ao titular e medidas de tratamento
- Dados de contato do controlador e do encarregado

> Texto-modelo pronto em [[modelo-comunicacao-anpd-titulares|Modelo de Comunicação à ANPD]].

### 4.2 Comunicação complementar (até 20 dias úteis)

- Confirmação/atualização das informações preliminares
- Resultado das investigações
- Causa raiz, extensão e medidas corretivas definitivas
- Retificação de dados incorretos na preliminar

### 4.3 Comunicação aos titulares (imediatamente após confirmação de risco relevante)

- Linguagem **clara e simples** (não jurídica), individualizada quando possível
- O que aconteceu, quais dados, quais riscos
- O que o titular **deve fazer** (trocar senha, monitorar cartão, desconfiar de contatos)
- Medidas adotadas pela empresa e canal de atendimento

> Quando **não** notificar titulares: quando o risco for **não relevante** (ex.: dados criptografados e não acessados), registrando a justificativa.

---

## Fase 5 — REMEDIAÇÃO E LIÇÕES APRENDIDAS

1. Corrigir causa raiz (patch, mudança de configuração, treinamento).
2. Reforçar controles apontados na investigação.
3. Revisar o RoPA e o RIPD afetado.
4. **Lições aprendidas** em até 30 dias (documento próprio + reunião).
5. Atualizar este playbook e o [[fluxograma-resposta-incidente|fluxograma]].
6. Encerrar o incidente no registro com todos os campos preenchidos e parecer do DPO.

---

## Checklist de conformidade (Art. 48 + Res. CD/ANPD nº 15/2024)

- [ ] Incidente registrado em até 1h (registro oficial)
- [ ] Comitê acionado em até 4h
- [ ] Avaliação de relevância concluída em até 24h
- [ ] **Notificação preliminar ANPD em até 3 dias úteis** (se aplicável)
- [ ] **Comunicação complementar em até 20 dias úteis**
- [ ] Titulares notificados (se risco relevante) com orientações práticas
- [ ] Evidências preservadas e forense concluída
- [ ] Causa raiz corrigida e controles reforçados
- [ ] Registro completo + lições aprendidas arquivadas (5 anos)

> **Prazos internacionais:** se operações atingirem titulares na **UE**, aplica-se o prazo de **72h** do GDPR (Art. 33) — mais curto que o da LGPD; nos casos com transferência de dados, o prazo mais restritivo prevalece.
