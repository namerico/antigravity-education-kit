```yaml
name: diagnostico-recuperacao-dificuldades
description: Identifica lacunas de aprendizagem em um aluno e propõe um plano de recuperação personalizado, coordenando o Avaliador de Aprendizagem e o Tutor Personalizado.
command: /orquestrador-educacional --workflow diagnostico-recuperacao-dificuldades
```

# Fluxo de Trabalho: Diagnóstico e Recuperação de Dificuldades

Este fluxo de trabalho é acionado quando um aluno apresenta dificuldades em um determinado tópico ou disciplina, ou quando um professor deseja identificar lacunas de aprendizagem. O **Orquestrador Educacional** coordena os agentes para diagnosticar o problema e propor um plano de recuperação eficaz.

## Fases do Fluxo de Trabalho

### Fase 1: Identificação da Dificuldade (Orquestrador Educacional)

1.  **Orquestrador Educacional** inicia o fluxo, solicitando ao usuário (aluno/professor) as seguintes informações:
    *   Tópico/Disciplina onde a dificuldade foi observada.
    *   Quais são os sintomas da dificuldade (ex: notas baixas, não consegue resolver exercícios, não entende conceitos).
    *   Qual o conhecimento prévio do aluno sobre o assunto.
    *   Qual o objetivo de recuperação (ex: passar na prova, dominar o conceito).
2.  **Orquestrador Educacional** utiliza a habilidade `comunicacao-eficaz` para interagir com o usuário e coletar detalhes.

### Fase 2: Diagnóstico da Lacuna de Aprendizagem (Avaliador de Aprendizagem)

1.  **Orquestrador Educacional** delega ao **Avaliador de Aprendizagem** a tarefa de diagnosticar a causa raiz da dificuldade.
2.  **Avaliador de Aprendizagem** utiliza a habilidade `avaliacao-de-conhecimento` para sugerir ou criar um instrumento de avaliação (ex: quiz, exercícios específicos) para o tópico.
3.  Após a aplicação do instrumento (pelo aluno, com supervisão do usuário), **Avaliador de Aprendizagem** utiliza a habilidade `analise-de-dados-educacionais` (implícita) para interpretar os resultados.
4.  **Avaliador de Aprendizagem** utiliza a habilidade `diagnostico-de-dificuldades` (implícita) para identificar as lacunas de conhecimento e as possíveis causas.
5.  **Avaliador de Aprendizagem** retorna ao Orquestrador Educacional um relatório detalhado do diagnóstico, incluindo as lacunas identificadas.

### Fase 3: Elaboração do Plano de Recuperação (Tutor Personalizado)

1.  **Orquestrador Educacional** delega ao **Tutor Personalizado** a tarefa de elaborar um plano de recuperação com base no diagnóstico.
2.  **Tutor Personalizado** utiliza a habilidade `pedagogia` para definir estratégias de ensino específicas para as lacunas.
3.  **Tutor Personalizado** utiliza a habilidade `motivacao-aluno` para incluir elementos que engajem o aluno no processo de recuperação.
4.  **Tutor Personalizado** pode solicitar ao **Criador de Conteúdo Didático** (via Orquestrador) a criação ou curadoria de materiais específicos para as lacunas.
5.  **Tutor Personalizado** retorna ao Orquestrador Educacional o plano de recuperação detalhado.

### Fase 4: Consolidação e Acompanhamento (Orquestrador Educacional)

1.  **Orquestrador Educacional** consolida o plano de recuperação, que pode incluir novos materiais e atividades.
2.  **Orquestrador Educacional** apresenta o plano ao usuário, explicando as etapas e a importância do acompanhamento.
3.  **Orquestrador Educacional** pode agendar verificações periódicas com o **Avaliador de Aprendizagem** para monitorar o progresso do aluno.

## Agentes Envolvidos

*   **Orquestrador Educacional:** Coordenação geral, coleta de informações, consolidação, acompanhamento.
*   **Avaliador de Aprendizagem:** Diagnóstico de lacunas, análise de resultados.
*   **Tutor Personalizado:** Elaboração de estratégias de recuperação, motivação.
*   **Criador de Conteúdo Didático (opcional):** Criação/curadoria de materiais específicos.

## Habilidades Utilizadas

*   `comunicacao-eficaz`
*   `avaliacao-de-conhecimento`
*   `pedagogia`
*   `motivacao-aluno`
*   `curadoria-de-conteudo` (opcional)
*   `producao-multimidia` (opcional)
*   `adaptacao-linguistica` (opcional)

## Saída Esperada

Um relatório de diagnóstico das dificuldades de aprendizagem e um plano de recuperação personalizado, com sugestões de atividades, materiais e estratégias para superar as lacunas identificadas. O plano deve ser claro, objetivo e focado no desenvolvimento do aluno.
