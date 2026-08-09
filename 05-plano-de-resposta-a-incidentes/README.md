# 05 — Plano de Resposta a Incidentes (Art. 48)

Incidentes acontecem. O que separa uma empresa preparada de uma em pânico é o **plano**. Esta pasta contém o conjunto completo para resposta a incidentes de segurança com dados pessoais, do acionamento à notificação regulatória.

## O que há na pasta

| Arquivo | Conteúdo |
|---|---|
| `fluxograma-resposta-incidente.md` | **Fluxograma** visual (Mermaid) com os tempos-chave: detecção → contenção → avaliação → notificação |
| `playbook-resposta-incidente.md` | **Playbook passo a passo** em 6 fases: preparação, detecção/triagem, contenção, avaliação de risco, notificação, remediação/lições |
| `modelo-registro-incidente.md` | **Modelo de Registro de Incidente** (INC-XXXX): linha do tempo, dados afetados, protocolos ANPD, encerramento |
| `modelo-comunicacao-anpd-titulares.md` | **Modelos de comunicação prontos**: preliminar ANPD (3 dias úteis), complementar (20 dias úteis), texto para titulares e aviso no site |

## Tempos que valem ouro (e mostram domínio da Res. CD/ANPD nº 15/2024)

| Ação | Prazo |
|---|---|
| Acionamento do comitê | 4h |
| Avaliação de relevância | 24h |
| **Notificação preliminar ANPD** | **3 dias úteis** |
| **Comunicação complementar ANPD** | **20 dias úteis** |
| Comunicação aos titulares | Imediato, se risco relevante |
| Nota: para titulares na UE (GDPR) | 72 horas — prazo mais curto prevalece |

## Diferenciais

- **Quem aciona quem**, com canais 24x7 e regras de escalonamento claras (dados sensíveis envolvidos → notifica-se mesmo com dúvida).
- **Modelos prontos**, pré-aprovados pela linguagem exigida pela ANPD — a equipe só preenche, não parte do zero sob pressão.
- **Prudência documentada:** critérios objetivos para decidir *quando não notificar* (dados criptografados) — e registrando a justificativa.
- Teste anual do plano (simulado de mesa).

[← Voltar ao índice](Github/LGPD/README.md)
