# Spring-Boot-Annotations

|In this article, you will learn Spring Boot Annotations like
@crossorigin
@Bean
@Service
@Repository
@Configuration
@Controller
@RequestMapping
@Autowired
@Component
@SpringBootApplication
@EnableAutoConfiguration


# 1. @crossorigin
It enables cross-origin resource sharing only for this specific method. By default, its allows all origins, all headers, and the HTTP methods specified in the @RequestMapping annotation

##Syntax
@CrossOrigin(origins = "http://localhost:8080")

# 2. @Bean
The @Bean annotations are used at the method level and indicate that a method produces a bean that is to be managed by the Spring container. It is an alternative to the XML<bean> tag. 

## Syntax:
@Bean
Public BeanExample beanExample ()
{
return new BeanExample (),
}

# 3. @Service
It is used at the class level. It shows that the annotated class is a service class, such as business basic logic, and call external APIs.
##Syntax
public class TestService
{
public void service1()
{
// business logic
}
}
# 4 .Repository
It is a Data Access Object (DAO) that accesses the database directly. It indicates that the annotated class is a repository. 
The repository annotation indicates the class has the capability of storage, retrieval, updating, deletion, and search
## Syntax
@Repository

public class TestRepository
{
public void delete()
{
// persistence code
}}

#5. @Configuration
 Tags the class as a source of bean definitions for the application context. @EnableAutoConfiguration : Tells Spring Boot to start adding beans based on classpath settings, other beans, and various property settings.
 
 ## Syntax
 @Configuration
public class Bus
{
@BeanBus engine()
{
return new Bus();
}
}
