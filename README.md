# Board: Um Gerenciador de Tarefas via Terminal

**Board** é uma aplicação de console robusta, projetada para a gestão eficiente de fluxos de trabalho através de quadros Kanban. Criado como um desafio de programação, este sistema permite organizar, acompanhar e analisar o ciclo de vida de tarefas de forma intuitiva e persistente.

## 📑 Sobre o Projeto

Inspirado em metodologias ágeis, o Board simula um quadro físico de tarefas, onde cada atividade (card) progride através de diferentes etapas (colunas) até sua conclusão ou cancelamento. A aplicação foi desenvolvida com foco em lógica de programação, interação com o usuário via terminal e persistência de dados com um banco de dados relacional.

## ✨ Principais Recursos

O sistema oferece um conjunto completo de funcionalidades para um gerenciamento de tarefas eficaz:

  * 🎨 **Quadros (Boards) Dinâmicos:** Crie múltiplos quadros para gerenciar diferentes projetos ou contextos. Alterne facilmente entre eles através de um menu interativo, permitindo deletar quadros que não são mais necessários.

  * 📊 **Fluxo de Trabalho Estruturado:** Organize suas tarefas em colunas personalizáveis que representam as etapas do seu processo. O sistema garante uma estrutura mínima (`A Fazer`, `Concluído`, `Cancelado`) e organiza as colunas em uma ordem lógica que define o fluxo de trabalho.

  * ➡️ **Movimentação Inteligente de Tarefas:** Arraste seus cards (tarefas) entre as colunas, seguindo a lógica do fluxo de trabalho. O sistema permite cancelar uma tarefa de qualquer etapa (exceto das colunas de finalização), oferecendo flexibilidade no processo.

  * 📝 **Gerenciamento Completo de Cards:** Cada tarefa possui título, descrição e data de criação. Adicione novos cards, visualize seus detalhes e gerencie seu ciclo de vida dentro do quadro.

  * 🔒 **Sistema de Bloqueio:** Interrompa o progresso de uma tarefa com a função de bloqueio. É possível bloquear e desbloquear qualquer card, sempre registrando uma justificativa para a ação.

  * 💾 **Persistência Confiável com MySQL:** Todos os seus dados — quadros, colunas e tarefas — são armazenados de forma segura em um banco de dados MySQL. Feche a aplicação e retome seu trabalho exatamente de onde parou.

## 🚀 Funcionalidades Avançadas (Desafios Opcionais)

Para uma análise mais profunda da produtividade, o projeto pode ser estendido com:

  * 📈 **Histórico de Movimentações:** Rastreie todo o percurso de um card, registrando carimbos de tempo para cada entrada e saída nas colunas.
  * ⏱️ **Relatório de Lead Time:** Gere métricas sobre o tempo total de conclusão de uma tarefa, com detalhes sobre quanto tempo ela permaneceu em cada etapa do fluxo.
  * 🛑 **Análise de Bloqueios:** Obtenha um relatório detalhado sobre o histórico de bloqueios de cada card, incluindo a duração de cada bloqueio e as justificativas associadas.

## 🛠️ Tecnologias e Ferramentas

  * **Linguagem:** Java
  * **Banco de Dados:** MySQL
  * **Gerenciamento de Dependências:** (Adicionar, se houver, ex: Maven, Gradle)
  * **Conector:** JDBC (Java Database Connectivity)

## ⚙️ Guia de Instalação e Uso

Para executar este projeto em sua máquina local, siga os passos abaixo.

### Pré-requisitos

  * Java Development Kit (JDK) instalado (versão 8 ou superior).
  * Um servidor de banco de dados MySQL ativo.
  * Git instalado.

### Passos de Instalação

1.  **Clone o repositório:**

    ```bash
    git clone https://github.com/hevlyo/board.git
    ```

2.  **Acesse o diretório do projeto:**

    ```bash
    cd board
    ```

3.  **Configure a Conexão com o Banco de Dados:**

      * Crie um banco de dados (schema) no seu servidor MySQL para o projeto.
      * Localize o arquivo de configuração de banco de dados (ex: `config.properties`, `persistence.xml`).
      * Atualize as credenciais de conexão com seu host, porta, nome do banco, usuário e senha.

4.  **Compile e Execute:**

      * Compile os arquivos Java. Se estiver usando um IDE (como IntelliJ ou Eclipse), basta executar a classe principal.
      * Via terminal, a execução pode variar dependendo da estrutura do projeto (ex: `java -jar board.jar` se for um projeto empacotado).

5.  **Comece a Usar:**

      * Ao iniciar, a aplicação apresentará um menu principal.
      * Siga as instruções no console para criar seu primeiro quadro, adicionar colunas e começar a gerenciar suas tarefas\!
