# CRUD Básico em C++

Esse projeto é um CRUD simples feito em C++, focado em gerenciar um cadastro de clientes na linha de comando.

## O que ele faz?

- **Cadastrar clientes:** adiciona novos clientes com nome e ID automático.
- **Listar clientes:** mostra todos os clientes cadastrados.
- **Editar clientes:** altera o nome do cliente pelo ID.
- **Excluir clientes:** remove o cliente pelo ID.
- **Sair:** fecha o programa.

## Estrutura do projeto

- **main.cpp:** arquivo principal com o menu e a interação com o usuário.
- **sistema.h:** classe `Sistema` que controla as operações do CRUD, usando um vetor de clientes.
- **cliente.h:** classe `Cliente` que representa o cliente, guarda o nome, um ID único gerado automaticamente e métodos para acessar/modificar os dados.

## Como funciona?

- O `main.cpp` roda um loop com menu, recebendo a opção do usuário.
- Dependendo da opção, chama os métodos da classe `Sistema` para executar cadastro, listagem, edição ou exclusão.
- A classe `Sistema` mantém um vetor interno de objetos `Cliente`.
- A classe `Cliente` gera um ID único estático para cada cliente novo e armazena o nome.

## Tecnologias usadas

- C++ padrão (com STL)
- Uso de vetor para armazenar clientes dinamicamente
- Separação de responsabilidades: classes Cliente e Sistema em arquivos separados para manter o código limpo e organizado.

## Como usar?

1. Compile os arquivos `.cpp` juntos, por exemplo:

```bash
g++ main.cpp -o crud
(só certifique-se de incluir todos os arquivos no comando ou montar um Makefile)
```
2. Rode o programa:
```bash
./crud
```
3. Use o menu pra cadastrar, listar, editar e excluir clientes.

Digite 0 para sair do programa.
