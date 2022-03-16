# Pull Request

Saindo um pouco do Git e ingressando em um contexto de comunidade, temos algumas ferramentas para contribuir com codigo aberto que já são disponibilizadas em plataformas como o Github, GitLab e BitBucket que é o Pull Request.

## O que é o pull request?

>As pull requests permitem que você informe outras pessoas sobre as alterações das quais você fez push para um branch em um repositório. Depois que uma pull request é aberta, você pode discutir e revisar as possíveis alterações com colaboradores e adicionar commits de acompanhamento antes que as alterações sofram merge no branch base.

Então para simplificar é um meio de gerar mudanças em um repositorio disponivel em uma das plataformas, com isso é possivel sugerir mudanças ou acrescentar novos features. Lembrando que não é necessario ter nenhum vinculo com o proprietario ou organização, é uma alteração que vai ser sugerida que pode ser aceita/incluida ou não.

----

## Praticando o pull request no Github

Primeiro passo, vá lá no repositorio de interesse, no nosso caso é [git-como-usar](https://github.com/Univesp-Computacao/git-como-usar) e criar um folk.

Agora que o repositorio já está atribuido a sua conta, fazer um pull para nossa maquina local:

1. Vá no repositorio que foi criado através do folk na sua conta
2. Abra ele
3. Vá em **Code**
4. Selecione o método SSH
5. Basta copia

----

![code](https://i.postimg.cc/Kvcs0wCT/image.png){ loading=lazy }

Faça um clone na sua maquina e vamos começar as alterações.

Assim que finalizar todas as alterações, faça o processo de push.

Finalizando, volte no github e vai ter uma notificação que houve alteração.

----

![alteração](https://i.postimg.cc/YSBPz07r/image.png){ loading=lazy }

Click em **Contribute** e vai lhe dá a opção de fazer o **Open Pull Request**:

----

![pull request](https://i.postimg.cc/QCggs8Pb/image.png){ loading=lazy }

Com isso podemos verificar na tela quais alterações estão sendo propostas:

----

![Comparação](https://i.postimg.cc/SQVJ0Y1P/image.png){ loading=lazy }

Click em **Create pull request** e em seguida vai ser direcionado para uma pagina que você pode descrever o motivo das alterações:

----

![Explicação](https://i.postimg.cc/VN53NpzM/image.png){ loading=lazy }

Basta finalizar em **Create pull request** que a vai ser disponibilizado para revisão do autor ou organização que mantém o repositorio.


## Do ponto de vista de quem recebe o pull request

Assim como existe quem solicita as alterações há quem as autorizas ou não, para isso vamos verificar essa outra parte do processo para ajudar na contextualização, assim que ocorre uma solicitação de **pull request** é habilitado no campo de **Pull request** do repositorio.

![pull auth](https://i.postimg.cc/7Y7kSfJ6/image.png){ loading=lazy }

----

E aqui está nossa solicitação que alguém sugeriu:

![pedido](https://i.postimg.cc/MHB1WyPV/image.png){ loading=lazy }

----

Após selecionar vai ter um historico de conversa e demais ações além de uma opção de fazer um **merge**/incluir essa alteração sugerida ou recusar com um **Close pull request**:

![Aceito](https://i.postimg.cc/0NF7wWJh/image.png){ loading=lazy }

Se for aceito a alteração é feito o merge e fechado a solicitação automaticamente, se não é somente fechado o topico.