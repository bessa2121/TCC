# 🧠📚 NeuroLearn — Plataforma de Adaptação Didática com IA

> **Inteligência Artificial aplicada à educação inclusiva para estudantes com TEA**

---

# 🎯 Visão Geral

O **NeuroLearn** é uma plataforma que utiliza Inteligência Artificial para adaptar materiais didáticos tradicionais (PDFs, imagens, textos) em conteúdos mais acessíveis para alunos com Transtorno do Espectro Autista (TEA), especialmente no ensino médio.

A proposta é:

* Reduzir barreiras de compreensão
* Ajudar professores a adaptar conteúdos rapidamente
* Melhorar a experiência de aprendizagem de alunos neurodivergentes

---

# 🧩 Problema

Professores enfrentam dificuldades como:

* Falta de tempo para adaptar conteúdos
* Ausência de formação em educação inclusiva
* Materiais complexos e pouco acessíveis

Alunos com TEA enfrentam:

* Dificuldade com textos longos
* Problemas com linguagem abstrata
* Sobrecarga cognitiva

---

# 💡 Solução

O sistema:

* Recebe materiais didáticos
* Processa o conteúdo
* Aplica IA para simplificação
* Gera versões acessíveis
* Permite edição pelo professor
* Exporta conteúdo final

---

# 🏗 Arquitetura do Sistema

```mermaid
flowchart TD
    A[📥 Upload de Arquivo] --> B[📄 Extração de Texto]
    B --> C[🧹 Limpeza e Organização]
    C --> D[🧠 Divisão em Blocos]
    D --> E[🤖 Processamento com IA]
    E --> F[📝 Texto Adaptado]
    E --> G[🧠 Mapa Mental]
    F --> H[✏️ Edição pelo Professor]
    G --> H
    H --> I[📤 Exportação PDF]
```

---

# ⚙️ Stack Tecnológica

## 🔹 Backend

* Java + Spring Boot
* Spring Data JPA
* Lombok

## 🔹 Frontend

* React (interface simples)
* Axios

## 🔹 Banco de Dados

* MySQL (produção)
* H2 (desenvolvimento)

## 🔹 Processamento de Arquivos

* Apache PDFBox (PDF)
* Apache POI (DOCX)
* Tesseract OCR (imagens)

## 🔹 Inteligência Artificial

* API externa (GPT ou similar)

---

# 🔄 Fluxo Completo do Sistema

```mermaid
flowchart LR
    A[Professor] --> B[Upload]
    B --> C[Backend Spring]
    C --> D[Extração de Texto]
    D --> E[Limpeza]
    E --> F[Chunking]
    F --> G[IA API]
    G --> H[Resposta Adaptada]
    H --> I[Frontend]
    I --> J[Edição]
    J --> K[Exportação]
```

---

# 🎨 Pipeline de Processamento

```mermaid
flowchart TD
    A[Entrada] --> B{Tipo}
    B -->|PDF| C[PDFBox]
    B -->|Imagem| D[OCR]
    B -->|Texto| E[Direto]
    C --> F[Texto Unificado]
    D --> F
    E --> F
    F --> G[Limpeza]
    G --> H[Divisão em Partes]
    H --> I[IA]
    I --> J[Saída Estruturada]
```

---

# 👨‍💻 Separação de Equipe (5 pessoas)

## 🧠 Backend (2 pessoas)

Responsáveis por:

* API (Spring Boot)
* Integração com IA
* Processamento de arquivos
* Banco de dados

---

## 🎨 Frontend (2 pessoas)

Responsáveis por:

* Interface React
* Upload de arquivos
* Exibição de resultados
* Editor de texto

---

## 🔬 IA + Integração (1 pessoa)

Responsável por:

* Criação de prompts
* Testes de qualidade
* Controle de respostas
* Redução de alucinações

---

# 📅 Cronograma (Abril → Outubro)

```mermaid
gantt
    title Cronograma NeuroLearn
    dateFormat  YYYY-MM-DD
    section Base
    Setup do Projeto        :a1, 2026-04-09, 14d
    Upload de Arquivos      :a2, after a1, 14d

    section Processamento
    Extração de Texto       :b1, after a2, 21d
    Integração com IA       :b2, after b1, 21d

    section Inteligência
    Melhorias IA + Chunking :c1, after b2, 14d
    Perfis de Usuário       :c2, after c1, 14d

    section Funcionalidades
    Mapa Mental             :d1, after c2, 14d
    Editor                  :d2, after d1, 14d
    Exportação              :d3, after d2, 14d

    section Finalização
    UI/UX                   :e1, after d3, 14d
    Testes                  :e2, after e1, 14d
    Ajustes Finais          :e3, after e2, 14d
```

---

# 🧠 Estratégia de IA (Resumo)

* Uso de API pronta (sem treinar modelo)
* Prompt estruturado
* Chunking (dividir texto)
* Temperatura baixa
* Professor no controle final

---

# 🚀 Diferenciais do Projeto

* ✔ Adaptação automática com IA
* ✔ Foco em TEA nível 1
* ✔ Geração de mapa mental
* ✔ Edição humana (professor)
* ✔ Exportação em PDF
* ✔ Pipeline estruturado (nível profissional)

---

# 🏁 Objetivo Final

Criar uma plataforma funcional que:

* Seja utilizável por professores reais
* Reduza o tempo de adaptação de materiais
* Melhore a compreensão de alunos com TEA
* Demonstre aplicação prática de IA na educação

---

# 📌 Status do Projeto

🚧 Em desenvolvimento
📅 Prazo final: **20 de Outubro de 2026**
🎯 Meta: MVP funcional até **Julho/Agosto**

---

# 💬 Observação Final

> O foco não é apenas tecnologia, mas impacto educacional real.

---
