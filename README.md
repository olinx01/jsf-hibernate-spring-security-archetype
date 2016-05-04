# JSF Hibernate Spring Security Archetype


Este é um Maven Archetype que lhe possibilita criar uma aplicação JSF com Hibernate, JPA e SpringSecurity em minutos. O projeto gerado já terá 2 CRUDS básicos para que lhe seja possível botar a mão na massa de imediato. A aplicação é protegida pelo SpringSecurity, desse modo sua aplicação já estará pronta para autenticar e autorizar seus usuários. Este Archetype foi desenvolvido baseado no projeto [Semeru JSF Maven](https://github.com/leandrocgsi/semeru_jsf_maven). Então mãos a obra vamos aprender como usar esse poderoso recurso. 

Se você quer entender direito como funciona essa arquitetura assista ao curso "Curso De JSF Do Zero À Nuvem" disponibilizado gratuitamente no [Youtube](https://www.youtube.com/playlist?list=PL18bbNo7xuh9d1AyAeC77O8xRz6hPD3iJ).

# Frameworks e Tecnologias Utilizadas

* [JSF (Mojarra)](https://javaserverfaces.java.net/)
* [Primefaces](http://www.primefaces.org/)
* [JPA](http://www.oracle.com/technetwork/java/javaee/tech/persistence-jsp-140049.html)
* [Hibernate](http://hibernate.org/)
* [Maven](https://maven.apache.org/)
* [Spring Security](http://projects.spring.io/spring-security/)
* [MySQL](https://www.mysql.com/)
* [MySQL Administrator](https://downloads.mysql.com/archives/administrator/) - Que foi descontinuado e você pode substituir pelo [Heidi SQL](http://www.heidisql.com/)
* [Apache Tomcat](http://tomcat.apache.org/)


# Como usar este Archetype?

Primeiro você precisa clonar esse projeto no seu computador. Para isso abra o terminal no diretório em que deseja armazenar o código e execute o comando abaixo.

```
git clone https://github.com/leandrocgsi/jsf-hibernate-spring-security-archetype.git
```

Abra a source folder gerado. Ele deverá se parecer com a imagem abaixo.

![OpenFolder](https://github.com/leandrocgsi/erudio-rest-api-archetype/blob/master/img/1-OpenFolder.png?raw=true)

Abra o terminal nessa pasta e execute o seguinte comando.

```
mvn clean install
```
Ele deve se parecer com a imagem abaixo

![CleanInstall](https://github.com/leandrocgsi/erudio-rest-api-archetype/blob/master/img/2-CleanInstall.png?raw=true)

Agora vá até o diretorio em que deseja criar o seu projeto e execute o seguinte comando.

```
mvn archetype:generate -DarchetypeGroupId=br.com.semeru
	-DarchetypeArtifactId=jsf-hibernate-spring-security-archetype
	-DarchetypeVersion=0.1.0
	-DgroupId=br.com.erudio
	-DartifactId=erudio-jsf-maven
```

Ele deve se parecer com a imagem abaixo.

![GenerateProject](https://github.com/leandrocgsi/erudio-rest-api-archetype/blob/master/img/3-GenerateProject.png?raw=true)

O Maven irá lhe perguntar se você deseja alterar a versão do seu projeto e a estrutura de pacotes como está destacado na imagem abaixo. Se você não quiser alterar nada apenas digite Enter Enter. Se tudo tiver corrido bem você deverá ver uma imagem similar à que se segue e isso significa que o seu projeto foi criado com sucesso ;-)

![Building1](https://github.com/leandrocgsi/erudio-rest-api-archetype/blob/master/img/4-Building.png?raw=true)

Agora só precisamos importar nosso projeto na nossa IDE favorita (Spring Suource Tool Suite - STS baseada no Eclipse no meu caso). Acesse o menu File >> Import >> Maven >> Existing Maven Projects >> Next.

![Importing1](https://github.com/leandrocgsi/erudio-rest-api-archetype/blob/master/img/9-Importing.png?raw=true)

Como na imagem abaixo digite ou navegue até o diretório onde se encontra o seu código e clique em Browse >> Finish.

![Importing2](https://github.com/leandrocgsi/erudio-rest-api-archetype/blob/master/img/10-Importing.png?raw=true)

Probably you see the following errors, dont be worry just click in Finish again.

![Importing3](https://github.com/leandrocgsi/erudio-rest-api-archetype/blob/master/img/11-Importing.png?raw=true)

Now we dont see our Groovy code this is because these code is out of default Maven lifecycle. To fix this we just need click with right button over our project and select New >> Source Folder.

![CreatingSourceFolders1](https://github.com/leandrocgsi/erudio-rest-api-archetype/blob/master/img/12-CreatingSourceFolders.png?raw=true)

In next window in Folder Name type *src/main/groovy*, repeat this proccess with *src/test/groovy* and *src/test_components/java*

![CreatingSourceFolders2](https://github.com/leandrocgsi/erudio-rest-api-archetype/blob/master/img/13-CreatingSourceFolders-CreatingSourceFolders.png?raw=true)

Now we have one structure similar to image bellow. As you can see, on *Markers tab*, we have some erros but dont be worry just click with right button and delete they.

![Final](https://github.com/leandrocgsi/erudio-rest-api-archetype/blob/master/img/14-Final.png?raw=true)

Now to execute your project [click here](https://github.com/leandrocgsi/semeru_jsf_maven)and follow the steps.
