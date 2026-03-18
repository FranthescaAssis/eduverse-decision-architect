# EduVerse: Mini Projeto "O Arquiteto Decisor" (v4)

**Aluno:** Franthesca Assis Pereira 

**Matrícula:** 2321041

**Link do Repositório GitHub (Scaffolding):** https://github.com/FranthescaAssis/eduverse-decision-architect.git

---

## 🟢 CICLO 1: Visão e Requisitos (Fase 1)

### 1.1 Resumo do Cenário de Negócio
Uma instituição de ensino identificou a oportunidade de aplicar inteligência artificial ao mercado da educação online. O modelo educacional tradicional — baseado em conteúdos lineares e avaliações pontuais — não atende à diversidade de ritmos e estilos de aprendizagem dos estudantes, resultando em baixo engajamento e altas taxas de evasão. O sistema EduVerse propõe adaptar o ensino ao perfil individual de cada aluno, oferecendo trilhas de aprendizado personalizadas, avaliações dinâmicas e feedback instantâneo. A plataforma utilizará IA para identificar lacunas de conhecimento e recomendar conteúdos adequados, integrando-se a sistemas de gestão acadêmica (LMS) já existentes e sendo acessível em múltiplos dispositivos. Os usuários principais são: alunos (acesso às trilhas e avaliações), professores/tutores (criação e monitoramento de conteúdo) e administradores institucionais (gestão de usuários e relatórios).

### 1.2 Atributos de Qualidade (RNFs) Priorizados
1.  **Escalabilidade:** O sistema precisa suportar crescimento no número de usuários simultâneos, processar análises de dados em massa e incorporar atualizações tecnológicas sem reestruturação completa. Plataformas educacionais enfrentam picos de acesso em períodos de avaliação.
2.  **Performance:** Respostas lentas afetam diretamente a experiência de aprendizado e aumentam a taxa de abandono. A otimização do uso de recursos de hardware e a entrega eficiente de conteúdo multimídia são requisitos essenciais.
3.  **Manutenibilidade:** O motor de IA e as trilhas pedagógicas precisam evoluir continuamente. A arquitetura deve permitir atualização de módulos independentes sem impacto no restante do sistema, garantindo modularidade e qualidade de código.
4.  **Compatibilidade:** O EduVerse deve integrar-se com LMS externos (Moodle, Canvas) via padrões abertos (SCORM/xAPI) e operar corretamente nos principais navegadores e sistemas operacionais móveis, evitando dependência de tecnologia proprietária.
5.  **Usabilidade:** A interface deve ser intuitiva e acessível para perfis variados — do estudante do ensino médio ao docente universitário.                     Uma experiência fluida reduz a curva de aprendizado e contribui diretamente para a retenção dos usuários na plataforma.

### 1.3 Diagrama de Contexto (C4 Nível 1)
<img width="1200" height="860" alt="EduVerse_C4_Diagrama_Contexto" src="https://github.com/user-attachments/assets/788486ff-8123-48aa-a904-72f81e894336" />

Disponível em: https://github.com/FranthescaAssis/eduverse-decision-architect/blob/main/diagrams/EduVerse_C4_Diagrama_Contexto.png

### 1.4 Classificação da Estratégia
-   **Classificação:** [Conservadora / Balanceada / Ousada]
-   **Justificativa:** [Explique em 5 linhas o porquê desta escolha em relação ao risco, inovação e maturidade tecnológica. Referencie o Capítulo 1 do Pressman sobre a natureza do software, se pertinente].

---

## 🔵 CICLO 2: Blueprint e Decisões (Fase 2)
*Preencher e entregar no AVA ao final do Ciclo 2.*

### 2.1 Diagrama de Containers (C4 Nível 2)
[Insira aqui a imagem do seu Diagrama de Containers (C4 Nível 2). Este diagrama deve detalhar a estrutura interna do sistema, mostrando os principais containers (aplicações, bancos de dados, filas, etc.) e suas interações. **Recomendado: Salvar o diagrama em `/diagrams` no GitHub e referenciar o link da imagem aqui.**]

### 2.2 Estilo Arquitetural Escolhido
[Descreva o estilo arquitetural principal que você adotou (ex: Microsserviços, Monolito Modular, Hexagonal, Event-Driven) e justifique sua escolha com pelo menos 3 trade-offs reais (prós e contras) em relação aos RNFs priorizados na Fase 1. Referencie o Capítulo 14 do Pressman sobre estilos arquiteturais, se pertinente].

### 2.3 Architecture Decision Record (ADR) Principal
[Escolha uma decisão arquitetural crucial que você tomou nesta fase (ex: Escolha da Tecnologia de Persistência, Estratégia de Comunicação entre Microsserviços) e documente-a como um ADR. **Recomendado: Criar o arquivo `.md` do ADR em `/adrs` no GitHub e referenciar o link aqui.**]
-   **Título:** [Ex: Escolha da Tecnologia de Persistência]
-   **Contexto:** [O problema ou necessidade técnica que levou a essa decisão. Qual era o cenário?]
-   **Decisão:** [O que foi decidido. Qual tecnologia/abordagem foi escolhida?]
-   **Justificativa:** [Por que esta opção venceu as alternativas? Quais foram os trade-offs considerados? Quais os impactos nos RNFs?]

---

## 🔴 CICLO 3: Cloud e Resiliência (Fase 3)
*Preencher e entregar no AVA ao final do Ciclo 3.*

### 3.1 Estratégia de Cloud e Implantação
[Descreva como sua arquitetura será implantada em um ambiente de nuvem (ex: AWS, Azure, GCP). Qual o modelo de serviço (IaaS, PaaS, Serverless)? Como o sistema será escalado e monitorado?]

### 3.2 Análise de Fragilidade e Mitigação
-   **Ponto Frágil:** [Identifique a maior fraqueza ou risco da sua arquitetura em um cenário de produção (ex: falha de um serviço crítico, pico de tráfego inesperado, vulnerabilidade de segurança).]
-   **Mitigação:** [Como você minimizaria esse risco? Quais estratégias de resiliência (ex: circuit breaker, retry, fallback, multi-região) seriam aplicadas?]

### 3.3 Parecer Técnico Final
[Resumo executivo (até 10 linhas) defendendo por que sua arquitetura é a melhor escolha para o cliente, considerando os requisitos de negócio, os RNFs e a estratégia de implantação. Qual o valor agregado da sua solução?]

---

## 🏆 BÔNUS: Evolução Arquitetural (Gamificação)
*Opcional - Preencher apenas se houver melhoria estrutural documentada no GitHub.*

[Descreva brevemente a melhoria arquitetural que você implementou no seu repositório GitHub para fins de bônus de nota. Referencie a nova ADR e o diagrama atualizado (se houver) no GitHub. Ex: Migração de um componente para Serverless, implementação de um padrão de resiliência, otimização de custo em cloud. **Lembre-se: a melhoria deve ser arquitetural, não apenas textual.**]

---

## 📚 Referências Bibliográficas
-   **Pressman, R. S.** (2021). *Engenharia de Software: Uma Abordagem Profissional*. McGraw Hill. (Capítulos selecionados conforme o tema da aula).
-   **Richards, M., & Ford, N.** (2020). *Fundamentals of Software Architecture: An Engineering Approach*. O'Reilly Media.
-   **C4 Model for Software Architecture.** (s.d.). Disponível em: [https://c4model.com/](https://c4model.com/)
-   **Architecture Decision Records (ADRs).** (s.d.). Disponível em: [https://adr.github.io/](https://adr.github.io/)
