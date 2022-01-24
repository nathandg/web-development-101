### Relatório  

0. O que são APIs.  Para que servem ?

APIs tem a função de conectar sistemas, softwares e aplicativos. Dessa forma, permitindo trocar dados entre sistemas diferentes, na maior parte das vez essas trocas de dados tem como objetivo automatizar processos manuais e/ou permitir a criação de novas funcionalidades.

1. O que são Verbos HTTP ? Quais são eles e o que cada um faz ?  

São métodos de requisição responsáveis por indicar a ação a ser executada para um dado recurso.

* GET: o método GET solicita a representação de um recurso específico. Requisições utilizando o método GET devem retornar apenas dados.

* HEAD: o método HEAD solicita uma resposta de forma idêntica ao método GET, porém sem conter o corpo da resposta.

* POST: o método POST é utilizado para submeter uma entidade a um recurso específico, frequentemente causando uma mudança no estado do recurso ou efeitos colaterais no servidor.

*  PUT: o método PUT substitui todas as atuais representações do recurso de destino pela carga de dados da requisição

* DELETE: o método DELETE remove um recurso específico.

* CONNECT: o método CONNECT estabelece um túnel para o servidor identificado pelo recurso de destino.

* OPTIONS: o método OPTIONS é usado para descrever as opções de comunicação com o recurso de destino.

* TRACE: o método TRACE executa um teste de chamada loop-back junto com o caminho para o recurso de destino.

* PATCH: o método PATCH é utilizado para aplicar modificações parciais em um recurso.

<br>
1.1.Instale o POSTMAN em sua máquina. 
<br>
1.2.Para que o POSTMAN é utilizado? 
<br><br>
Postman é uma plataforma de API para construir e usar APIs.  O Postman simplifica cada etapa do ciclo de vida da API e agiliza a colaboração para que você possa criar APIs melhores e mais rapidamente.
<br><br>

2. O que acontece se voce enviar uma requisição GET pelo POSTMAN a sua githubpage ?

* Mostra o codigo fonte da página.

3. Quando voce acessa uma pagina web pelo navegador, qual é o verbo utilizado ?

* GET

4. O que são os códigos de status de resposta HTTP ?  

* São códigos de 3 dígitos, representando uma resposta a uma solicitação de uma página da web. 

4.1 Quais as classes de agrupamento dos status HTTP ?   

* Respostas de informação (100-199),
* Respostas de sucesso (200-299),
* Redirecionamentos (300-399)
* Erros do cliente (400-499)
* Erros do servidor (500-599).

4.2 Quando a requisição HTTP é bem sucedida, qual o código ?  

* 200 OK

4.3 Qual o status HTTP quando você não é autorizado a acessar um recurso ?  

* 403 Forbidden

4.4 Listar e descrever a utilização os seguintes códigos de cada agrupamento: 100, 200, 201, 202, 301, 400, 401, 403, 404, 405, 500, 501, 502. 

* 100 Continue: essa resposta provisória indica que tudo ocorreu bem até agora e que o cliente deve continuar com a requisição ou ignorar se já concluiu o que gostaria.

* 200 OK: estas requisição foi bem sucedida.

* 201 Created: a requisição foi bem sucedida e um novo recurso foi criado como resultado. Esta é uma tipica resposta enviada após uma requisição POST.

* 202 Accepted: a requisição foi recebida mas nenhuma ação foi tomada sobre ela. Isto é uma requisição não-comprometedora, o que significa que não há nenhuma maneira no HTTP para enviar uma resposta assíncrona indicando o resultado do processamento da solicitação. Isto é indicado para casos onde outro processo ou servidor lida com a requisição, ou para processamento em lote. 

* 301 Moved Permanently: esse código de resposta significa que a URI do recurso requerido mudou. Provavelmente, a nova URI será especificada na resposta.

* 400 Bad Request: essa resposta significa que o servidor não entendeu a requisição pois está com uma sintaxe inválida.

* 401 Unauthorized: embora o padrão HTTP especifique "unauthorized", semanticamente, essa resposta significa "unauthenticated". Ou seja, o cliente deve se autenticar para obter a resposta solicitada.

* 403 Forbidden: o cliente não tem direitos de acesso ao conteúdo portanto o servidor está rejeitando dar a resposta. Diferente do código 401, aqui a identidade do cliente é conhecida.

* 404 Not Found: o servidor não pode encontrar o recurso solicitado. Este código de resposta talvez seja o mais famoso devido à frequência com que acontece na web.

* 405 Method Not Allowed: o método de solicitação é conhecido pelo servidor, mas foi desativado e não pode ser usado. Os dois métodos obrigatórios, GET e HEAD, nunca devem ser desabilitados e não devem retornar este código de erro.

* 500 Internal Server Error: o servidor encontrou uma situação com a qual não sabe lidar. 

* 501 Not Implemented: o método da requisição não é suportado pelo servidor e não pode ser manipulado. Os únicos métodos exigidos que servidores suportem (e portanto não devem retornar este código) são GET e HEAD.

* 502 Bad Gateway: esta resposta de erro significa que o servidor, ao trabalhar como um gateway a fim de obter uma resposta necessária para manipular a requisição, obteve uma resposta inválida.

5. O que é Node.js ?  

* Node.js é um ambiente de execução JavaScript que permite executar aplicações desenvolvidas com a linguagem de forma autônoma, sem depender de um navegador.

5.1 Instale-o em sua máquina, versão LTS v14.17.3  | Listar os comandos que utilizou.
5.2 Para checar se você possui o node:   
```
$ node -v
v14.17.3
```
6. O que são gerenciadores de pacotes (software)?  
6.1 Instale os principais gerenciadores de pacote para a linguagem JavaScript em sua máquina. | Listar os comandos que utilizou.  
6.2 Para checar se você possui os gerenciadores:  
```
$ npm -v
7.24.1

$ yarn -v
1.22.11
```
7. Java e JavaScript são a mesma linguagem ? Descreva as diferenças entre essas linguagens e pesquise do porque do nome ser parecido.
  
8. Você possui o gerenciador de pacotes da linguagem Python em sua máquina?  
8.1  Caso não tenha, instale o principal gerenciador de pacote para a linguagem python. | Listar os comandos que utilizou.  
8.2 Para checar se você possui o gerenciador de pacote do python (V maisusculo):  
```
$ pip -V
pip 21.3.1
```
9. O que é linguagem interpretada ? O que é linguagem compilada ? E hibidria ?  
9.1 Escreva exemplos de linguagens compiladas, interpretadas e hibidrias.  
9.2 Qual o nome do compilador da linguagem C ?  
9.3 Qual o nome do compilador da linguagem Java ?
9.4 Qual o nome do interpretador do bytecode da linguagem java ?  
9.5 Qual o nome do interpretador da linguagem JavaScript ?
9.6 Qual o nome interpretador da linguagem Python?
9.7 Python é ou não compilado ? Pesquise e descreva o que encontrar.

10. O que é POO  em programação?  
10.1 Java é totalmente POO. O que é uma classe e o que é um objeto ?  
10.2 O que é a JVM, JRE e a JDK ? Descreva.  
10.3 Quais os principais gerenciadores de pacote da linguagem java ?
10.4 Instale o Open JDK 11 em sua máquina. | Listar os comandos que utilizou.  

```
$ java --version
java 11.0.12 2021-07-20 LTS
```     

11. O que é uma IDE, o que é um editor de texto ?    
11.1 Vs Code é uma IDE ou um editor de Texto ?  
11.2  Instale o Vs Code em sua máquina.  
11.3 IntelliJ é uma IDE ou editor de texto ?  
11.4 Instale o IntelliJ em sua máquina

12. O que é docker ?    
12.1 Quais suas vantagens ?  
12.1 Instale o Docker em sua máquina. | Listar os comandos que utilizou.  

* Estudaremos containers Docker, a linguagem Java entre outras com calma futuramente, por enquanto é somente importante se familiarizar com os conceitos apresentados nesse exercicio e com os processos de instalação e configuração do ambiente de desenvolvimento. 
---
