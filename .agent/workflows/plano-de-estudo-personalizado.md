```yaml
name: plano-de-estudo-personalizado
description: Cria um plano de estudo detalhado e adaptado às necessidades e objetivos de um aluno, coordenando o Tutor Personalizado e o Criador de Conteúdo Didático.
command: /orquestrador-educacional --workflow plano-de-estudo-personalizado
```

# Fluxo de Trabalho: Plano de Estudo Personalizado

Este fluxo de trabalho é acionado quando um aluno (ou professor) solicita um plano de estudo adaptado para um tópico ou disciplina específica. O **Orquestrador Educacional** coordena os agentes para entregar um plano abrangente e eficaz.

## Fases do Fluxo de Trabalho

### Fase 1: Coleta de Informações e Análise de Necessidades (Orquestrador Educacional)

1.  **Orquestrador Educacional** inicia o fluxo, solicitando ao usuário (aluno/professor) as seguintes informações:
    *   Tópico/Disciplina de interesse.
    *   Nível de conhecimento atual (iniciante, intermediário, avançado).
    *   Objetivos de aprendizagem (ex: passar em uma prova, aprender um novo conceito, aprofundar conhecimento).
    *   Estilo de aprendizagem preferencial (visual, auditivo, leitura/escrita, cinestésico).
    *   Prazo disponível para o estudo.
2.  **Orquestrador Educacional** utiliza a habilidade `comunicacao-eficaz` para interagir com o usuário e garantir que todas as informações necessárias sejam coletadas de forma clara.

### Fase 2: Elaboração da Estratégia de Ensino (Tutor Personalizado)

1.  **Orquestrador Educacional** delega ao **Tutor Personalizado** a tarefa de elaborar uma estratégia de ensino inicial com base nas informações coletadas.
2.  **Tutor Personalizado** utiliza a habilidade `pedagogia` para definir a melhor abordagem didática e a sequência de tópicos.
3.  **Tutor Personalizado** utiliza a habilidade `motivacao-aluno` para identificar pontos de engajamento e sugestões para manter o aluno motivado.
4.  **Tutor Personalizado** retorna ao Orquestrador Educacional um esboço do plano de estudo, incluindo tópicos, sequência e sugestões de atividades.

### Fase 3: Criação/Curadoria de Conteúdo (Criador de Conteúdo Didático)

1.  **Orquestrador Educacional** delega ao **Criador de Conteúdo Didático** a tarefa de desenvolver ou curar materiais para os tópicos definidos pelo Tutor.
2.  **Criador de Conteúdo Didático** utiliza a habilidade `curadoria-de-conteudo` para buscar e selecionar recursos existentes (artigos, vídeos, exercícios).
3.  Se necessário, **Criador de Conteúdo Didático** utiliza a habilidade `producao-multimidia` para criar novos materiais (infográficos, resumos, roteiros de vídeo).
4.  **Criador de Conteúdo Didático** utiliza a habilidade `adaptacao-linguistica` para garantir que os materiais sejam adequados ao nível e estilo de aprendizagem do aluno.
5.  **Criador de Conteúdo Didático** retorna os materiais ao Orquestrador Educacional.

### Fase 4: Consolidação e Apresentação do Plano (Orquestrador Educacional)

1.  **Orquestrador Educacional** consolida o plano de estudo detalhado, integrando a estratégia do Tutor Personalizado e os materiais do Criador de Conteúdo Didático.
2.  **Orquestrador Educacional** apresenta o plano final ao usuário, utilizando a habilidade `comunicacao-eficaz` para explicar cada etapa e como o aluno deve proceder.
3.  **Orquestrador Educacional** solicita feedback inicial do usuário para possíveis ajustes.

## Agentes Envolvidos

*   **Orquestrador Educacional:** Coordenação geral, análise de necessidades, consolidação.
*   **Tutor Personalizado:** Elaboração da estratégia pedagógica, sugestões de motivação.
*   **Criador de Conteúdo Didático:** Curadoria e desenvolvimento de materiais.

## Habilidades Utilizadas

*   `comunicacao-eficaz`
*   `pedagogia`
*   `motivacao-aluno`
*   `curadoria-de-conteudo`
*   `producao-multimidia`
*   `adaptacao-linguistica`

## Saída Esperada

Um documento Markdown (ou outro formato solicitado) contendo um plano de estudo personalizado, com a sequência de tópicos, materiais recomendados, atividades sugeridas e dicas de motivação, adaptado ao perfil do aluno. O plano deve ser claro, objetivo e fácil de seguir.
