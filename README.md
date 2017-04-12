# springboot
This repo contains all the knowledge to use springboot to create end to end applications.


What is Spring Boot?
SpringBoot makes it easy to create a standalone, production grade spring based applications
that you can "just run"


What do springboot applications look like?
Spring boot is
1. opinionated
2. Convention over configuration
3. Standalone - just run a command and starts a standalone application.
3. Production Ready


Springboot startup steps
1. Sets up default configuration from the spring boot parent
2. Starts spring application context
3. Performs class path scan
4. Starts Tomcat Server


Setup Dev Environment
1. have java sdk
2. create a simple maven project.
3. add parent spring boot dependency. Configuration is defined in parent project. Our Project will inherit all configurations from parent.
	Convention over configuration
	<parent>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-parent</artifactId>
		<version>1.5.2.RELEASE</version>
	</parent>
	
4. Add below dependency. this will download all the jars required for a web application.
	<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
			<version>1.5.2.RELEASE</version>
		</dependency>
5.  Create a simple java class with main method. Add @SpringBootApplication annotation. in main method add SpringApplication.run(ClassName.class, args);
6. Done. Your spring boot application is ready. run it using JavaApplication.
7. Or from command line using, 


References
https://www.youtube.com/watch?v=9Pl4rlVAoOc&list=PLqq-6Pq4lTTbx8p2oCgcAQGQyqN8XeA1x&index=2


 
