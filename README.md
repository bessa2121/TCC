# Portaria Digital — MVP

Sistema web de **controle de acesso para condomínios residenciais**, desenvolvido como Trabalho de Conclusão de Curso (TCC) na ETEC.  
O projeto digitaliza o registro de visitantes na portaria, permitindo que moradores autorizem entradas em tempo real e síndicos consultem históricos.

---

## 🚪 Problema

A maioria dos condomínios ainda utiliza **cadernos físicos** para registrar visitantes, sem rastreabilidade digital.  
Isso gera falhas graves de segurança:

- Morador não sabe quem entrou
- Síndico não tem relatórios
- Registros podem ser perdidos ou adulterados

> **68 milhões de brasileiros** vivem em condomínios — o mercado potencial é enorme.

---

## 🎯 Objetivo

Construir um sistema web que permita:

- Registro digital de visitantes com foto
- Notificação em tempo real ao morador
- Autorização ou recusa de entrada pelo sistema
- Histórico consultável de acessos para o síndico

---

## 👥 Perfis de Usuário

- **Porteiro** → registra visitantes e saída
- **Morador** → autoriza ou recusa entrada
- **Síndico** → consulta histórico completo

---

## 🛠️ Stack Tecnológica

- **Frontend:** React 18, React Router, Axios, SockJS + StompJS, Context API  
- **Backend:** Spring Boot 3, Spring Security + JWT, WebSocket STOMP, Spring Data JPA, JavaMailSender  
- **Banco:** MySQL 8 + Flyway migrations  

---

## 📐 Escopo do MVP

- Login com JWT  
- Cadastro de moradores, unidades e porteiros  
- Registro de visitantes com foto via webcam  
- Notificação em tempo real ao morador (WebSocket)  
- Autorização/recusa pelo morador  
- Histórico consultável pelo síndico  

> **Critério de sucesso:** ciclo completo funcionando de ponta a ponta.

---

## 🗂️ Banco de Dados

Principais tabelas:

- `USUARIOS` (moradores, porteiros, síndico)  
- `UNIDADES` (bloco, número, morador vinculado)  
- `VISITANTES` (dados pessoais + foto)  
- `REGISTROS_ACESSO` (entrada, saída, decisão)  
- `CONSENTIMENTOS_LGPD` (prazo de retenção e consentimento explícito)

---

## 🔌 API REST

### Autenticação
- `POST /auth/login` → retorna JWT  
- `POST /auth/logout` → invalida token  

### Usuários e Unidades
- `GET /usuarios` → lista usuários (síndico)  
- `POST /usuarios` → cria morador ou porteiro  
- `GET /unidades` → lista unidades  
- `POST /unidades` → cria unidade  

### Visitantes
- `POST /visitantes` → cria visitante + upload foto  
- `GET /visitantes/{id}` → busca visitante  

### Registros de Acesso
- `POST /acessos` → registra entrada  
- `PUT /acessos/{id}/autorizar` → morador autoriza  
- `PUT /acessos/{id}/recusar` → morador recusa  
- `PUT /acessos/{id}/saida` → porteiro registra saída  
- `GET /acessos` → histórico com filtros (síndico)  
- `GET /acessos/minha-unidade` → histórico do morador  
- `GET /acessos/{id}` → detalhe de um registro  

---

## 📅 Roadmap (Sprints)

1. **Sprint 1 (Semanas 1-6):** autenticação, cadastros e banco  
2. **Sprint 2 (Semanas 7-12):** registro de visitante e captura de foto  
3. **Sprint 3 (Semanas 13-18):** WebSocket e decisão do morador  
4. **Sprint 4 (Semanas 19-24):** histórico, ajustes e demo final  

---

## 👨‍💻 Divisão do Time

- **M1 (Back-end Tech Lead):** Spring Boot, Security, JWT  
- **M2 (Back-end):** WebSocket, endpoints de acesso, upload de foto  
- **M3 (Front-end Porteiro):** formulário, webcam, SockJS/StompJS  
- **M4 (Front-end Morador/Síndico):** notificações, histórico, filtros  
- **M5 (Banco + QA + Docs):** modelagem, migrations, documentação, demo  

---

## ⚖️ Conformidade LGPD

- Consentimento explícito obrigatório  
- Finalidade declarada: "imagem usada exclusivamente para controle de acesso"  
- Prazo de retenção: 90 dias (`expira_em`)  
- Direito à exclusão: `DELETE /visitantes/{id}` remove foto e dados pessoais  

---

## ⚠️ Riscos e Mitigações

- **WebSocket instável na demo:** usar localhost + vídeo backup  
- **Sprint 3 atrasar:** iniciar config WS no fim da Sprint 2  
- **Câmera não funcionar:** testar ambiente antecipadamente  
- **Escopo crescer:** só após ciclo completo funcional  
- **Divisão desigual de trabalho:** contrato de interface na semana 1  

---

## 📽️ Pitch

> *"68 milhões de brasileiros vivem em condomínios. A maioria confia sua segurança a um caderno de papel.  
> Nossa solução digitaliza a portaria: o porteiro registra o visitante com foto, o morador autoriza em tempo real, e o síndico consulta o histórico completo.  
> É a segurança que o condomínio já deveria ter — simples, acessível e sem custo de hardware especializado."*

---

## 🚀 Status

- MVP em desenvolvimento  
- Prazo total estimado: **6 meses**  
- Entrega final: **demo ao vivo + vídeo backup**
