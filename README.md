# wwwCK
application.template

spring.datasource.driver-class-name=org.mariadb.jdbc.Driver
spring.datasource.url=jdbc:mariadb://localhost:3306/week7?createDatabaseIfNotExist=true
spring.datasource.username=root
spring.datasource.password=sapassword
spring.jpa.hibernate.ddl-auto=update

build gradle
dependencies {
	implementation 'net.datafaker:datafaker:2.0.2'
	implementation 'org.springframework.boot:spring-boot-starter-data-jpa'
	implementation 'org.springframework.boot:spring-boot-starter-thymeleaf'
	implementation 'org.springframework.boot:spring-boot-starter-web'
	implementation 'org.springframework.session:spring-session-core'
	compileOnly 'org.projectlombok:lombok'
	developmentOnly 'org.springframework.boot:spring-boot-devtools'
	runtimeOnly 'org.mariadb.jdbc:mariadb-java-client'
	annotationProcessor 'org.projectlombok:lombok'
	testImplementation 'org.springframework.boot:spring-boot-starter-test'
	//for country code
	implementation 'com.neovisionaries:nv-i18n:1.29'
	//For database REST
	implementation 'org.springframework.data:spring-data-rest-core:4.1.4'
	testImplementation 'org.springframework.security:spring-security-test'
}
