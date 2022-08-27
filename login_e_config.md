## Login e configuracao do Git
Quando voce instala o git eh necessario abrir um terminal e configurar algumas coisas basicas para que ele funcione com outros servidores git (github por exemplo)

Que sao:
- Nome (Muito importante sera o nome do Autor dos commits)
- Email (Mais importante ainda, esse email deve bater com o mesmo email do servidor git (ou seja no caso do github deve ser o mesmo e-mail usado no github))
- Login e Senha ou Chave SSH (Cada servidor tem o seu e vou explicar brevemente como isso funciona para o caso do Github)

### Configurar Nome e Email

O seguinte comando configura o nome do autor que aparecera no git:
```shell
git config --global user.name "Marcela Torro"
```

O seguinte comando configura o email do autor para o git:
```shell
git config --global user.email marcelatorro@gmail.com
```

### Login e Senha ou Chave SSH
O git da 2 opcoes para login com servidores git e farei um topico para cada uma a baixo explicando como funciona

#### Login e Senha
Eh o metodo menos seguro de autenticacao e algumas vezes servidores git podem ate mesmo negar sua autenticacao (Github comecara a negar em alguma data ai nao me lembro qual)

Para usar esse metodo eh preciso possuir um "Credential Manager" instalado no seu Sistema Operacional, para o caso do Windows o mesmo ja possui um credenciador nativo, para outros sistemas como Linux e Mac eh necessario instalar um por fora caso nao possuam nativamente.

Esse metodo agora se torna mais simples, ao tentar realizar um push ele vai pedir seu login e senha (pode nao pedir o login e usar simplesmente o e-mail), apos preencher tudo ja esta certo e sua senha sera gravada no gerenciador de credenciais.

#### Chave SSH
Eh o metodo mais seguro de todos para utilizar com servidores git, esse metodo consiste em criar uma chave no seu PC e ela sera sua chave de acesso para realizar acoes git que necessitam de um servidor (pull e push por exemplo)

Essa chave de acesso pode ser configurada com permissoes especificas e ser revogada a cada momento, alem disso vc pode ter infinitas chaves.

Essa chave tem que ser adicionada no servidor git para funcionar devidamente.

Para isso siga esses 2 tutoriais do Github de como criar uma chava ssh e adiciona-la no Github
- [Criar Chave SSH](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key)
- [Adicionar Chave SSH ao Github](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

ssh-keygen -t ed25519 -C "marcelatorro6@gmail.com"