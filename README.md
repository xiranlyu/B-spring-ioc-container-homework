@Component已经可以支持声明一个bean了，为何还要再弄个@Bean出来？

@Component注释在类上。通过类路径扫描自动检测bean并注入到Spring容器中。

@Bean不能注释在类上，只能用于在配置类中显式声明单个bean，让Spring要按照该方式去获取这个bean。
它将bean的声明与类定义分离，可以精确地创建和配置bean。