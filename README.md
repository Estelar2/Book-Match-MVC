# BookMatchMVC

O **BookMatchMVC** é um sistema web em Java (Jakarta EE) para o gerenciamento e recomendação de livros, desenvolvido com a arquitetura **MVC** (Model-View-Controller).

## Estrutura de Pastas (MVC)
* **`model` (`Livro.java`)**: Representa os dados do livro.
* **`controller` (`LivroController.java`)**: Controla as rotas e recebe as ações da web.
* **`service` (`LivroService.java`)**: Contém as regras de negócio e validações.
* **`dao` (`LivroDAO.java`)**: Responsável por salvar e procurar os dados no MySQL.
* **`util` (`ConnectionFactory.java`)**: Cria a conexão com o banco de dados.

## O Fluxo do Cadastro
1. **View (Tela)**: O usuário envia os dados do livro pelo formulário.
2. **Controller**: Recebe os dados e cria o objeto `Livro`.
3. **Service**: Valida se as informações estão corretas (ex: nota entre 0 e 10).
4. **DAO**: Salva o livro permanentemente no banco de dados.

## Tecnologias
* Java 17 / Jakarta EE 6.0 (Servlets)
* Maven (Dependências)
* MySQL (Banco de dados)
