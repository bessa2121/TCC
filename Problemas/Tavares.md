# Relatório Técnico: ConstruLink ODS
## Inovação Digital e Sustentabilidade na Construção Civil

---

## 1. Contextualização e Visão Geral do Projeto

O setor da construção civil atua como um dos pilares fundamentais da economia global, sendo o motor por trás da infraestrutura necessária para o desenvolvimento urbano. Contudo, essa vitalidade econômica é acompanhada por desafios críticos de eficiência operacional e sustentabilidade, com processos que frequentemente geram desperdícios sistêmicos. A integração estratégica da Tecnologia da Informação (TI) surge como o imperativo para mitigar essas falhas, alinhando o setor aos Objetivos de Desenvolvimento Sustentável (ODS) da ONU.

O projeto **ConstruLink ODS** é apresentado como uma plataforma Fullstack e um ecossistema IoT (Internet das Coisas) desenvolvido para centralizar a comunicação e a logística em canteiros de obras. O projeto, fundamentado em pesquisas conduzidas no **IFPB (Campus Campina Grande)** e no **IFRN (Campus João Câmara)**, foca no **ODS 9** (Indústria, Inovação e Infraestrutura) e no **ODS 12** (Consumo e Produção Responsáveis). Ao converter dados brutos em inteligência logística, a solução estabelece a base tecnológica para a transição definitiva em direção às Smart Cities. Esta análise detalha como a digitalização resolve as dores crônicas de um setor em busca de conformidade ESG.

---

## 2. Diagnóstico do Cenário Atual e Problemática

A gestão contemporânea de canteiros de obras sofre com uma severa fragmentação comunicativa. A dependência de processos manuais, como o uso indiscriminado de WhatsApp, planilhas isoladas e e-mails, cria gargalos que resultam em erros de orçamento, compras excessivas, atrasos crônicos e falta de rastreabilidade de insumos.

Mais crítico do que o desperdício financeiro é o impacto ambiental: o monitoramento global indica que a geração de resíduos eletrônicos (e-lixo) — cada vez mais presentes na infraestrutura de construção moderna — saltou de **33,8 milhões de toneladas em 2010** para uma projeção alarmante de **74 milhões de toneladas até 2030**.

A manutenção do status quo é inviável, especialmente considerando que o descarte inadequado de componentes eletrônicos libera metais pesados como **Chumbo, Mercúrio e Cádmio**, que causam danos severos ao sistema nervoso e aos ecossistemas. Em cidades como Campina Grande-PB, o diagnóstico de campo revela uma lacuna entre a consciência ambiental e a ação prática. O ConstruLink ODS foi projetado para preencher esse vazio, transformando a gestão de resíduos e logística em um processo auditável, reduzindo o impacto tóxico e os custos operacionais que hoje drenam a rentabilidade das empresas.

---

## 3. Arquitetura da Solução e Funcionalidades Críticas

O ConstruLink ODS propõe a transição do *"caos das mensagens perdidas"* para um *"fluxo inteligente"* de dados. A plataforma funciona como um hub integrado onde a visibilidade em tempo real é a prioridade. Seus diferenciais estratégicos incluem:

**Dashboards Personalizados**
Interface desenvolvida em React.js com segmentação por perfis (Cliente, Empresa, Colaborador e Fornecedor), permitindo tomadas de decisão baseadas em dados precisos de inventário.

**Segurança IoT e Notificações**
Utilizando microcontroladores ESP32, a solução integra um sistema de detecção de obstáculos (com sensores ultrassônicos e sinal vibratório) para aumentar a segurança do colaborador no canteiro, comunicando alertas via Firebase em tempo real.

**Rastreabilidade via RFID**
Implementação de módulos RFID-RC522 para o controle de procedência e localização de insumos sob o piso ou em estoque, garantindo que a logística reversa seja aplicada com precisão.

**Integração Automatizada**
Uso do serviço Nodemailer para eliminar falhas de comunicação com fornecedores, automatizando pedidos de compra e confirmações de entrega (*"Em Trânsito"*, *"Aprovado"*).

Essa robustez funcional diferencia o sistema ao unir a gestão de software de alto nível com o controle físico do canteiro através do hardware.

---

## 4. Especificações Tecnológicas e Infraestrutura de Dados

A escolha da stack tecnológica justifica-se pela necessidade de alta disponibilidade e sincronização instantânea em ambientes de mobilidade. A arquitetura abandonou modelos tradicionais de bancos locais (como MySQL) em favor de uma estrutura em nuvem mais ágil e escalável.

| Componente     | Tecnologia                  | Função Estratégica                                                    |
|----------------|-----------------------------|-----------------------------------------------------------------------|
| Frontend       | React.js / Bootstrap        | Interface responsiva focada em UX/UI, prototipada em Figma.           |
| Backend        | Java                        | Ambiente de execução para regras de negócio e APIs REST.              |
| Persistência   | MySQL/PostgreSQL            | Banco de dados em tempo real para notificações e autenticação segura. |
| Hardware/IoT   | ESP32 / C++ (Arduino)       | Microcontroladores para sensores de segurança e leitura de tags RFID. |
| Energia        | Baterias 3.7V / Reguladores | Autonomia para dispositivos portáteis de rastreamento e segurança.    |

O desenvolvimento seguiu a **Cultura Maker** e a abordagem **STEAM**, utilizando prototipagem rápida e impressão 3D para as carcaças dos dispositivos. Esse processo garante que a evolução do software acompanhe a robustez do hardware necessário no campo.

---

## 5. Viabilidade Operacional e Metodologia de Execução (Modelo ETEC)

O projeto possui uma estrutura pedagógica sólida, simulando o Ciclo de Vida de Desenvolvimento de Software (SDLC) real. Sob o **Modelo ETEC**, a execução é dividida entre **6 alunos** com papéis definidos: Frontend, Backend, Infraestrutura IoT, e Documentação/ODS. Esta colaboração simula as metodologias ágeis (Scrum) utilizadas no desenvolvimento do sistema E-Collect do IFPB.

A viabilidade técnica é classificada como **Alta**, dado que as ferramentas utilizadas (React/Node) são o padrão de mercado, e o custo de implementação do hardware (ESP32/Sensores) é reduzido, conforme validado pelas pesquisas do IFRN. A aplicação da metodologia ágil prepara a equipe para os desafios de integração de sistemas complexos, garantindo a entrega de um CRUD completo e regras de negócio funcionais que atendem aos requisitos de sustentabilidade moderna.

---

## 6. Alinhamento Estratégico com os Objetivos de Desenvolvimento Sustentável (ODS)

O ConstruLink ODS atua como um agente de transformação vinculado à **Agenda 2030**:

| ODS | Título | Contribuição |
|-----|--------|--------------|
| **ODS 9** | Indústria e Inovação | Promove a digitalização de uma infraestrutura tradicionalmente analógica, fomentando a inovação tecnológica no Brasil. |
| **ODS 12** | Consumo Responsável | Atende à Meta 12.5, reduzindo drasticamente o desperdício de materiais e e-lixo através da logística reversa inspirada no modelo E-Collect. |
| **ODS 3** | Saúde e Bem-Estar | Minimiza a exposição de trabalhadores e da população a substâncias tóxicas (Mercúrio, Cádmio) ao garantir o descarte correto de componentes. |
| **ODS 11** | Cidades Sustentáveis | Otimiza a gestão de resíduos urbanos e a segurança nos canteiros, pilares para o desenvolvimento de comunidades resilientes. |
| **ODS 4 e 10** | Educação e Igualdade | Fomenta a formação técnica profissional e utiliza tecnologias assistivas para garantir autonomia e inclusão no ambiente de trabalho. |

---

## 7. Pitch de Mercado e Considerações Finais

O ConstruLink ODS entrega uma solução definitiva para a gestão da construção civil: elimina o caos comunicativo, garante precisão orçamentária e estabelece transparência total sobre o impacto ambiental de cada obra. Através da união entre o poder do desenvolvimento Fullstack e a precisão do IoT, a plataforma permite *"construir as cidades do futuro, um clique por vez"*.

O veredito de viabilidade é incontestável: trata-se de uma proposta técnica e pedagógica robusta, enraizada na excelência acadêmica do IFPB e IFRN. Ao harmonizar a eficiência produtiva com a preservação ambiental e a saúde pública, o ConstruLink ODS prova que a tecnologia é a ponte essencial para um progresso que não compromete as gerações futuras.
