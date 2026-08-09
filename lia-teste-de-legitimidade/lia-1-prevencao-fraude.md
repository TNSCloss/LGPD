# LIA-01 · Teste de Legitimidade (LIA) — Prevenção à Fraude e Segurança Patrimonial

> **Enquadramento legal:** Art. 7º, IX + Art. 10, §3º da LGPD — o controlador que usa interesse legítimo **deve documentar** a necessidade, o balanceamento e as salvaguardas (LIA — *Legitimate Interest Assessment*).
> **Alcance:** cobrança de clientes inadimplentes, videomonitoramento das lojas, monitoramento de segurança de TI e fraudes no programa de fidelidade.

---

## 1. Finalidade Legítima

| Pergunta | Resposta |
|---|---|
| Qual é a finalidade do tratamento? | Prevenir e combater fraudes (cobrança, devoluções abusivas, furtos), proteger o patrimônio e garantir a segurança de colaboradores, clientes e ambientes (lojas, CD, estacionamentos). |
| A finalidade é legítima e específica? | **Sim.** Há interesse legítimo do controlador (redução de prejuízo) e de terceiros (segurança de clientes e colaboradores) — Art. 7º, IX. |
| A finalidade pode ser alcançada de outra forma menos intrusiva? | Videomonitoramento e logs de TI **não têm alternativa** de eficácia equivalente; cobrança de dívida legítima é exercício regular de direito (Art. 7º, IX c/c Art. 206 do CC). |
| Documentação | RoPA, processos "Financeiro — Cobrança", "TI — Logs e Monitoramento", "TI — Videomonitoramento". |

> **Transparência (Art. 10, §2º):** a base de interesse legítimo é **informada ao titular** na política de privacidade e nos avisos de videomonitoramento nas lojas.

---

## 2. Necessidade

| Pergunta | Resposta |
|---|---|
| Os dados são adequados, pertinentes e limitados ao necessário? (Art. 6º, II e III) | **Sim.** Cobrança: apenas nome, CPF, valores em aberto e histórico de compras — **sem** dados de saúde, religião ou origem. Câmeras: **imagem captada apenas nas áreas de fluxo/estratégicas**; nunca em vestiários, banheiros ou caixas com cobertura de privacidade. Logs: metadados de rede, sem conteúdo de comunicação. |
| Por quanto tempo os dados são necessários? | Cobrança: até quitação ou prescrição (5 anos). Câmeras: 30 dias. Logs: 6 meses (12 em investigação). Ver [[../04-politicas/politica-retencao-descarte|Política de Retenção e Descarte]]. |
| Há dados desnecessários no fluxo? | **Não.** A minimização foi aplicada por desenho (privacy by design — Art. 46, §2º). |
| **Conclusão de necessidade** | **O tratamento é necessário e limitado ao mínimo.** |

---

## 3. Balanceamento

### 3.1 Interesses do controlador/terceiros

- Redução de perdas por fraude e furto (impacto financeiro direto e na competitividade de preços).
- Segurança física de clientes e colaboradores (dever de cuidado).
- Exercício regular de direito de crédito (Art. 7º, IX e X).

### 3.2 Impacto sobre os direitos e liberdades dos titulares

- **Cobrança:** impacto moderado (desconforto), mitigado por regras de contato ético.
- **Câmeras:** percepção de vigilância — expectativa razoável de privacidade nas áreas internas é preservada (não há captura em áreas íntimas).
- **Logs de TI:** impacto baixo (metadados, sem interceptação de conteúdo).

### 3.3 Juízo de proporcionalidade

| Fator | Análise |
|---|---|
| Severidade da interferência | Baixa a moderada, localizada, com mitigação por desenho |
| Expectativa razoável do titular | Atendida: sinalização e transparência ativa |
| Benefício esperado | Alto: redução de fraude, proteção patrimonial e de pessoas |
| Medidas menos intrusivas disponíveis | Não há alternativa de eficácia equivalente |

**RESULTADO DO BALANCEAMENTO: o interesse legítimo do controlador PREVALECE**, pois a interferência é limitada, transparente e não afeta o núcleo essencial dos direitos fundamentais dos titulares.

---

## 4. Salvaguardas

| Salvaguarda | Aplicação |
|---|---|
| **Minimização por desenho** | Apenas dados necessários; câmeras fora de áreas íntimas; logs sem conteúdo |
| **Transparência ativa** | Avisos de videomonitoramento; política de privacidade; informação sobre a base legal (Art. 10, §2º) |
| **Direito de oposição** | Canal do titular permite solicitar revisão do tratamento (Art. 18) |
| **Revisão humana** | Decisões de bloqueio/cobrança sempre validadas por humano (Art. 20) |
| **Segurança** | RBAC, criptografia, trilha de auditoria, [[../05-plano-de-resposta-a-incidentes/README|plano de resposta a incidentes]] (Art. 46) |
| **Retenção controlada** | Prazos definidos e descarte automático na política de retenção |
| **RIPD quando alto risco** | Uso de biometria facial avaliado em [[../02-ripd-relatorio-de-impacto/ripd-reconhecimento-facial|RIPD-2026-001]] |

---

## 5. Decisão e Monitoramento

**DECISÃO:** utilizar a base legal do **Art. 7º, IX (interesse legítimo)** para prevenção à fraude e segurança patrimonial, com as salvaguardas acima.

- [x] LIA revisado em 08/08/2026
- [ ] Revisar novamente quando: mudança de fluxo, incidente relevante, atualização de guia ANPD ou revisão anual (08/08/2027)

> **Nota de accountability:** este LIA está disponível para auditoria e para a ANPD (Art. 10, §3º e Art. 6º, IX). Não constitui aconselhamento jurídico — recomendada validação por assessoria legal.
