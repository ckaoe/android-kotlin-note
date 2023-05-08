# 类的讲解

class InitOrderDemo(name: String)-(name: String)：是一个构造函数。

```kotlin
class InitOrderDemo(name: String){
    // .also(::println)能使用println的
    val firstProperty = "First propert: $name".also(::println)
    // 相当于构造函数中的代码，可以直接被执行。
    init {
        println("first initializer block thatprints $name")
    }
    val secondProperty = "second property: ${name.length}".also ( ::println )

    init {
        println("second initializer block that prints ${name.length}")
    }
}

fun main(){
    InitOrderDemo("hello wrold")
}
```
