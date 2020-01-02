元注解	描述
@Target	
表示该注解可以用于什么地方。可能的ElementType参数包括：

CONSTRUCTOR：构造器的生命

FIELD：域声明（包括enum实例）

LOCAL_VARIABLE：局部变量声明

METHOD：方法声明

PACKAGE：包声明

PARAMETER：参数声明

TYPE：类、接口（包括注解类型）和enum声明

ANNOTATION_TYPE：注解声明（与TYPE的区别？，专门用在注解上的TYPE）

TYPE_PARAMETER：Java8

TYPE_USE：Java8

@Retention	
表示需要在什么级别保存该注解信息。可选的RetentionPolicy参数包括：

SOURCE：注解将在编译器丢弃

CLASS：注解在class文件中可用，但会被VM丢弃

RUNTIME：VM将在运行期也保留注解，因此可以通过反射机制读取注解的信息

@Documented	将此注解包含在Javadoc中
@Inherited	允许子类继承父类中的注解
