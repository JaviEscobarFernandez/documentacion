##### Ternary operator (sustitución)
```kt
val resultado = if (condicion) "Verdadero" else "Falso"
```

##### Data class
```kt
data class User(
    val id: String = "",
    val name: String = "",
    val isAdmin: Boolean = false
)

// uso posterior
val usuario = User("21mfr", "Javi", true)
```
