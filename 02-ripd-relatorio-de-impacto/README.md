# 02 — RIPD · Relatório de Impacto à Proteção de Dados (Art. 38)

O **RIPD/DPIA** é obrigatório quando o tratamento pode gerar **alto risco** (Art. 38 da LGPD) e é o documento que a ANPD mais valoriza na fiscalização de casos de biometria e de decisões automatizadas. Muito poucos profissionais conseguem produzi-lo bem — ele demonstra domínio de **análise de risco**, **proporcionalidade** e **medidas de mitigação**.

## O caso escolhido: reconhecimento facial

Tratamento de **dados biométricos (sensíveis — Art. 5º, II)** de ~180.000 clientes, com duas finalidades:

1. **Prevenção à fraude** no programa de fidelidade (base: Art. 11, II, "g") — comparação contra a lista de bloqueio de fraudadores.
2. **Personalização de ofertas** (base: consentimento específico — Art. 11, I), com alternativa sem biometria.

É um caso **deliberadamente difícil**: exige teste de balanceamento, minimização (imagem descartada em <2s), revisão humana contra falso positivo, e alinhamento ao **Guia de Reconhecimento Facial da ANPD**.

## Estrutura do documento (modelo ANPD)

`ripd-reconhecimento-facial.md` segue a estrutura exigida pelo Guia Orientativo de RIPD da ANPD:

1. **Informações gerais** — identificação do controlador, encarregado e bases legais
2. **Escopo e descrição do tratamento** — finalidade, categorias de dados, titulares, sistemas, fluxo de dados (com diagrama) e compartilhamento
3. **Avaliação de necessidade e proporcionalidade** — minimização, expectativa razoável, alternativas
4. **Identificação e avaliação de riscos** — matriz de probabilidade × impacto (ISO 31000) e registro de 7 riscos
5. **Plano de ação e controles de mitigação** — controles técnicos e administrativos, risco residual e aceite formal
6. **Parecer do Encarregado** — favorável com condicionantes, com gatilhos de revisão

## Diferenciais

- **Risco residual formalmente aceito pela diretoria** — prática de accountability (Art. 6º, IX)
- **Diagrama de fluxo de dados** em Mermaid, visualizando a minimização
- **Referência à Res. CD/ANPD nº 19/2024** (SCCs) para transferência a data center nos EUA — sem se apoiar em premissas ultrapassadas sobre a UE (adequação mútua desde jan/2026)
- Integração com o RoPA (pasta 01), LIAs (pasta 03) e políticas (pasta 04)

[← Voltar ao índice](Github/LGPD/README.md)
