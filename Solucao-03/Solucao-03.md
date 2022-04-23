**Solu��o 03**

Boas pr�ticas no processo de entrega em produ��o, pensando nos conceitos de disponibilidade, qualidade e seguran�a.


Ponto DISPONIBILIDADE:
- Servidores das aplica��es com redund�ncia e configura��es de balanceamento de cargas (F5 por exemplo).
- Utiliza��o da AWS ou qualquer outra solu��o em nuvem.
- Utiliza��o de Docker para conteineriza��o.
- Persistencia de dados com boas prt�ticas de Disaster Recovery.
- Utiliza��o de monitoramento das aplica��es e verifica��o de logs com ferramentas como New Relic, ElastichSearch/Kibana.
- Automa��o de acionamento de respons�veis pelas aplica��es e/ou plant�o.
- Esteira de CI/CD.

Ponto QUALIDADE
- Processos de CAB/Candidate para testes das aplica��es, com isso efetuando teste regressivo, teste de carga.
- Reuni�es de Chapter para dissemina��o de cen�rios ocorridos em PRD.
- Cria��o de testes unit�rios nos sistemas desenvolvidos.
- Execu��o de Code Review para an�lise de c�digo.
- Aplica��o de SonarQube para medi��o da qualidade do c�digo desenvolvido.

Ponto SEGURAN�A
- Utiliza��o de autentica��o de servi�o entre aplica��es.
- Utiliza��o de HTTPS.
- Dados sensiveis no header da reuqisi��o.
- Aplica��o de replace token para senhas nas aplica��es.

