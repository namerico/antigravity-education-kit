# Antigravity Kit - Edição Educação

Bem-vindo ao **Antigravity Kit - Edição Educação**, uma adaptação da arquitetura modular do Antigravity Kit original, projetada especificamente para revolucionar o processo de ensino-aprendizagem.

Este kit fornece uma estrutura robusta para criar assistentes de IA educacionais altamente especializados, capazes de atuar como tutores, criadores de conteúdo, avaliadores e orquestradores em diversas áreas do conhecimento.

## 🚀 Como Instalar e Usar

Para utilizar o **Antigravity Education Kit** em seu ambiente de desenvolvimento ou integrá-lo ao seu assistente de IA, siga os passos abaixo:

### 1. Pré-requisitos
Certifique-se de ter o [Git](https://git-scm.com/) instalado em sua máquina.

### 2. Clonar o Repositório
Abra o terminal e execute o comando para clonar o projeto:
```bash
git clone https://github.com/namerico/antigravity-education-kit.git
```

### 3. Estrutura de Uso
Este framework é baseado em arquivos Markdown que definem o comportamento dos agentes. Para "instalar" em um sistema de IA (como o Manus ou outros agentes baseados em arquivos de sistema):

1.  **Copie a pasta `.agent/`** para o diretório raiz do seu projeto de IA.
2.  **Configure o Orquestrador:** Aponte seu agente principal para ler as instruções em `.agent/agents/orquestrador-educacional.md`.
3.  **Carregue as Skills:** Certifique-se de que o sistema de IA tenha acesso à pasta `.agent/skills/` para que os agentes possam "equipar" os conhecimentos necessários.

### 4. Visualização Web
O projeto inclui uma interface de apresentação que pode ser visualizada localmente:
1. Navegue até a pasta `docs/`.
2. Abra o arquivo `index.html` em seu navegador preferido.

---

## 🧠 O que é o Antigravity Kit Educação?

É um framework que organiza a inteligência artificial em três componentes principais:

1.  **Agentes (`.agent/agents/`):** Personas de IA com funções específicas no ecossistema educacional (ex: Tutor Personalizado, Avaliador de Aprendizagem).
2.  **Habilidades (`.agent/skills/`):** Módulos de conhecimento que os agentes podem "equipar" conforme a necessidade. Incluem tanto habilidades pedagógicas (ex: Design Instrucional) quanto conhecimentos de domínio (ex: Matemática Fundamental, Ciências Humanas).
3.  **Fluxos de Trabalho (`.agent/workflows/`):** Procedimentos passo a passo que coordenam múltiplos agentes para realizar tarefas complexas (ex: Criar um Plano de Estudo Personalizado).

## 📂 Estrutura do Projeto

```text
antigravity-education-kit/
├── .agent/
│   ├── agents/
│   │   ├── avaliador-de-aprendizagem.md
│   │   ├── criador-de-conteudo-didatico.md
│   │   ├── orquestrador-educacional.md
│   │   └── tutor-personalizado.md
│   ├── skills/
│   │   ├── adaptacao-linguistica/
│   │   ├── artes/
│   │   ├── avaliacao-de-conhecimento/
│   │   ├── avaliacao-formativa/
│   │   ├── ciencias-da-natureza/
│   │   ├── ciencias-humanas/
│   │   ├── comunicacao-eficaz/
│   │   ├── curadoria-de-conteudo/
│   │   ├── design-instrucional/
│   │   ├── ingles-lingua-estrangeira/
│   │   ├── matematica-fundamental/
│   │   ├── motivacao-aluno/
│   │   ├── pedagogia/
│   │   ├── portugues-linguagens/
│   │   ├── producao-multimidia/
│   │   └── tecnologia-programacao/
│   └── workflows/
│       ├── criacao-material-didatico.md
│       ├── diagnostico-recuperacao-dificuldades.md
│       └── plano-de-estudo-personalizado.md
├── docs/                # Interface de apresentação (GitHub Pages)
└── README.md
```

## ⚙️ Como Funciona

1.  **O Orquestrador Recebe a Demanda:** O usuário (aluno ou professor) interage com o `orquestrador-educacional`, solicitando, por exemplo, ajuda para entender um conceito de física.
2.  **Delegação:** O Orquestrador aciona o `tutor-personalizado`.
3.  **Equipando Habilidades:** O Tutor "equipa" as habilidades `pedagogia`, `comunicacao-eficaz` e `ciencias-da-natureza`.
4.  **Execução:** O Tutor interage com o aluno, adaptando a explicação ao seu nível e estilo de aprendizagem.
5.  **Fluxos Complexos:** Para tarefas maiores, como criar um curso inteiro, o Orquestrador utiliza um *Workflow* para coordenar o Tutor, o Criador de Conteúdo e o Avaliador em uma sequência lógica.

## ✨ Vantagens desta Abordagem

*   **Especialização:** Cada agente foca no que faz de melhor, garantindo alta qualidade.
*   **Modularidade:** É fácil adicionar novas disciplinas (Habilidades) ou novos papéis (Agentes) sem alterar o sistema inteiro.
*   **Personalização:** A separação entre "como ensinar" (Pedagogia) e "o que ensinar" (Conteúdo) permite uma adaptação fina às necessidades de cada aluno.
*   **Escalabilidade:** Pode ser usado para tutorias individuais ou para gerenciar o currículo de uma escola inteira.

## 🤝 Como Contribuir

Para adicionar uma nova disciplina, crie uma nova pasta em `.agent/skills/` com um arquivo `SKILL.md` detalhando os princípios e tópicos chave daquela área. Para criar um novo processo, adicione um arquivo `.md` em `.agent/workflows/`.

---
© 2025 Antigravity Education Kit. Open Source sob licença MIT.
