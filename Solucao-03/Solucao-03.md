**Solução 03**

Boas práticas no processo de entrega em produção, pensando nos conceitos de disponibilidade, qualidade e segurança.


Ponto DISPONIBILIDADE:
- Servidores das aplicações com redundância e configurações de balanceamento de cargas (F5 por exemplo).
- Utilização da AWS ou qualquer outra solução em nuvem.
- Utilização de Docker para conteinerização.
- Persistencia de dados com boas prtáticas de Disaster Recovery.
- Utilização de monitoramento das aplicações e verificação de logs com ferramentas como New Relic, ElastichSearch/Kibana.
- Automação de acionamento de responsáveis pelas aplicações e/ou plantão.
- Esteira de CI/CD.

Ponto QUALIDADE
- Processos de CAB/Candidate para testes das aplicações, com isso efetuando teste regressivo, teste de carga.
- Reuniões de Chapter para disseminação de cenários ocorridos em PRD.
- Criação de testes unitários nos sistemas desenvolvidos.
- Execução de Code Review para análise de código.
- Aplicação de SonarQube para medição da qualidade do código desenvolvido.

Ponto SEGURANÇA
- Utilização de autenticação de serviço entre aplicações.
- Utilização de HTTPS.
- Dados sensiveis no header da reuqisição.
- Aplicação de replace token para senhas nas aplicações.

