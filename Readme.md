

## Prepara o ambiente

### Rodas os seguintes comandos na pasta raiz do projeto:

- Para criar uma rede docker
    - ```docker network create microservices_network```

- Inicializar as dependencias de repositórios
    -  ```git submodule init```

- Baixar/Atualizar os repositórios
    -  ```git submodule update```

- Start no projeto
    -  ```docker-compose up -d --build```    


### Endpoints:
* service-a: http://localhost:3001     
* service-b: http://localhost:3002    


> Este projeto foi desenvolvido para fins didáticos onde, o service-a se comunica com o service-b através de Mensageria utilizando o RabitMQ. Ambos os services tem seu próprio repositório mas, para centralizar em um único lugar, adotei o conceito de submodules git.

### Tecnologias:
- NestJS
- Postgress SQL
- RabitMQ
- Docker