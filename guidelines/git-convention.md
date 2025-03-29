# Padronização do Git Workflow, Commits, Nomes das Branchs e Pull Requests

Este documento aborda a importância da padronização do workflow utilizando o git, na nomenclatura de commits, branches e pull requests em um projeto de desenvolvimento de software. A adoção de convenções claras e consistentes não apenas melhora a legibilidade do histórico do projeto, mas também facilita a colaboração entre os membros da equipe, tornando o processo de desenvolvimento mais eficiente e organizado.

## Git Workflow

O fluxo que será aplicado é o seguinte: o projeto terá duas branchs, **main** e **develop**. O desenvolvedor que desejar adicionar uma nova alteração deve criar sua branch a partir da branch **develop**, realizar as alterações e, em seguida, solicitar um Pull Request (PR) para a branch **develop**. Assim que cada bloco de funcionalidades for testado e validado na branch **develop**, as alterações serão integradas à branch **main** por meio de um PR.

## Padronização de Commits

A padronização dos commits é fundamental para manter um histórico claro e compreensível. As diretrizes adotadas seguem as recomendações do [Conventional Commits](https://www.conventionalcommits.org/pt-br/v1.0.0-beta.4/). Seguem alguns pontos importantes:

- **Formato da Mensagem:**
  Utilize o formato `tipo: descrição`, onde o tipo pode ser:

  - **feat:** nova funcionalidade
  - **fix:** correção de bug
  - **docs:** documentação
  - **style:** formatação
  - **refactor:** refatoração
  - **test:** testes
    **Exemplos:**
    `feat: adicionar funcionalidade de login`
    `fix: corrigir erro no cálculo de impostos`

- **Limite de Caracteres:**
  Mantenha a descrição do commit curta, idealmente com até 72 caracteres na linha de título, utilizando o corpo da mensagem para detalhes adicionais, se necessário.

- **Imperativo:**
  Escreva as mensagens no modo imperativo, como se estivesse dando uma ordem (por exemplo, "Adicionar" em vez de "Adicionado").

## Nomenclatura das Branchs

A nomenclatura das branchs deve ser clara e descritiva, permitindo que todos os membros da equipe entendam rapidamente o propósito da branch. Recomenda-se:

- **Formato de Nomes:**
  Utilize um padrão que inclua o tipo de trabalho e uma breve descrição, por exemplo:
  `feature/adicionar-login`
  `bugfix/corrigir-erro-calculo`

- **Uso de Identificadores:**
  O JIRA fornece um identificador único para cada tarefa. Utilize esse identificador no nome da branch para facilitar o rastreamento e a associação com a tarefa correspondente. Por exemplo:
  `bugfix/MBA-4-sample-initiate-fund-transfer`
  `feature/MBA-5-sample-two-factor-authentication-setup`
  `hotfix/MBA-6-sample-fix-typo-in-documentation`

## Padronização de Pull Requests

Os pull requests (PRs) são essenciais para um fluxo de trabalho colaborativo. Para melhorar a revisão e a integração do código, siga estas diretrizes:

- **Título do PR:**
  O título deve ser claro e descritivo, seguindo o mesmo formato dos commits, incluindo o tipo e uma breve descrição.
  **Exemplo:**
  `feat: adicionar funcionalidade de login`

- **Descrição do PR:**
  Forneça uma descrição detalhada que explique o que foi feito, por que foi feito e como testar a nova funcionalidade ou correção. Inclua referências a issues relacionadas, se aplicável.

- **Checklist:**
  Inclua uma checklist no corpo do PR para garantir que todos os passos necessários foram seguidos antes da revisão (ex.: testes realizados, documentação atualizada, etc.).

## Conclusão

A padronização de commits, nomes de branchs e pull requests é essencial para a manutenção de um projeto de software saudável e colaborativo. Ao seguir estas diretrizes, a equipe melhora a comunicação, a organização e a eficiência no desenvolvimento, resultando em um código mais limpo e de fácil manutenção.
