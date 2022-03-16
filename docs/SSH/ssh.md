# O que é SSH?

>O SSH é um protocolo e um serviço, que permite a comunicação entre dois pontos de uma rede de qualquer abrangência, utilizando criptografia para aumentar o nível de segurança na troca de informações, bem como facilitar transações e ações.

O SSH foi criado por Tatu Ylönen, em 1995, quando era professor na Universidade de Tecnologia de Helsinque, em função de uma invasão na rede da universidade, em que se descobriu um sniffer e que basicamente consiste em um programa usado com frequência para monitorar e analisar o tráfego de redes e dependendo da motivação, pode ter uma destinação maliciosa.

Esse foi o caso. O sniffer descoberto na rede, havia capturado informações de milhares de usuários e respectivas senhas e armazenado-as em um banco de dados.

Isso foi suficiente para que o então jovem docente, lançasse poucos meses depois, a primeira versão de código aberto (Open Source) para o SSH.

No entanto, com o passar do tempo a empresa criada por Ylönen tornou o SSH proprietário, até que um grupo de desenvolvedores independentes baseou-se na última versão de código aberto do SSH para criar o que hoje é conhecido como OpenSSH e é incorporado aos sistemas operacionais Unix, Linux e desde 2017, até mesmo no Windows.

Estima-se que atualmente mais da metade dos servidores web no mundo, utilizem o serviço.

----

## Quais as vantagens do SSH?

O que se viu até aqui, já bastaria para justificar a importância e quais as principais vantagens de se utilizar o SSH como protocolo nas transações que envolvem trocas de dados em redes de todas as abrangências, mas vamos além e listaremos abaixo as principais vantagens do uso deste serviço:

+ Troca de dados criptografados, que mesmo que ocorra a interceptação da comunicação por parte de um invasor na rede, impede que ele tenha conhecimento da informação trafegada.
+ Há serviços, bem como clientes de SSH gratuitos e open source.
+ Todos os principais sistemas operacionais já tem clientes SSH, o que evita que se tenha que instalar um cliente de SSH.
+ A grande maioria dos servidores de hospedagem tem serviços SSH instalados, o que permite que se conecte ao servidor de modo seguro.
+ Em sistemas Linux, por exemplo, é possível efetuar um acesso SSH ao servidor e com os devidos privilégios administrativos, ter total controle do ambiente, da mesma forma que se estivesse fisicamente em frente a máquina
+ Em vez de efetuar o login a um servidor utilizando o velho método de usuário e senha e requer muitas vezes que boa parte dos usuários mantenham algum categoria de lista ou arquivos de senhas, já que elas estão presentes em tudo hoje em dia e, ao mesmo tempo vulnerabiliza os protocolos de segurança, o protocolo SSH permite a utilização de chaves criptografadas para autenticação, poupando trabalho e melhorando a segurança das transações de login / autenticação.
+ Certas ações feitas usando-se o SSH, são mais simples e seguras do que usando outros protocolos, como, por exemplo, o FTP. Assim, um usuário com os devidos conhecimentos e privilégios, consegue realizar um backup alternativamente ao FTP, de forma mais rápida e fácil.
+ Pelo fato de utilizar linhas de comando para realização de todas as ações, consegue-se maior controle e poder sobre servidor acessado, em detrimento das facilidades de uma interface gráfica, mas que geralmente são mais limitadas.

----

## Quais são as criptografias usadas pelo SSH?

A criptografia é o que garante, além da segurança do site, também a proteção dessa tarefa de conexão entre o cliente e o servidor remoto. No entanto, há diferentes estruturas de criptografia que podem ser aplicadas na hora de usar o protocolo SSH nessa demanda. São, basicamente, três alternativas: simétrica, assimétrica e hashing;

### Criptografia simétrica

Essa é uma forma de criptografia realizada por uma chave secreta, essa sendo compartilhada apenas entre o servidor e o usuário. Seu papel é criptografar ou descriptografar a mensagem transferida nesse processo, no entanto, a secure shell só oferece a leitura do conteúdo mediante a apresentação dessa chave.

A nomenclatura de referência à simetria é originada do processo utilizado para gerar essa chave. Ela é criada por um algoritmo que, automaticamente, envia a chave para as duas partes envolvidas: cliente e servidor. No entanto, não há a transferência dessa informação entre as duas partes, cabendo ao algoritmo enviar a cada uma separadamente.

Cada vez que uma sessão SSH é criada, uma nova chave de criptografia é gerada no momento anterior à autenticação. Assim, na hora de transferir o arquivo, o usuário já tem a senha utilizada para criptografar o conteúdo e então realizar esse envio ao servidor.

### Criptografia assimétrica

Esse modelo é o oposto do anterior: são usadas duas chaves, uma para o cliente e outra para o servidor, para haver a criptografia dos dados transferidos. As chaves são chamadas pública e privada, formando então a combinação necessária para gerar o SSH e seu protocolo de segurança.

Nesse modelo, a chave pública é distribuída de forma aberta e compartilhada. No entanto, a partir dela não é possível descobrir qual é a chave privada. Isso acontece graças a um processo que funciona da seguinte maneira: mensagens criptografadas por chaves públicas só podem ser descriptografadas pela chave privada da mesma máquina.

A chave privada, em meio a esse processo, deve permanecer inacessível a terceiros, sendo de posse e uso somente do cliente. Isso é fundamental, dado que seu uso possibilita descriptografar as chaves públicas, e assim acessar o conteúdo transferido.

### Hashing

O hashing é um método unidirecional de criptografia usado no SSH. Essa prática consiste em criar um hash, por um algoritmo, para garantir que a mensagem será protegida em uma forma específica de criptografia e códigos de autenticação. O processo é feito usando HMACs (Hash-based Message Authentication Codes), garantindo que não haja violação nos códigos que serão recebidos pelo servidor remoto.

----

## Fontes

[Github](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/about-ssh)

[RockContent](https://rockcontent.com/br/blog/ssh/)
