---
title: Modelo de Comunicação à ANPD e aos Titulares (LGPD Art. 48)
date: 2026-08-08
tags: [lgpd, incidente, art-48, anpd, comunicacao, modelo, portfolio, supermercado10]
aliases: [Comunicação ANPD, Notificação de Incidente, Modelo Notificação ANPD]
status: approved
version: 1.0
owner: Encarregado de Dados (DPO)
framework: LGPD
related_docs:
  - playbook-resposta-incidente
  - modelo-registro-incidente
---

# Modelo de Comunicação à ANPD e aos Titulares

> Modelos prontos para preenchimento. Referência: Art. 48 da LGPD e **Res. CD/ANPD nº 15/2024** (notificação preliminar em **3 dias úteis**; complementar em **20 dias úteis**).

---

## A. Modelo de Notificação Preliminar à ANPD

*(Transcrito na plataforma de notificação da ANPD — com os dados do controlador e do encarregado)*

**Identificação do Controlador**
- Razão social: Supermercados 10 Comércio de Alimentos Ltda.
- CNPJ: 12.345.678/0001-90
- Encarregado: [Nome do Encarregado] — lgpd@supermercado10.com.br — +55 (11) 4000-1010

**1. Descrição do incidente**
Em **[data/hora]** foi identificado **[resumo: ex. acesso indevido a banco de dados do e-commerce com dados de clientes]**. A detecção ocorreu por **[meio: monitoramento/notificação de terceiro]**.

**2. Categorias e quantidade de titulares afetados**
**[ex.: ~40.000 titulares]** — categorias: **[clientes do e-commerce; colaboradores; candidatos]**.

**3. Categorias de dados pessoais envolvidos**
- Dados pessoais: nome, CPF, e-mail, telefone, endereço.
- Dados sensíveis: **[se aplicável: dados biométricos / financeiros]**.
- Dados de crianças e adolescentes: **[sim/não]**.

**4. Medidas técnicas adotadas**
- **[Isolamento do sistema, revogação de acessos, reset de senhas, bloqueio do vetor]**.
- **[Dados criptografados em repouso? Sim/Não — se sim: AES-256, chaves em KMS não comprometidas]**.
- **[Acionamento de forense digital / notificação aos operadores]**.

**5. Riscos aos titulares e medidas de tratamento**
- Riscos identificados: **[fraude financeira, phishing direcionado, exposição de dados]**.
- Medidas: **[monitoramento antifraude, orientação aos titulares, canal de atendimento]**.

**6. Medidas que serão ou já foram adotadas para reverter os efeitos**
**[Remediação da causa raiz, reforço de controles, revisão do RoPA]**.

---

## B. Modelo de Comunicação Complementar à ANPD (20 dias úteis)

**1. Atualização das informações preliminares**
- Nº do protocolo da notificação preliminar: ______
- Informações retificadas/acrescidas: ______

**2. Resultado das investigações**
- Causa raiz: ______
- Extensão real do incidente: ______
- Evidências de uso indevido dos dados: **[ex.: acessos não autorizados efetivados / não há indícios]**.

**3. Medidas corretivas definitivas**
- Ações técnicas: ______
- Ações administrativas (políticas, treinamento): ______
- Revisão de RoPA/RIPD: ______

**4. Dados complementares**
- Comunicação aos titulares realizada em: ______ (meio: ______)
- Autoridades adicionais notificadas: ______

---

## C. Modelo de Comunicação aos Titulares

*(Redação clara, sem juridiquês — remeter por e-mail/SMS/app conforme o caso)*

---

**Assunto:** Aviso importante sobre segurança dos seus dados — Supermercado 10

Olá, **[Nome]**,

Identificamos um incidente de segurança que pode ter envolvido os seus dados pessoais cadastrados no nosso **[site/app / programa Cliente 10]**. Estamos escrevendo para ser transparentes e para ajudar você a se proteger.

**O que aconteceu?**
Em **[data]**, **[resumo simples — ex.: um acesso não autorizado ao nosso cadastro de clientes]**.

**Quais dados podem ter sido afetados?**
**[ex.: nome, e-mail, telefone e, em alguns casos, CPF]**.

**O que estamos fazendo?**
Já **[contivemos o acesso, reforçamos nossos controles de segurança]** e notificamos a Autoridade Nacional de Proteção de Dados (ANPD), conforme exige a lei (LGPD — Art. 48).

**O que recomendamos que você faça?**
- Troque a senha do nosso site/app e de outros serviços que usem a mesma senha.
- **[Se aplicável: fique atento ao seu cartão e ao extrato; nosso parceiro financeiro pode emitir um novo cartão.]**
- Desconfie de e-mails, ligações ou SMS que peçam seus dados — **nunca enviamos solicitações de senha por esses canais**.
- Em caso de dúvida, fale conosco: **lgpd@supermercado10.com.br** ou **0800 400 1010**.

Nossos canais são os únicos oficiais. Lamentamos o ocorrido e reforçamos nosso compromisso com a proteção dos seus dados.

Equipe de Privacidade — Supermercado 10
**[Nome do Encarregado]** — Encarregado de Dados

---

## D. Modelo de Aviso no Site (quando necessário — casos de ampla repercussão)

```
[AVISO]
A Supermercado 10 informa que identificou [resumo]. As medidas de contenção foram adotadas
e a ANPD foi notificada. Clientes afetados estão sendo contatados diretamente. Dúvidas:
lgpd@supermercado10.com.br.
```

---

> **Regras de ouro:** (1) notificação ao titular **não substitui** a notificação à ANPD e vice-versa; (2) o titular deve receber **orientação prática de proteção**, não só a notícia; (3) nunca publique detalhes técnicos que ajudem atacantes; (4) o prazo de 3 dias úteis é contado da **confirmação** do incidente — não da detecção da suspeita.
