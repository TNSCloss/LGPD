
# Modelo de Relatório de Impacto à Proteção de Dados Pessoais (RIPD/DPIA)

> **Instruções de uso:** Substitua todos os campos entre `[colchetes]` pelos dados reais do tratamento avaliado. Remova ou marque as opções não aplicáveis. Documentos preenchidos devem ser persistidos em `.opencode/vault/privacy/` com identificador próprio e revisados sempre que houver mudança no fluxo do dado.

## 1. Informações Gerais

| Campo | Preenchimento |
|-------|---------------|
| Identificador do RIPD | `[EXEMPLO: RIPD-2026-001]` |
| Nome da operação de tratamento | `[Nome do sistema/processo]` |
| Controlador | `[Razão social, CNPJ, endereço]` |
| Encarregado (DPO) | `[Nome, e-mail, contato público]` |
| Data de elaboração | `[AAAA-MM-DD]` |
| Versão | `[1.0]` |
| Status | `[Rascunho / Em revisão / Aprovado / Arquivado]` |
| Responsável pelo preenchimento | `[Nome e cargo]` |
| Base legal principal | `[Art. 7º e/ou Art. 11 da LGPD — citar inciso]` |
| Motivo da elaboração | `[Legítimo interesse (Art. 10, §3º) / Solicitação da ANPD (Art. 38) / Tratamento de alto risco / Privacy by Design]` |

## 2. Escopo e Descrição do Tratamento

Descreva o **ciclo de vida completo do dado**: coleta, utilização, armazenamento, compartilhamento e descarte.

### 2.1 Finalidade do Tratamento

`[Qual objetivo legítimo, específico e explícito do tratamento? — Art. 6º, I da LGPD]`

### 2.2 Categorias de Dados Pessoais

| Tipo | Dados Tratados | Sensíveis? (Art. 5º, II) |
|------|----------------|--------------------------|
| Dados pessoais | `[Ex.: nome, e-mail, CPF]` | Não |
| Dados sensíveis | `[Ex.: dados de saúde, biométricos, orientação sexual]` | Sim |
| Dados de crianças/adolescentes | `[Sim/Não — aplicar Art. 14]` | — |

### 2.3 Titulares Afetados

- `[Ex.: colaboradores, clientes, usuários da plataforma, candidatos a vagas]`
- Volume estimado: `[Nº de titulares ou faixa]`
- Frequência do tratamento: `[Contínuo / Eventual / Por demanda]`

### 2.4 Sistemas e Tecnologias Utilizados

`[Sistemas, aplicações, nuvens, provedores e tecnologias (IA, profiling, automação de decisões, monitoramento em larga escala)]`

### 2.5 Compartilhamento e Transferências

| Destinatário | Finalidade | Natureza (Controlador/Operador) | Transferência Internacional |
|--------------|------------|--------------------------------|-----------------------------|
| `[Nome]` | `[Finalidade]` | `[Controlador/Operador]` | `[Sim/Não — mecanismo: adequação/SCC/BCR]` |

> **Nota 2026:** Transferências Brasil ⇆ União Europeia estão cobertas por reconhecimento de adequação mútua desde janeiro/2026 — não exigem SCCs/BCRs (Art. 33 da LGPD; Art. 45 do GDPR).

## 3. Avaliação de Necessidade e Proporcionalidade

| Pergunta | Resposta | Justificativa |
|----------|----------|---------------|
| O tratamento é necessário para atingir a finalidade? | `[Sim/Não]` | `[Justificativa]` |
| Há alternativa com menos dados (Minimização — Art. 6º, III)? | `[Sim/Não]` | `[Justificativa]` |
| O prazo de retenção é proporcional? | `[Sim/Não]` | `[Prazo e base normativa]` |
| É possível anonimizar ou pseudonimizar para reduzir risco? | `[Sim/Não]` | `[Justificativa]` |
| Os direitos dos titulares (Art. 18) são preservados? | `[Sim/Não]` | `[Como]` |
| A expectativa razoável do titular é respeitada? | `[Sim/Não]` | `[Justificativa]` |

### 3.1 Teste de Balanceamento (Legítimo Interesse — Art. 10, §3º)

- Interesse legítimo do controlador/terceiro: `[Descrever]`
- Impacto sobre direitos e liberdades dos titulares: `[Descrever]`
- Salvaguardas adotadas para proteger o titular: `[Descrever]`
- **Conclusão:** `[O interesse legítimo prevalece / Não prevalece]`

## 4. Identificação e Avaliação de Riscos

### 4.1 Matriz de Risco (Probabilidade × Impacto — ISO 31000 / ISO 27005)

| Probabilidade \ Impacto | Insignificante | Menor | Moderado | Crítico |
|------------------------|----------------|-------|----------|---------|
| **Rara** | Baixo | Baixo | Médio | Alto |
| **Possível** | Baixo | Médio | Alto | **Extremo** |
| **Provável** | Médio | Alto | **Extremo** | **Extremo** |
| **Quase certa** | Alto | Alto | **Extremo** | **Extremo** |

### 4.2 Registro de Riscos Identificados

| ID | Ameaça / Cenário | Probabilidade | Impacto | Nível de Risco | Decisão de Risco |
|----|------------------|---------------|---------|----------------|------------------|
| R-01 | `[Ex.: acesso não autorizado a dados sensíveis]` | `[Rara/.../Quase certa]` | `[Menor/.../Crítico]` | `[Baixo/.../Extremo]` | `[Aceitar/Mitigar/Transferir/Eliminar]` |
| R-02 | `[Ex.: vazamento por falha de segurança (Art. 48)]` | | | | |
| R-03 | `[Ex.: uso discriminatório de dados]` | | | | |
| R-04 | `[Ex.: perda ou corrupção de dados]` | | | | |
| R-05 | `[Ex.: dados inexatos/desatualizados]` | | | | |

> **Nível de risco:** Baixo = risco residual aceitável; Médio = requer monitoramento; Alto = requer mitigação; **Extremo = mitigação obrigatória antes do Go-Live**.

## 5. Plano de Ação e Controles de Mitigação

| ID do Risco | Controle Técnico | Controle Administrativo | Risco Residual | Responsável | Prazo |
|-------------|------------------|--------------------------|----------------|-------------|-------|
| R-01 | `[Ex.: criptografia, RBAC, MFA]` | `[Ex.: política de acesso, treinamento]` | `[Baixo/Médio]` | `[Nome]` | `[AAAA-MM-DD]` |
| R-02 | `[Ex.: DLP, monitoramento, resposta a incidentes]` | `[Ex.: plano de resposta, notificação ANPD]` | | | |
| R-03 | `[Ex.: revisão de algoritmos, vieses]` | `[Ex.: governança de IA, auditoria]` | | | |

### 5.1 Controles Recomendados (Mapeamento Multi-Framework)

| Framework / Norma | Controle / Cláusula | Diretriz Técnica |
|-------------------|--------------------|------------------|
| ISO/IEC 27701:2019 | Cláusula 7.2.5 | Formalizar procedimento de avaliação de impacto na privacidade antes do processamento de PII. |
| ISO/IEC 27001:2022 | Anexo A 5.8 | Segurança da Informação no Gerenciamento de Projetos: condicionar liberação de projetos à aprovação do RIPD. |
| ISO/IEC 27002:2022 | Controle 8.8 | Gestão de Vulnerabilidades: sanar falhas mapeadas no RIPD antes do Go-Live. |
| CIS Controls v8 | Controle 14.1 | Conscientização sobre privacidade para equipes de produto e arquitetura. |
| NIST CSF v2.0 | ID.RA-01 | Identificar e documentar ameaças/vulnerabilidades de privacidade na fase de design. |

### 5.2 Aceite de Risco Residual

| Risco Residual | Nível | Aceite Formal (Diretoria/Área solicitante) | Data | Assinatura |
|----------------|-------|---------------------------------------------|------|-----------|
| `[ID]` | `[Baixo/Médio]` | `[Sim/Não — nome do diretor]` | `[AAAA-MM-DD]` | |

> **Nota:** Riscos residuais que não podem ser sanados tecnicamente devem ser formalmente aceitos pelos diretores das áreas solicitantes, desonerando o DPO e a equipe de Segurança da Informação.

## 6. Aprovação e Monitoramento Contínuo

### 6.1 Parecer do Encarregado (DPO)

- **Parecer:** `[Favorável / Favorável com condicionantes / Desfavorável]`
- **Condicionantes:** `[Descrever]`
- **Data:** `[AAAA-MM-DD]`
- **Assinatura:** `[Nome]`

### 6.2 Aprovação da Gestão

| Papel | Nome | Decisão | Data | Assinatura |
|-------|------|---------|------|-----------|
| Controlador | | `[Prosseguir / Modificar / Cancelar]` | | |
| Data Owner | | `[Prosseguir / Modificar / Cancelar]` | | |

### 6.3 Gatilhos de Revisão

O RIPD deve ser **revisado** quando:

- [ ] Houver alteração na finalidade ou no fluxo do tratamento
- [ ] Houver mudança de base legal
- [ ] Novo sistema, tecnologia ou provedor for incorporado
- [ ] Novas categorias de dados (incluindo sensíveis) forem coletadas
- [ ] Incidente de segurança relevante ocorrer (Art. 48)
- [ ] Atualização de normas da ANPD ou de frameworks aplicáveis
- [ ] Periodicidade definida: `[Ex.: revisão anual — data: AAAA-MM-DD]`

## 7. Referências Normativas

- **LGPD (Lei 13.709/2018):** Art. 5º, II e XIX; Art. 6º; Art. 7º; Art. 10, §3º; Art. 11; Art. 14; Art. 18; Art. 38; Art. 46; Art. 48; Art. 52.
- **GDPR (Regulamento UE 2016/679):** Art. 35 (DPIA); Art. 36 (consulta prévia).
- **ISO/IEC 27701:2019:** Cláusula 7.2.5 — Avaliação de Impacto na Privacidade.
- **ISO/IEC 27005:2022 / ISO 31000:2018:** Gestão de riscos.
- **NIST CSF v2.0:** GV.RM (Risk Management Strategy) e ID.RA (Risk Assessment).
- **ANPD:** Guia Orientativo de RIPD; Resolução CD/ANPD nº 2/2022; Resolução CD/ANPD nº 15/2024.
- **GOV.BR (SGD/MGI):** Modelo simplificado de RIPD da Secretaria de Governo Digital.

## Anexos

- [ ] Registro das evidências coletadas (screenshots, diagramas de fluxo de dados, contratos)
- [ ] Diagrama de fluxo de dados (coleta → uso → armazenamento → compartilhamento → descarte)
- [ ] Política de privacidade correspondente ([[policies/index|Índice de Políticas]])
- [ ] Acordo de processamento (DPA) com operadores
- [ ] Relação com outros documentos: [[templates/index|Índice de Modelos e Templates]]
