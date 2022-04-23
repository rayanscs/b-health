Solu��o 01

Foram desenvolvidos duas solu��es baseadas na mesma arquitetura, por�m com implementa��es diferentes.

A arquitetura utilizada:
- Cada hospital/Client iria acessar um frontend via WEB e/ou apps mobile.
- As rotas do front passariam por uma infra de gateway externo e interno.
- H� um BFF para os apps (solucao-01.1).
- As rotas referentes aos sistemas da empresa ficariam todos controlados pelo gateway interno.
- Com o backend do sistema apartado do frontend, as inclus�es de exames seriam efetuadas por mensageria utilizando RabbitMQ.
- Utilizar�amos como parte da resili�ncia do sistema envelvendo a mensageria, fila de hospital e cemiterio.
- H� consumidores para a fila, podendo ser paralelizados suas inst�ncias.
- A persist�ncia poderia ser feita em um banco SQL ou NoSQL, com bancos secundarios de backup, para quest�es de "Disaster Recovery". 

Solu��o 01.1
- Toda infra/sistemas s�o mantidos pela empresa.

Solu��o 01.2
- Toda infra/sistemas s�o mantidos na AWS.

Geral
- APIs desenvolvidos com modelagem de software em Domain Driven Design.
- Fronts desenvolvidos em arquitetura MVVM e modula��o de cosumo de servi�os.