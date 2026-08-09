# 03 — LIA · Testes de Legitimidade (Art. 10, §3º)

O **LIA (Legitimate Interest Assessment)** é o documento que comprova que o uso de **interesse legítimo** (Art. 7º, IX) é legal e proporcional. É raro ver isso bem feito — a maioria das empresas usa "interesse legítimo" como coringa sem qualquer documento. Aqui, cada uso da base é **lastreado por um LIA com 4 etapas**.

## Estrutura dos LIAs (4 etapas — padrão EDPB adaptado à LGPD)

1. **Finalidade Legítima** — a finalidade existe, é específica e tem base no interesse do controlador/terceiro
2. **Necessidade** — os dados são mínimos e não há alternativa menos intrusiva
3. **Balanceamento** — os interesses do controlador **não prevalecem** sobre os direitos e liberdades dos titulares
4. **Salvaguardas** — medidas que protegem o titular (opt-out, minimização, transparência, DPA)

## Os dois documentos

| Arquivo | Caso | Conclusão |
|---|---|---|
| `lia-1-prevencao-fraude.md` | Prevenção à fraude, cobrança e segurança patrimonial (câmeras, logs) | Interesse legítimo prevalece com salvaguardas (minimização por desenho, revisão humana, retenção controlada) |
| `lia-2-marketing-direto.md` | Marketing direto a **clientes existentes** | Prevalece **somente para clientes ativos**; para não-clientes, a base é consentimento |

## O que diferencia este material

- **Delimitação de escopo honesta:** o LIA de marketing deixa explícito que **não autoriza** compra de base, telemarketing ou perfilamento sensível — mostrando que você sabe onde o interesse legítimo termina.
- **Integração com o RoPA:** cada uso de interesse legítimo no RoPA (pasta 01) referencia seu LIA.
- **Monitoramento contínuo:** cada LIA define indicadores (ex.: taxa de descadastro) e gatilhos de revisão.
- **Teste de balanceamento com fatores objetivos** (severidade, expectativa razoável, benefício, alternativas).

[← Voltar ao índice](Github/LGPD/README.md)
