```yaml
name: criacao-material-didatico
description: Desenvolve um novo material didático (texto, apresentação, infográfico, vídeo) para um tópico específico, coordenando o Criador de Conteúdo Didático e o Tutor Personalizado.
command: /orquestrador-educacional --workflow criacao-material-didatico
```

# Fluxo de Trabalho: Criação de Material Didático

Este fluxo de trabalho é acionado quando há a necessidade de desenvolver um novo material didático para um tópico específico, seja para complementar um plano de estudo, abordar uma lacuna de conhecimento ou criar um novo curso. O **Orquestrador Educacional** coordena os agentes para produzir um material de alta qualidade.

## Fases do Fluxo de Trabalho

### Fase 1: Definição do Material e Objetivos (Orquestrador Educacional)

1.  **Orquestrador Educacional** inicia o fluxo, solicitando ao usuário (aluno/professor) as seguintes informações:
    *   Tópico/Conteúdo do material.
    *   Público-alvo (nível de escolaridade, faixa etária).
    *   Objetivos de aprendizagem do material (o que o aluno deve aprender/ser capaz de fazer).
    *   Formato desejado (texto, apresentação, infográfico, roteiro de vídeo, exercício).
    *   Recursos existentes ou referências.
2.  **Orquestrador Educacional** utiliza a habilidade `comunicacao-eficaz` para interagir com o usuário e garantir clareza nas especificações.

### Fase 2: Planejamento e Estruturação do Conteúdo (Criador de Conteúdo Didático)

1.  **Orquestrador Educacional** delega ao **Criador de Conteúdo Didático** a tarefa de planejar e estruturar o material.
2.  **Criador de Conteúdo Didático** utiliza a habilidade `design-instrucional` para definir a melhor abordagem pedagógica e a estrutura lógica do material.
3.  **Criador de Conteúdo Didático** utiliza a habilidade `curadoria-de-conteudo` para pesquisar e organizar informações relevantes e confiáveis.
4.  **Criador de Conteúdo Didático** retorna ao Orquestrador Educacional um esboço detalhado do material, incluindo tópicos, subtópicos e a abordagem geral.

### Fase 3: Desenvolvimento e Produção (Criador de Conteúdo Didático)

1.  **Orquestrador Educacional** aprova o esboço e delega ao **Criador de Conteúdo Didático** a produção do material.
2.  **Criador de Conteúdo Didático** utiliza a habilidade `adaptacao-linguistica` para escrever o texto com linguagem adequada ao público-alvo.
3.  Se o formato incluir elementos visuais ou audiovisuais, **Criador de Conteúdo Didático** utiliza a habilidade `producao-multimidia` para criar ou editar imagens, infográficos, roteiros de vídeo, etc.
4.  **Criador de Conteúdo Didático** retorna o material didático completo ao Orquestrador Educacional.

### Fase 4: Revisão Pedagógica e Validação (Tutor Personalizado e Avaliador de Aprendizagem)

1.  **Orquestrador Educacional** envia o material para o **Tutor Personalizado** para uma revisão pedagógica.
2.  **Tutor Personalizado** utiliza a habilidade `pedagogia` para avaliar a clareza, engajamento e alinhamento do material com os objetivos de aprendizagem, sugerindo ajustes.
3.  **Orquestrador Educacional** pode envolver o **Avaliador de Aprendizagem** para criar pequenas questões ou atividades de verificação para o material, garantindo sua eficácia.
4.  **Orquestrador Educacional** consolida o feedback e solicita ao **Criador de Conteúdo Didático** as revisões necessárias.

### Fase 5: Entrega Final (Orquestrador Educacional)

1.  Após as revisões, **Orquestrador Educacional** entrega o material didático finalizado ao usuário.
2.  **Orquestrador Educacional** solicita feedback final do usuário sobre a qualidade e utilidade do material.

## Agentes Envolvidos

*   **Orquestrador Educacional:** Coordenação geral, definição de objetivos, consolidação de feedback, entrega.
*   **Criador de Conteúdo Didático:** Planejamento, pesquisa, desenvolvimento e produção do material.
*   **Tutor Personalizado:** Revisão pedagógica, sugestões de melhoria.
*   **Avaliador de Aprendizagem (opcional):** Validação da eficácia do material.

## Habilidades Utilizadas

*   `comunicacao-eficaz`
*   `design-instrucional`
*   `curadoria-de-conteudo`
*   `adaptacao-linguistica`
*   `producao-multimidia`
*   `pedagogia`
*   `avaliacao-de-conhecimento` (opcional)

## Saída Esperada

Um material didático completo no formato solicitado (ex: arquivo Markdown, PDF, apresentação, roteiro de vídeo), pronto para ser utilizado no processo de ensino-aprendizagem, acompanhado de uma breve descrição de como ele atende aos objetivos definidos.
