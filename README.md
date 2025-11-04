# BMAD - ARTHUR LUCENA

# O que é?
BMAD faz parte um novo paradigma conhecido como *Desenvolvimento Agentic*, avança significativamente essa capacidade, promovendo os LLMs de assistentes passivos para membros ativos e especializados de uma equipe virtual. O desenvolvimento agentic baseia-se na orquestração de múltiplas IAs, cada uma personificando uma função especializada (como Arquiteto, Scrum Master ou QA), que trabalham de forma colaborativa e sequencial. Este modelo exige uma imposição rigorosa de estrutura e governança sobre a natureza inerentemente flexível e por vezes inconsistente dos LLMs, garantindo a qualidade e a reprodutibilidade do código em escala de produção. A adoção de frameworks como o BMAD (Breakthrough Method of Agile AI-Driven Development) reflete essa necessidade de impor ordem metodológica no caos potencial da geração de código por IA.

### BMAD: Definição, Acrônimo e Filosofia Central
O BMAD, acrônimo para _Breakthrough Method of Agile AI-Driven Development_, é um sistema de fluxo de trabalho (workflow) projetado para orquestrar o desenvolvimento de software através de múltiplos agentes de IA. Não é apenas uma ferramenta de codificação, mas um framework modular abrangente, baseado em uma interface de linha de comando (CLI), que simula a operação de equipes inteiras de desenvolvimento dentro do ambiente de desenvolvimento integrado (IDE) do engenheiro.   

A filosofia central que impulsiona o BMAD é encapsulada na diretriz **"Stop Prompting, Start Architecting"**. Este princípio sublinha que a produtividade e a qualidade não advêm de prompts conversacionais longos e genéricos, mas sim da estruturação do problema. O método exige que o esforço se concentre inicialmente na decomposição rigorosa do problema em seus princípios fundamentais, na incorporação de expertise em agentes especializados, e na subsequente codificação desses _insights_ iniciais em artefatos explícitos e duráveis, como Documentos de Requisitos do Produto (PRDs) e especificações de arquitetura. Esses documentos se tornam a fonte de verdade e o contexto primário para todos os agentes subsequentes.   

É fundamental diferenciar esta metodologia de IA de outros softwares que compartilham o acrônimo. O BMAD de que se trata neste relatório não tem relação com o _Bmad Software Toolkit for Charged-Particle and X-Ray Simulations_ da Cornell University, um kit de ferramentas focado em simulações de partículas carregadas e raios-X.   A estrutura de funcionalmente é dividida em quatro fases críticas que se assemelham a um acrônimo descritivo: **Briefing, Modelagem/Arquitetura, Automação/Dev, e Dados/QA**. A força do método reside em exigir artefatos estruturados para cada uma dessas fases, estabelecendo assim uma base sólida para o desenvolvimento agentic durável. 

O sistema é construído sobre o **BMad CORE**, que atua como o framework central e aloja o Agente Mestre responsável pela orquestração primária.

1. **BMad Method (BMM):** Este é o coração da metodologia de desenvolvimento. Ele contém o conjunto de agentes e fluxos de trabalho que implementam o ciclo ágil completo. Inclui 12 agentes especializados e 34 workflows definidos.   
    
2. **BMad Builder (BMB):** Módulo focado na construção e otimização, contendo 1 agente e 7 workflows.   
    
3. **Creative Intelligence Suite (CIS):** Este módulo é dedicado à inteligência criativa e análise, incluindo 5 agentes e 5 workflows específicos.

# O que resolve?

O BMAD foi concebido para mitigar os principais pontos de fricção no desenvolvimento de software, especialmente aqueles exacerbados pelo uso não estruturado de Large Language Models.

O método BMAD transforma o processo de desenvolvimento em um ciclo ágil repetível que opera quase automaticamente após a fase inicial de planejamento. Isso se traduz diretamente em ganhos de produtividade e aceleração do _time-to-market_.   

A automação de funções chave e a organização do trabalho em painéis visuais (similar ao Kanban) garantem o que é descrito como "produtividade máxima". O sistema é capaz de reduzir drasticamente o tempo necessário para desenvolver software, transformando projetos que levariam meses em questão de dias. 

Para projetos complexos, especialmente aqueles que envolvem arquiteturas de microserviços, o BMAD é essencial. A metodologia garante que cada serviço independente, mesmo em repositórios separados, seja construído com a mesma disciplina e clareza, graças ao fluxo estruturado de artefatos. Essa abordagem assegura que a implementação final possa ser rastreada desde a visão inicial do produto até a entrega final do código, garantindo a coerência e o cumprimento dos objetivos estratégicos.
# Como instalar?
O BMAD é instalado como um pacote NPM, utilizando o comando `npx`. A escolha entre as versões estável e alpha depende da prioridade do projeto:

1. **Versão v6 Alpha (Recomendada):** A versão v6-alpha é a mais aprimorada, estando próxima da qualidade beta e sendo recomendada para novos projetos devido aos avanços metodológicos significativos em relação à versão anterior. O comando de instalação é:

```
npx bmad-method@alpha install
```

2. **Versão v4 Estável (Produção):** A versão v4 é a linha de base de produção, recomendada para ambientes que priorizam a estabilidade comprovada, embora possua funcionalidades mais limitadas que a v6. O comando é: 
```
npx bmad-method install
```

Após executar o comando de instalação, o usuário é guiado por um **Interactive Setup**.   

O instalador solicita informações críticas para a configuração do ambiente, incluindo:

- A definição do `Project Location` (local de instalação do projeto).
    
- A **Seleção Modular**, onde o usuário escolhe quais módulos deseja instalar (BMM, BMB, CIS ou todos), permitindo um ajuste fino das funcionalidades.   
    
- Configurações de personalização, como nome, idioma e opções específicas para desenvolvimento de jogos (se aplicável).
    
- A configuração automática de integração com as IDEs suportadas (Claude Code, Cursor, Windsurf, VS Code).   
    

A instalação cria uma estrutura de pasta unificada e limpa denominada `bmad/` dentro do diretório do projeto, onde residem os componentes principais.

|**Diretório**|**Conteúdo**|**Importância**|
|---|---|---|
|`core/`|Framework central + BMad Master agent|Base de orquestração do sistema.|
|`bmm/`|BMad Method (12 agentes, 34 workflows)|Implementação da metodologia ágil.|
|`bmb/`|BMad Builder (1 agente, 7 workflows)|Foco na construção e utilitários.|
|`cis/`|Creative Intelligence (5 agentes, 5 workflows)|Módulo de inteligência criativa/análise.|
|`_cfg/`|Personalizações do usuário|Garante que modificações personalizadas (como arquivos de agente `qa.md` ou `sm.md`) sobrevivam a atualizações do framework, permitindo a persistência e a extensibilidade da lógica dos agentes.[6, 7]|

# Como funciona?

O BMAD funciona transformando o ciclo de desenvolvimento de software em uma "linha de montagem metódica". A chave para o seu sucesso é a utilização de agentes especializados que operam em sequência, onde a saída estruturada (_output_) de um agente se torna a entrada contextualizada (_input_) para o agente seguinte.

O fluxo de trabalho central do BMAD simula uma equipe ágil completa, envolvendo seis papéis de agente críticos que garantem que cada fase do desenvolvimento seja tratada por um especialista em IA dedicado.

### Workflow Sequencial:

| **Fase**            | **Agente**           | **Foco Operacional e Função**                                | **Ação/Comando Chave**                             | **Artefato de Saída Principal**                 |
| ------------------- | -------------------- | ------------------------------------------------------------ | -------------------------------------------------- | ----------------------------------------------- |
| **1. Iniciação**    | Analyst              | Define domínio, valor e pesquisa inicial.                    | `*workflow-init` (início) / `create-project-brief` | `brief.md` (Resumo do Projeto)                  |
| **2. Definição**    | Product Manager (PM) | Estabelece o _O Quê_ (escopo, requisitos, MVP).              | `create PRD`                                       | `prd.md` (Requisitos do Produto)                |
| **3. Modelagem**    | Architect            | Estabelece o _Como_ (design técnico, _stack_).               | _Design System Architecture_                       | `architecture.md` (Design de Sistema)           |
| **4. Planejamento** | Scrum Master (SM)    | Orquestração da Sprint, Decomposição do Contexto (Sharding). | `sharddoc`, `createEpic`, `draft`                  | Epics e User Stories detalhadas e sequenciadas. |
| **5. Execução**     | Developer (Dev)      | Implementação e codificação da funcionalidade.               | _Code Implementation_                              | Código fonte, Modificações de Repositório.      |
| **6. Qualidade**    | QA Agent             | Validação da conformidade com requisitos e padrões.          | `QAMDC.file` (revisão) / _Review and Validate_     | Status de _Done_, Relatórios de Teste.          |
É fundamental notar que, apesar do alto nível de automação, o BMAD não é uma caixa preta autônoma. Ele opera como um **co-piloto de governança**, onde o controle humano é exigido em pontos críticos para mitigar o risco de alucinações de IA em fases estratégicas.

O ponto de intervenção mais significativo ocorre após a fase de Planejamento. O Scrum Master gera as histórias de usuário detalhadas, mas o processo exige a **aprovação manual** dessas histórias antes que o trabalho seja liberado para o Agente Developer. Isso garante que as decisões críticas sobre o que deve ser construído (_o que construir agora_) e o alinhamento com a estratégia do produto permaneçam sob o controle do Product Owner ou Technical Lead humano.

- Exemplo de caso de uso: https://gemini.google.com/share/b59b8e408c89
