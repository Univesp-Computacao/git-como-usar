# Praticando as conexões de SSH

Por padrão a **Criptografia assimétrica** é mais usada, que é a chamada da chave publica e privada.

É um processo bem simples, aonde a chave privada fica na sua maquina local e não pode ser compartilhada, enquanto a chave publica você envia para os diversos acessos remotos. Lembre-se sempre disso, sempre que houve um meio de acesso SSH, basta passa sua chave publica que resolve sua vida, ou seja, vamos supor que você tenha que acessa 100 maquinas remotas, bem é um processo demorado, ainda mais quando usamos soluções gráficas. Para isso, basta definir sua chave publica em todos os acessos e resolvido com um único comando você pode acessar cada uma delas com acesso total.

Vou deixa aqui o tutorial do [github SSH](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent){:target="_blank"} para criar uma chave publica e privada.

Para adicionar a chave na sua conta do [github adicionar SSH](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account){:target="_blank"}

E com isso já é possivel acessar via ssh seus repositorios no github.

Aqui o [Criando chave SSH - Git e Github para Iniciantes](https://www.youtube.com/watch?v=7YVQLZp1jb0){:target="_blank"} para ajudar visualmente a realizar o procedimento.

Lembre-se sempre disso, a geração da chave só é necessária uma única vez. Para realizar acessos remotos em outras máquinas é necessário que ela tenha sua chave publica, para isso existem muitas formas de realizar esse procedimento.

[Cloud GCP](https://www.youtube.com/watch?v=NPRO5NqOyLA){:target="_blank"}

[Cloud AWS](https://www.youtube.com/watch?v=2aAbbARgIwM){:target="_blank"}

[Cloude Azure](https://www.youtube.com/watch?v=3Ecm90UZHv0){:target="_blank"}

São alguns exemplos, a maioria dos clouds permitem que você faça upload da sua chave publica, use ela sem medo, vai facilitar sua vida, agora a chave partícula, não repasse para ninguém.

----

## Acessando outra máquina com SSH

Vou dá um exemplo prático para acessar via SSH alguma máquina remota, no caso vou acessar uma máquina VM que está na nuvem.

![exemplo](https://i.postimg.cc/TYXH7Wj5/image.png){ loading=lazy }

----

```bash
ssh ubuntu@150.230.89.10
```

Estou passando o seguinte comando para o **ssh** vai no usuário **ubuntu** no IP externo **150.230.89.10** bate a minha chave privada com a chave publica que está lá.

E pronto, o acesso está feito.

Quando falamos de acesso em cloud e em outras máquinas precisamos liberar as portas de acesso, por padrão o acesso da porta **22** exclusiva para acesso via protocolo SSH já vem liberado. Você só vai precisar do usuário e IP externo da máquina, além de que sua chave publica esteja lá.
