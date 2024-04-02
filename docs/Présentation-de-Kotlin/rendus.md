---
layout: default
chapitre: Présentation de Kotlin
order: 2
---

<!-- new slide -->

# Présentation de Kotlin

<!-- new slide -->

## Exécuter votre premier programme


Vous avez besoin d'un outil appelé compilateur Kotlin, qui convertit le code Kotlin que vous avez écrit ligne par ligne afin de le traduire en un langage compréhensible par l'ordinateur. Ce processus est la compilation de votre code.

```bash
fun main() {
    println("Hello, world!")
}
```

En bas de l'éditeur de code, vous devriez voir un volet qui affiche la sortie, ou le résultat de votre programme :

```bash
Hello, world!
```
<!-- new slide -->

## Variables et types de données



| Type de données Kotlin | Types de données qu'il peut contenir | Exemples de valeurs littérales |
|------------------------|---------------------------------------|--------------------------------|
| String                 | Texte                                 | "Add contact" / "Search" / "Sign in" |
| Int                    | Nombre entier                          | 32  /  1293490  / -59281         |
| Double                 | Nombre décimal                        | 2.0 / 501.0292  / -31723.99999    |
| Float                  | Nombre décimal (moins précis qu'un Double), suivi de f ou F. | 5.0f / 1.2940278F / -1630.209f|
| Boolean                | true ou false. Utilisez ce type de données quand il n'y a que deux valeurs possibles. Notez que true et false sont des mots clés en Kotlin. | true false|

<!-- new slide -->

## Examples

```bash
fun main() {
    val count : Int = 2
    println(count)
}

fun main() {
    val count: Int = 2
    println("You have $count unread messages.")
}

fun main() {
    birthdayGreeting()
    println(birthdayGreeting())
}

fun birthdayGreeting(): String {
    val nameGreeting = "Happy Birthday, Rover!"
    val ageGreeting = "You are now 5 years old!"
    return "$nameGreeting\n$ageGreeting"
}

fun main() {
    birthdayGreeting()
}

fun birthdayGreeting(): Unit {
    println("Happy Birthday, Rover!")
    println("You are now 5 years old!")
}

fun main() {
    birthdayGreeting("Ahmed")
    println(birthdayGreeting("Ahmed"))
}
fun birthdayGreeting(name: String): String {
    val nameGreeting = "Happy Birthday, $name!"
    val ageGreeting = "You are now 5 years old!"
    return "$nameGreeting\n$ageGreeting"
}

fun main() {
    birthdayGreeting("Ahmed",24)
    println(birthdayGreeting("Ahmed",24))
}

fun birthdayGreeting(name: String, age: Int): String {
    val nameGreeting = "Happy Birthday, $name!"
    val ageGreeting = "You are now $age years old!"
    return "$nameGreeting\n$ageGreeting"
}

```