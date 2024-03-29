# API Produtos
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/Anna-Caroline/api-produtos/blob/main/LICENSE) 

# Sobre o Projeto
API desenvolvida para sistema de exibição, criação, edição e deleção de produtos vendidos por uma Companhia X e integração com banco de dados MySQL.

# Tecnologias
- Spring Boot
- Spring MVC
- Spring Data JPA
- MySQL

# Práticas adotadas
- SOLID
- DRY
- API REST
- Consultas com Spring Data JPA
- Injeção de dependências

# Como executar o projeto
- Clonar o repositório ou fazer download
- Abrir em IDE de preferência o arquivo DesafioTraineeAplication.java dentro da pasta src e rodar
<br> <br>A API poderá ser acessada em localhost:8080

# API Endpoints
Para fazer as requisições abaixo, foi utilizada a ferramenta [httpie](https://httpie.io/)

- Criar produto
```bash
$ http POST :8080/produtos nome="notebook" descricao="produto eletronico" codigo="3218" preco="2500"
[
    {
        "codigo": 3218,
        "descricao": "produto eletronico",
        "id": 1,
        "nome": "notebook",
        "preco": 2500.0
    }
]
```
- Listar produtos
```bash
$ http GET :8080/produtos
[
    {
        "codigo": 3218,
        "descricao": "produto eletronico",
        "id": 1,
        "nome": "notebook",
        "preco": 2500.0
    }
]

```
- Atualizar produto

```bash
$ http PUT :8080/projetos/1 nome="notebook marca x" preco="3000"
[
    {
        "codigo": 3218,
        "descricao": "produto eletronico",
        "id": 1,
        "nome": "notebook marca x",
        "preco": 3000.0
    }
]
```
- Remover produto
```bash
$ http DELETE :8080/produtos/1
[ ]
```

## Autora

Caroline Feitosa 

https://www.linkedin.com/in/carolinefeitosa/
