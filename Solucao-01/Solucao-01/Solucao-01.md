Solução 01

Foram desenvolvidos duas soluções baseadas na mesma arquitetura, porém com implementações diferentes.

A arquitetura utilizada:
- Cada hospital/Client iria acessar um frontend via WEB e/ou apps mobile.
- As rotas do front passariam por uma infra de gateway externo e interno.
- Há um BFF para os apps (solucao-01.1).
- As rotas referentes aos sistemas da empresa ficariam todos controlados pelo gateway interno.
- Com o backend do sistema apartado do frontend, as inclusões de exames seriam efetuadas por mensageria utilizando RabbitMQ.
- Utilizaríamos como parte da resiliência do sistema envelvendo a mensageria, fila de hospital e cemiterio.
- Há consumidores para a fila, podendo ser paralelizados suas instâncias.
- A persistência poderia ser feita em um banco SQL ou NoSQL, com bancos secundarios de backup, para questões de "Disaster Recovery". 

Solução 01.1
- Toda infra/sistemas são mantidos pela empresa.

Solução 01.2
- Toda infra/sistemas são mantidos na AWS.

Geral
- APIs desenvolvidos com modelagem de software em Domain Driven Design.
- Fronts desenvolvidos em arquitetura MVVM e modulação de cosumo de serviços.