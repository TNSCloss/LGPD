# 09 — Canal do Encarregado e Política de Cookies

O Art. 41, §1º da LGPD exige que o Encarregado tenha um **canal de comunicação com os titulares**. Aqui está uma página funcional e a política de cookies com o mapa completo.

## O que há na pasta

| Arquivo | Conteúdo |
|---|---|
| `index.html` | **Página web do canal do titular** (HTML/CSS/JS puros, sem dependências) — formulário DSAR, lista dos 10 direitos do Art. 18, contatos e canal de incidentes |
| `politica-cookies.md` | **Política de Cookies** com **mapa de cookies** por categoria: essenciais, analíticos e marketing |
| `README.md` | Este índice + instruções do screenshot |

## Como gerar o print da página

A página é autossuficiente (abre sem servidor). Para o screenshot do portfólio:

```bash
# 1) Abra no navegador
open index.html            # mac
xdg-open index.html        # linux
start index.html           # windows

# 2) Ou gere o print por linha de comando (se tiver um navegador headless)
google-chrome --headless --screenshot=canal-encarregado.png --window-size=1200,900 index.html
# ou
chromium --headless --screenshot=canal-encarregado.png --window-size=1200,900 index.html
```

Depois, adicione a imagem ao repositório e referencie-a aqui como `![Canal do Encarregado](canal-encarregado.png)` (o placeholder foi deixado como comentário no HTML).

> **Dica:** para uma versão com identidade real, substitua `[Nome do Encarregado]` no HTML e ajuste as cores da marca.

## Diferenciais

- **Formulário que cobre os 10 direitos do Art. 18** em um único seletor, alinhado ao fluxo DSAR da pasta 06.
- **Canal de incidente separado** com alerta visual (Art. 48) — mostra a preocupação com notificação ágil.
- **Mapa de cookies com categorias, fornecedores, dados, duração e base legal** — nível de detalhe que a maioria dos sites não publica.
- **Sem dependências externas** — sem CDN, sem trackers no próprio código da página (coerência com o tema).

## Documentos relacionados

- Fluxo de atendimento (15 dias): [06-gestao-de-direitos-do-titular](Github/LGPD/06-gestao-de-direitos-do-titular/README.md)
- Política de privacidade do site: [04-politicas/politica-privacidade-externa-site](politica-privacidade-externa-site.md)
- LIA de marketing (base dos cookies de marketing): [03-lia-teste-de-legitimidade/lia-2-marketing-direto](lia-2-marketing-direto.md)

[← Voltar ao índice](Github/LGPD/README.md)
