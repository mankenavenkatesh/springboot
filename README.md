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


Adding Web Components using Spring MVC.
1. Spring MVC provides annotations to create REST Endpoints.
https://www.youtube.com/watch?v=oRFCeRVWCNE&index=11&list=PLqq-6Pq4lTTbx8p2oCgcAQGQyqN8XeA1x


Behind the scenes
1. parent dependency will pull just the configuration. it will tell what version of dependency jars to use.
2. 


Spring MVC
1. @RestController - Tells it's a rest controller. Rest Controller by default converts response to JSON type.
2. @RequestMapping - Defines path
3. @Service - Stereotype annotation. This marks class as spring business service. spring will create singleton instances of business services on bootup. it will register. 
				if any dependency controller asks for service, spring will inject the existing spring instance.
4. 				

References
https://www.youtube.com/watch?v=9Pl4rlVAoOc&list=PLqq-6Pq4lTTbx8p2oCgcAQGQyqN8XeA1x&index=2


 
