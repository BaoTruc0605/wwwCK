# wwwCK
application.template

spring.datasource.driver-class-name=org.mariadb.jdbc.Driver
spring.datasource.url=jdbc:mariadb://localhost:3306/week7?createDatabaseIfNotExist=true
spring.datasource.username=root
spring.datasource.password=sapassword
spring.jpa.hibernate.ddl-auto=update




spring.datasource.driver-class-name=org.mariadb.jdbc.Driver
spring.datasource.url=jdbc:mariadb://localhost:3306/onckSecurity?createDatabaseIfNotExist=true
spring.datasource.username=root
spring.datasource.password=sapassword
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true


spring.h2.console.enabled=true
#spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.security.user.name=truc
spring.security.user.password=truc

spring.main.allow-circular-references=true




build gradle
dependencies {
	implementation 'net.datafaker:datafaker:2.0.2'
    implementation 'org.springframework.boot:spring-boot-starter-data-jpa'
    implementation 'org.springframework.boot:spring-boot-starter-security'
    implementation 'org.springframework.boot:spring-boot-starter-thymeleaf'
    implementation 'org.springframework.boot:spring-boot-starter-web'
    implementation 'org.thymeleaf.extras:thymeleaf-extras-springsecurity6'
    implementation 'org.springframework.session:spring-session-core'
    compileOnly 'org.projectlombok:lombok'
    runtimeOnly 'com.h2database:h2'
    developmentOnly 'org.springframework.boot:spring-boot-devtools'
    runtimeOnly 'org.mariadb.jdbc:mariadb-java-client'
    annotationProcessor 'org.projectlombok:lombok'
    testImplementation 'org.springframework.boot:spring-boot-starter-test'
    testImplementation 'org.springframework.security:spring-security-test'
    implementation 'com.neovisionaries:nv-i18n:1.29'
    implementation 'org.springframework.data:spring-data-rest-core:4.1.4'

}
