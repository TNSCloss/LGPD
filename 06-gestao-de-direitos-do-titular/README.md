# 06 — Gestão de Direitos do Titular (Art. 18)

A LGPD dá ao titular **10 direitos** (Art. 18) que devem ser atendidos em **15 dias**. Esta pasta mostra o processo completo de atendimento de requisições (DSAR) — do recebimento à resposta — sem tropeçar no detalhe que mais gera incidentes: a **validação de identidade**.

## O que há na pasta

| Arquivo | Conteúdo |
|---|---|
| `fluxo-dsar-15-dias.md` | Fluxo completo com SLAs internos (0/1/3/7/10/15 dias), diagrama e decisões de negócio |
| `formulario-requisicao-titular.md` | Formulário pronto (web/lojas/SAC) cobrindo os 10 direitos do Art. 18 |
| `templates-resposta-direitos.md` | **7 templates de resposta** pré-aprovados: acesso, correção, exclusão, portabilidade, revogação, oposição/automatizada e pedido não aplicável |
| `matriz-validacao-identidade.md` | Como validar identidade **sem criar novo risco** (nunca pedir senha; 4 níveis proporcionais) |

## Por que esta pasta vale ouro

- **Prazo de 15 dias** com SLA interno agressivo (resposta pronta em 10 dias) — folga para imprevistos.
- **Tratamento correto das exceções:** o template de exclusão explica por que NF fiscal **não** é excluída (Art. 16) — evitando negativa sem fundamento.
- **Matriz de identidade proporcional ao risco:** acesso simples = nível 1; exclusão de dados sensíveis = nível 3 (gov.br/biometria). É a resposta prática ao dilema "validar sem vazar".
- **Trilha de auditoria** e KPIs (95% dentro do prazo) — accountability (Art. 6º, IX).

## Documentos relacionados

- Canal do titular (página web): [09-canal-do-encarregado](Github/LGPD/09-canal-do-encarregado/README.md)
- DPA com operadores (execução de requisições): [07-contratos](Github/LGPD/07-contratos/README.md)
- Política de retenção (prazos dos registros DSAR): [04-politicas/politica-retencao-descarte](politica-retencao-descarte.md)

[← Voltar ao índice](Github/LGPD/README.md)
