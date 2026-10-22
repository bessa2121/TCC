# Diário de Bordo

Este documento consolida os principais trabalhos realizados pelos colaboradores dos repositórios `TCC`, `tealearn-backend` e `tealearn-frontend`, com base nos commits, autores e atividades registradas.

Observação: os commits dos repositórios de frontend e TCC aparecem com autores e mensagens, mas nem sempre com data detalhada em um único retorno da API; por isso, a linha do tempo abaixo combina as datas confirmadas do backend com a contribuição geral observada nos demais repositórios.

## 1) Colaboradores e papéis principais

- `bessa2121` — responsável pela liderança técnica, arquitetura, backend, deploy, integração, autenticação, documentação e ajustes finais do projeto.
- `LeonardoBuso` — principal colaborador do repositório `TCC` e também contribuiu no frontend do projeto.
- `Fernandofiani` — contribuições pontuais no `TCC` e apoio no desenvolvimento do material do projeto.
- `ValeJesus` — contribuições em artefatos e ajustes no repositório `TCC`.
- `felipergomes19` — contribuições pontuais no `TCC`.
- `BryanLustri` — contribuições pontuais no `TCC`.

## 2) Resumo por repositório

### `bessa2121/tealearn-backend`
- Repositório principal da lógica de negócio do sistema.
- Desenvolvimento focado em autenticação, materiais, dashboard, PDF, integração com frontend, deploy e correções operacionais.
- Autor principal: `bessa2121`.

### `bessa2121/tealearn-frontend`
- Repositório do cliente web do sistema.
- Tempo de desenvolvimento concentrado em interface, consumo da API e experiência do usuário.
- Autores principais: `bessa2121` e `LeonardoBuso`.

### `bessa2121/TCC`
- Repositório de documentação e material acadêmico do projeto.
- Trabalho colaborativo com participação de vários membros do grupo.
- Contribuidores principais: `LeonardoBuso`, `bessa2121`, `ValeJesus`, `Fernandofiani`, `felipergomes19` e `BryanLustri`.

## 3) Diário de bordo por dia

### 2026-04-21
- `bessa2121`:
  - criação inicial dos repositórios `tealearn-backend` e `tealearn-frontend`;
  - início da estrutura do projeto e organização do desenvolvimento.

### 2026-05-04
- `bessa2121`:
  - organização inicial das dependências do backend;
  - preparação do ambiente para continuar a implementação.

### 2026-05-18
- `bessa2121`:
  - atualização de pendências e organização do backlog do projeto;
  - preparando o caminho para as próximas entregas técnicas.

### 2026-05-19
- `bessa2121`:
  - adicionou planejamento, dependências e configuração inicial para o backend;
  - movendo arquivos e estruturando o projeto para a próxima etapa de desenvolvimento;
  - alinhou a base do sistema com a ideia de produto e arquitetura inicial.

### 2026-05-20
- `bessa2121`:
  - implementou variáveis de ambiente e ajustes no `.gitignore`;
  - criou a base para usuários do banco e deixou o projeto pronto para evoluções posteriores.

### 2026-06-04
- `bessa2121`:
  - revisão de pendências e organização da próxima etapa de implementação.

### 2026-06-06
- `bessa2121`:
  - adicionou README e documentação inicial do repositório para facilitar uso e entendimento do projeto.

### 2026-06-08
- `bessa2121`:
  - implementou autenticação e camada de usuários no backend;
  - iniciou upload de materiais em PDF e extração de texto, etapa-chave para adaptação educacional.
- `LeonardoBuso` / `bessa2121` (no frontend):
  - desenvolvimento inicial da interface e integração com a API para evoluir a experiência do usuário.

### 2026-06-09
- `bessa2121`:
  - implementou adaptação de materiais com nível de suporte e exportação em PDF;
  - avançou na jornada do usuário, tornando o material educacional mais útil e personalizável.

### 2026-06-11
- `bessa2121`:
  - refinou o backend principal;
  - finalizou a parte central do sistema e documentou a API.

### 2026-06-12
- `bessa2121`:
  - adicionou logs estruturados e controle de erros;
  - ajustou status HTTP; melhorou a robustez do backend;
  - implementou rate limit básico e ajustes de segurança;
  - configurou ambiente e Docker do backend.

### 2026-06-14
- `bessa2121`:
  - ajustou CORS e configuração de segurança para integração com React e ambiente de desenvolvimento.

### 2026-06-16
- `bessa2121`:
  - implementou endpoints para dashboard de materiais;
  - iniciou ajustes de deploy com Docker e Railway;
  - centralizou variáveis de ambiente e melhorou configuração para publicação.

### 2026-06-17
- `bessa2121`:
  - corrigiu CORS, Swagger e configuração HTTPS/server para funcionar corretamente em produção;
  - ajustou problemas de deploy e roteamento da API.

### 2026-06-28
- `bessa2121`:
  - atualizou pendências e retomou a organização das tarefas do projeto.

### 2026-07-01
- `bessa2121`:
  - corrigiu PDF generator e navegador compatibility;
  - adicionou pendências e melhorias de layout e cabeçalho do documento exportado.

### 2026-07-02
- `bessa2121`:
  - ajustou dashboard com dados reais;
  - melhorou logs de produção e refinou a camada de visualização do sistema.

### 2026-07-03
- `bessa2121`:
  - melhorou cabeçalho do PDF;
  - adicionou logo e corrigi problemas no gerador de PDFs.

### 2026-07-06
- `bessa2121`:
  - atualizou a lista de pendências e manteve o projeto alinhado com objetivos de entrega.

### 2026-07-17
- `bessa2121`:
  - adicionou mais informações ao layout do PDF;
  - ajustou pendências e refinou aparência/funcionalidade do material gerado.

### 2026-08-14
- `bessa2121`:
  - corrige rate limit do sistema e ajusta o comportamento de segurança do backend.

## 4) Contribuição por membro no repositório TCC

A partir dos commits e contribuições registradas no repositório `TCC`:

- `LeonardoBuso` — maior volume de contribuições no TCC, com foco em estrutura, documentação e refinamento do material/pesquisa.
- `bessa2121` — contribuiu de forma consistente, com grande participação em organização, ações técnicas e alinhamento do projeto.
- `ValeJesus` — contribuições relevantes em ajustes e apoio ao material do TCC.
- `Fernandofiani` — contribuições pontuais no desenvolvimento e revisão do trabalho.
- `felipergomes19` — contribuições pontuais e apoio no material do TCC.
- `BryanLustri` — contribuições menores, porém registradas no histórico do repositório.

## 5) Conclusão

O projeto foi conduzido principalmente por `bessa2121`, que concentrou a liderança técnica, arquitetura, integração, deploy e refinamento do backend. O frontend teve participação ativa de `bessa2121` e `LeonardoBuso`, enquanto o repositório `TCC` recebeu uma contribuição coletiva, com `LeonardoBuso` como principal impulsionador e com vários membros colaborando em diferentes momentos.

Em resumo, a evolução do projeto foi definida por três pilares: desenvolvimento técnico do sistema, integração do produto com usuários e documentação acadêmica do trabalho.

---

Documento gerado para registro do progresso do grupo e de suas contribuições ao projeto.
