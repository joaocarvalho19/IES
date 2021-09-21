## What would be the proper HTTP Status code to get when searching an API for non-existent?

404 not Found

## GET - http://localhost:8080/employees/

{
    "_embedded": {
        "employeeList": [
            {
                "id": 1,
                "firstName": "Bilbo",
                "lastName": "Baggins",
                "role": "burglar",
                "name": "Bilbo Baggins",
                "_links": {
                    "self": {
                        "href": "http://localhost:8080/employees/1"
                    },
                    "employees": {
                        "href": "http://localhost:8080/employees"
                    }
                }
            },
            {
                "id": 2,
                "firstName": "Frodo",
                "lastName": "Baggins",
                "role": "thief",
                "name": "Frodo Baggins",
                "_links": {
                    "self": {
                        "href": "http://localhost:8080/employees/2"
                    },
                    "employees": {
                        "href": "http://localhost:8080/employees"
                    }
                }
            }
        ]
    },
    "_links": {
        "self": {
            "href": "http://localhost:8080/employees"
        }
    }
}

## POST - http://localhost:8080/employees/

{
	"role": "gardener",
	"name": "Gustavo Rodrigues"
}
----------
{
	"role": "gardener",
	"name": "Joao Carvalho"
}

## PUT - http://localhost:8080/employees/6

{
    "name": "Gustavo Rodrigues",
    "role": "burglar"
}

## GET - http://localhost:8080/employees/

{
                "id": 1,
                "firstName": "Bilbo",
                "lastName": "Baggins",
                "role": "burglar",
                "name": "Bilbo Baggins",
                "_links": {
                    "self": {
                        "href": "http://localhost:8080/employees/1"
                    },
                    "employees": {
                        "href": "http://localhost:8080/employees"
                    }
                }
            },
            {
                "id": 2,
                "firstName": "Frodo",
                "lastName": "Baggins",
                "role": "thief",
                "name": "Frodo Baggins",
                "_links": {
                    "self": {
                        "href": "http://localhost:8080/employees/2"
                    },
                    "employees": {
                        "href": "http://localhost:8080/employees"
                    }
                }
            },
            {
                "id": 5,
                "firstName": "Joao",
                "lastName": "Carvalho",
                "role": "gardener",
                "name": "Joao Carvalho",
                "_links": {
                    "self": {
                        "href": "http://localhost:8080/employees/5"
                    },
                    "employees": {
                        "href": "http://localhost:8080/employees"
                    }
                }
            },
            {
                "id": 6,
                "firstName": "Gustavo",
                "lastName": "Rodrigues",
                "role": "burglar",
                "name": "Gustavo Rodrigues",
                "_links": {
                    "self": {
                        "href": "http://localhost:8080/employees/6"
                    },
                    "employees": {
                        "href": "http://localhost:8080/employees"
                    }
                }

## Ex3_2-----------------------------------------------------------------------

## @Table
    Especifica o nome da tabela da base de dados("employees")

## @Column
    Especifica a coluna da tabela a ser mapeada

## Id
    Especifica a chave primaria da tabela("id")

## Autowired
    É usado ao colocar uma instância de um bean no campo desejado em uma instância de outro bean.


## Ex3_3-----------------------------------------------------------------------

## Controller e RestController

O @Controller cria um mapa do model object e encontra uma view, mas @RestController simplesmente retorna o object e os dados do object é gravado diretamente na resposta HTTP.