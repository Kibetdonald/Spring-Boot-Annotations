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
@GetMapping

# 1. @crossorigin
It enables cross-origin resource sharing only for this specific method. By default, its allows all origins, all headers, and the HTTP methods specified in the @RequestMapping annotation

## Syntax
```
@CrossOrigin(origins = "http://localhost:8080")
```
# 2. @Bean
The @Bean annotations are used at the method level and indicate that a method produces a bean that is to be managed by the Spring container. It is an alternative to the XML<bean> tag. 

## Syntax:
```
 @Bean
Public BeanExample beanExample ()
{
return new BeanExample (),
}
```
# 3. @Service
It is used at the class level. It shows that the annotated class is a service class, such as business basic logic, and call external APIs.
## Syntax
 ```
public class TestService
{
public void service1()
{
// business logic
}
}
 ```
# 4 .Repository
It is a Data Access Object (DAO) that accesses the database directly. It indicates that the annotated class is a repository. 
The repository annotation indicates the class has the capability of storage, retrieval, updating, deletion, and search
## Syntax
```
 @Repository

public class TestRepository
{
public void delete()
{
// persistence code
}}
```
# 5. @Configuration
 Tags the class as a source of bean definitions for the application context. @EnableAutoConfiguration : Tells Spring Boot to start adding beans based on classpath settings, other beans, and various property settings.
 
 ## Syntax
 ```
 @Configuration
public class Bus
{
@BeanBus engine()
{
return new Bus();
}
}
 ```
 # 6. @ Controller
 The annotation is used to indicate that the class is a web request handler. It is often used to present web pages. It goes hand in hand with @RequestMapping annotation
 
 ## Syntax
```
 @Controller
@RequestMapping(“cars”)
public class CarsController
{
@RequestMapping(value= “/{name}”, method= RequestMethod.GET)
public Employee getCarsByName()
{
Return carsTemplate;
}
}
 ```
# 7. @RequestMapping
 It is used to map the HTTP Request. It also has many other optional elements like consumes, name, method, request, path, etc. 
 
 ## Syntax
 ```
 @Controller
public class FlowersController
{
@RequestMapping (“/red-colour/flowers”)
public String getAllFlowers(Model model)
{
//application code
return “flowerlist”;
}
 ```
 
 # 8. @Autowired
 This annotation is used to auto-wire spring bean on setter methods, constructor and instance variable. It injects object dependency implicitly. When we use this annoation, the spring container auto-wires the bean by its matching data type.
 ```
 ## Syntax
 @Component
public class Employee
private Person person;
@Autowired
public Employee(Person person)
{
this.person=person
}
}
 ```
 # 9. @SpringBootApplication
 It consists of @Configuration, @ComponentScan, and @EnabeAutoConfiguration. The class annotated with @SpringBootApplication is kept in the base package. This annotation does the component scan. However, only the sub-packages are scanned. 

# 10.  @GetMapping annotation 
 Indicates that the function processes a GET request.
 
# 11. @PostMapping annotation
 Indicates that a function processes a POST request.
 
# 12. @PutMapping annotation 
 Indicates that a function processes a PUT request.
 
# 13. @DeleteMapping annotation 
 Indicates that a function processes a DELETE request.
 
