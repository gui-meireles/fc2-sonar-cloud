### Conceitos do SonarQube

- Rules: Temos regras que aplicaremos no nosso projeto, como validações, segurança, etc....

- Quality Profiles: Criamos um perfil para a linguagem do nosso projeto e atribuimos as rules pra esse perfil

- Quality Gates: Ele quem bloqueia caso a aplicação tenha alguma falha de segurança, taxa baixa de testes, linhas duplicadas, etc...

---

### Primeiros passos

- Subir docker local do sonarqube: `docker run -d --name sonarqube -e SONAR_ES_BOOTSTRAP_CHECKS_DISABLE=true -p 9000:9000 sonarqube:latest`

- Usuario e senha: `admin`. Mude para `admin1` ou uma senha de sua escolha.

- Crie seu projeto no sonarqube e ele te dará um token ( Veja o nome/key do projeto nas .properties dentro das pastas Go e Js )
- Cole esse token no seu .properties

- Na pasta de js, digite os comandos npm install jest @types/jest sonar-scanner --only-dev

---

### Depois de configurado

- Abra um terminal e rode o comando sonar-scanner
- Com isso ele testará nossa aplicação Go/Js e conseguiremos ver na interface do sonar.