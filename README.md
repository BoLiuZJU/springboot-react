# springboot-react
可访问正常访问一般页面，但是react的页面始终为空白，我的步骤如下
1\依次安装
vscode
https://code.visualstudio.com/
jdk
https://adoptopenjdk.net/
java
2\新建一个springboot项目
在面板中输入maven
选中spring initializr: Create Maven project
选中一个springboot版本，选中java语言，然后按提示对文件命名，选中一个文件放置位置，就成功建立了一个springboot项目
3\在springboot中引入web包与themeleaf依赖（pom.xml）
web
<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>
    
themeleaf
<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-thymeleaf</artifactId>
		</dependency>
	</dependencies>
  
到这一步编写controller可以正常访问页面了
4\建立react项目然后将其build，指定 homepage='.'
5\将build的整个文件夹拷贝到springboot项目的resources/public文件夹中，
6、使用controller访问页面，页面为空白
