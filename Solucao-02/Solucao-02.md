**Solu��o 02**

- Projeto de frontend apartado do backend.
- Desenvolver API para o agendamento de exames, pagamentos, consultas dos dados do hospital. Com isso, o front consome suas rotas.
- Aplicar o pattern Singleton para conex�o com o banco de dados.
- Utilizar Repository Pattern para isolar a camada de acesso a dados (DAL), impulsionando o uso de inje��o de depend�ncia.
- Para CRUDs, utiliza��o de algum Micro ORM para usar "query pura", caso seja um BD SQL.
- Cria��o de �ndices em banco de dados caso necess�rio.
- Para CRUDs NoSQL, otimiza��o de estrutura json caso necess�rio (gen�rica adaptativa).
- Aplica��o de cache no Redis.

Desenho
<img src="./Solucao-02-b-health.jpeg" width="1024"/>