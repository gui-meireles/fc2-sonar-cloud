### Conceitos do SonarQube

- Rules: Temos regras que aplicaremos no nosso projeto, como validações, segurança, etc....

- Quality Profiles: Criamos um perfil para a linguagem do nosso projeto e atribuimos as rules pra esse perfil

- Quality Gates: Ele quem bloqueia caso a aplicação tenha alguma falha de segurança, taxa baixa de testes, linhas duplicadas, etc...

---

### Primeiros passos

- O funcionamento do SonarCloud pegará apenas pull requests feitos na develop

- Adicione o seu repositório no SonarCloud: https://sonarcloud.io/projects

![adicionando_repositorio_sonar.gif](help_gif_images%2Fadicionando_repositorio_sonar.gif)

- Após, clique em continuar com GitHub Actions e adicione o token no seu repository

![img.png](help_gif_images/img.png)

![img_1.png](help_gif_images/img_1.png)

- Continuando, selecione a linguagem da sua aplicação e adicione o que o sonar recomendar:

![img_2.png](help_gif_images/img_2.png)