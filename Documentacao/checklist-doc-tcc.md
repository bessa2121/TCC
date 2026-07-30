# Checklist para TCC - Relatório Técnico (Manual CPS Etecs 2022)

Este checklist foi ajustado especificamente para a modalidade de **Relatório Técnico**, ideal para TCCs de desenvolvimento de software, projetos práticos e solução de problemas técnicos nas Etecs do Centro Paula Souza (CPS).

---

## 1. Normas Gerais e Formatação ABNT (Padronização CPS)

### Configurações de Página e Texto
- [ ] **Papel:** Formato A4 (21 cm x 29,7 cm), cor branca ou reciclada, impresso em apenas uma face.
- [ ] **Fonte:** Arial ou Calibri (utilizar a mesma em todo o trabalho).
- [ ] **Tamanho da Fonte:**
  - `12 pt` para texto principal, títulos e subseções.
  - `10 pt` para citações longas (mais de 3 linhas), notas de rodapé, paginação, fontes e legendas de figuras/tabelas/códigos.
- [ ] **Margens:**
  - Superior: `3 cm`
  - Esquerda: `3 cm`
  - Inferior: `2 cm`
  - Direita: `2 cm`
- [ ] **Espaçamento entre linhas:**
  - `1,5` no texto principal.
  - `Simples` para: citações longas, notas de rodapé, resumo, referências e legendas de ilustrações/tabelas/código.
  - Espaço entre parágrafos: Antes `0 pt`, Depois `6 pt`.
- [ ] **Paginação:**
  - Contada a partir da Folha de Rosto.
  - Numerada em algarismos arábicos no canto superior direito a partir da **primeira folha da parte textual (Introdução)**.

---

## 2. Checklist do Relatório Técnico

### 2.1 Elementos Pré-textuais
- [ ] **Capa** (Obrigatório)
  - [ ] Nome da Instituição e da Unidade de Ensino (Etec)
  - [ ] Nome do Curso (ex: Técnico em Desenvolvimento de Sistemas)
  - [ ] Nome do(s) Autor(es)
  - [ ] Título do Projeto (e Subtítulo, se houver)
  - [ ] Local (Cidade da escola)
  - [ ] Ano de entrega
- [ ] **Folha de Rosto** (Obrigatório)
  - [ ] Nome do(s) Autor(es)
  - [ ] Título e Subtítulo
  - [ ] Nota Explicativa (Relatório Técnico apresentado ao curso X da Etec Y como requisito parcial para obtenção do título de técnico...)
  - [ ] Nome do Professor Orientador
  - [ ] Local e Ano
- [ ] **Resumo em Língua Portuguesa** (Obrigatório)
  - [ ] Parágrafo único, voz ativa, em 3ª pessoa.
  - [ ] Breve descrição do problema, do software/projeto desenvolvido e dos resultados.
  - [ ] Palavras-chave ao final (de 3 a 5 termos).
- [ ] **Listas Opcionais / Recomendadas:**
  - [ ] Lista de Ilustrações (telas do sistema, diagramas de caso de uso, ER, etc.)
  - [ ] Lista de Tabelas
  - [ ] Lista de Abreviaturas, Siglas e Símbolos
- [ ] **Sumário** (Obrigatório) — Alinhado à esquerda, sem contar os elementos pré-textuais.

---

### 2.2 Elementos Textuais

#### 1. Introdução
- [ ] **Contextualização e Delimitação do Problema:** Explicação clara da dor/problema que a empresa ou sociedade enfrenta.
- [ ] **Justificativa:** Por que é importante resolver esse problema e qual o impacto da solução tecnológica.
- [ ] **Objetivos:**
  - [ ] **Objetivo Geral:** O que o projeto/software se propõe a fazer.
  - [ ] **Objetivos Específicos:** Etapas técnicas para alcançar o objetivo (ex: mapear requisitos, modelar banco de dados, desenvolver a interface, realizar testes).
- [ ] **Metodologia:** Tecnologias, linguagens, frameworks, banco de dados e metodologias (Agile/Scrum, Kanban) utilizadas no desenvolvimento.

#### 2. Desenvolvimento e Implementação da Solução
- [ ] **Levantamento de Requisitos e Modelagem:**
  - [ ] Requisitos Funcionais e Não Funcionais.
  - [ ] Diagramas técnicos (Caso de Uso, Entidade-Relacionamento, Fluxogramas, etc.).
- [ ] **Arquitetura e Telas da Aplicação:**
  - [ ] Apresentação e explicação das telas/interfaces do sistema.
  - [ ] Fluxo de navegação do usuário.
- [ ] **Validação Técnica e Código:**
  - [ ] Inclusão e explicação de trechos chave de código (scripts, rotas, regras de negócio ou EULA).
  - [ ] Testes realizados (testes de unidade, usabilidade ou de desempenho) e correção de falhas.
- [ ] **Análise Mercadológica / Comparações:**
  - [ ] Comparativo técnico da sua solução em relação a concorrentes ou soluções existentes.

#### 3. Considerações Finais / Conclusão
- [ ] Síntese dos resultados técnicos alcançados.
- [ ] Avaliação se o software/projeto atendeu ao problema proposto na Introdução.
- [ ] Limitações encontradas durante o desenvolvimento e propostas de melhorias futuras.

---

### 2.3 Elementos Pós-textuais
- [ ] **Referências** (Obrigatório) — Fontes teóricas, documentações de linguagens/frameworks e artigos consultados (ordenadas alfabeticamente no sistema Autor-Data).
- [ ] **Apêndices** (Opcional) — Documentos ou tabelas produzidos por você (ex: questionário de testes de usabilidade aplicado aos usuários).
- [ ] **Anexos** (Opcional) — Documentos externos (ex: manuais de APIs de terceiros utilizadas no projeto).

---

## 📌 Guia Rápido: Padrão ABNT/CPS para Ilustrações e Tabelas

### 1. Na Lista de Ilustrações (Elemento Pré-textual)
* Não coloque apenas nomes soltos (ex: "Diagrama MER").
* Formato correto: **[Tipo] [Número] – [Título descritivo] ..... [Página]**
* *Exemplo:* `Figura 1 – Modelo Entidade-Relacionamento (MER) conceitual ..... 15`

### 2. No Corpo do Texto (Onde a imagem aparece)
* **Topo da Imagem:** Categoria + Número + Título.
* **Abaixo da Imagem:** Fonte de origem.
* *Exemplo:*
  * **Figura 1 – Modelo Entidade-Relacionamento (MER) conceitual**
  * *(Imagem do Diagrama)*
  * **Fonte:** Elaborado pelos autores (2026).

### 3. Chamada de Imagem no Texto
* Nenhuma imagem pode ficar "solta" sem ser citada na explicação.
* *Exemplo no parágrafo:* *"Para representar a estrutura do banco de dados, foi elaborado o modelo conceitual, conforme apresentado na **Figura 1**."*