# Login feito com Java e Spring 

## ⌨ Tecnologias usadas:
- Java
- MySQL
- Spring
- HTML
- CSS

## 📚 Observações:

- Durante o desenvolvimento, enfrentei alguns desafios técnicos que me proporcionaram uma curva de aprendizado significativa sobre o framework Spring. Encontrei dificuldades em implementar corretamente a lógica de requisições `POST` e em alguns momentos, tive problemas relacionados ao retorno das respostas no banco de dados. No entanto, por meio de pesquisas aprofundadas e análise de documentação, fui capaz de resolver essas questões de maneira eficiente. Embora seja um projeto simples, essas experiências contribuíram para o aprimoramento das minhas habilidades em Spring, me permitindo lidar de forma mais eficaz com problemas semelhantes no futuro.

## Banco de Dados: `applogin`

Este projeto utiliza um banco de dados chamado **applogin** para armazenar informações de usuários. Abaixo está a estrutura da tabela e suas colunas:

## Estrutura do Banco de Dados

### Nome do Banco de Dados:
- **applogin**

### Tabela: `usuario`

| Coluna  | Tipo de Dados | Descrição                          |
|---------|---------------|------------------------------------|
| `id`    | `BIGINT`      | Identificador único do usuário (chave primária, auto-incremento) |
| `email` | `VARCHAR(255)` | Endereço de e-mail do usuário (único) |
| `nome`  | `VARCHAR(255)` | Nome completo do usuário            |
| `senha` | `VARCHAR(255)` | Senha do usuário (armazenada de forma segura) |

### Exemplo de Estrutura SQL:

```sql
CREATE DATABASE applogin;

USE applogin;

CREATE TABLE usuario (
    id BIGINT AUTO_INCREMENT PRIMARY KEY,
    email VARCHAR(255) UNIQUE NOT NULL,
    nome VARCHAR(255) NOT NULL,
    senha VARCHAR(255) NOT NULL
);
