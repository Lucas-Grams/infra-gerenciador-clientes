Para o desenvolvimento da solução "Gerenciamento de dados de clientes" proponho um sistema que utiliza uma arquitetura de microsserviços, onde teremos:

Uma API desenvolvida utilizando o framework Spring Boot (repositório "api-gerenciador-clientes").
Um cliente desenvolvido utilizando o framework Angular (repositório "client-gerenciador-clientes").
Uma base de dados utilizando o PostgreSQL.

Para executar a aplicação é necessário primeiramente ter instalado na máquina de testes o Docker para utilizar os containers da aplicação. 

Se já tivermos o Docker disponível é necessário apenas acessar a pasta "infra-gerenciador-clientes" no terminal da máquina e utilizar o comando:
	docker compose up --build

 Para que o build ocorra de forma correta também é necessário que o Client e a API estejam no mesmo diretório do infra.

Após isso será feito o buid do projeto inteiro, base de dados, api e cliente para um container "infra-gerenciador-cliente".

Para utilizarmos o sistema devemos acessar em algum navegador web a url: 
	http://localhost:4200/
