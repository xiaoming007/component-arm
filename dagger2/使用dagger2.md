# 依赖注入
### 提供依赖类的方式
* 1.对于自己完全可控的类，可以使用构造函数注入的方式，也就是使用@Inject注解构造函数  
* 2.对于像Activity，等这种有系统启动调用的，可以使用@Module然后通过provider的形式提供  

### 使用@component
* 1.通过接口中定义的方法与返回类型，来提供你想要创建的对象，并且会生成一个容器，这个容器会通过图去创建其所有的依赖项。  
* 2.通过inject方法，来确认将这个组建使用在哪里。
* 3.通过 @Inject lateinit var loginViewModel: LoginViewModel这个方式向不能通过构造函数注入的类中注入依赖，例如activity  



