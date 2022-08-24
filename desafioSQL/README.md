# Desafio

Criar 3 tabelas
  - Pais
      id (numero e chave primaria)
      nome (texto)
      sigla (3 caracteres)

  - Estado
      id (numero e chave primaria)
      nome (texto)
      sigla (2 caracteres)
      id_pais (numero)

  - Cidade
      id (numero e chave primaria)
      nome (texto)
      id_estado (numero)

Parte 2:
  - Inserir ao menos 2 paises
  - Inserir os 27 estados
  - Inserir 2 municipios por estado

Parte 3:
- Tirar um relatorio (uma consulta SELECT) com os seguintes campos:
    nome_pais
    sigla_pais
    nome_estado
    sigla_estado
    nome_cidade


# Solução

Usando o "SELECT" você consegue listar as tabelas e com o "JOIN" você consegue consultar as 3 tabelas Tendo alguma coisa que esteja iguais nelas.

```SELECT PAIS.NOME, PAIS.SIGLA, ESTADO.NOME, ESTADO.SIGLA, CIDADE.NOME FROM PAIS JOIN ESTADO ON PAIS.ID = ESTADO.ID_PAIS JOIN CIDADE ON ESTADO.ID = CIDADE.ID_ESTADO;```

![Captura de Tela 2022-08-23 às 18 38 05](https://user-images.githubusercontent.com/69183396/186271247-dda9f8d9-36aa-4aa6-8ae1-d8a47c55a214.png)

O "JOIN" Está linkando o PAIS com o ESTADO com o id Dos dois e a mesma coisa entre ESTADO E CIDADE.
