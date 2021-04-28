# Kotlin/Native
The technology used to bring Kotlin beyond the JVM. Allows you to compile Kotlin code outside of virtual machines, resulting in

## Konan and LLVM


![](images/konan.png)

## Kotlin Standard Library
When compiling with Kotlin/Native, the executable file can be larger due to the fact that the Kotlin standard library is statically linked in to the executable file.

# Kotlin Multiplatform
With the size of an app, the amount of code duplication grows essentially linearly as would the

<div style="text-align:center"><img src="images/duplication.png" width="90%"/></div>

## Sharing Code
Reduce the amount of duplication by putting common logic and functionality into one module or shared project. The shared module includes business logic,and things like networking code, data parsing, data peristence, and more.

<div style="text-align:center"><img src="images/shared_module.png" width="80%"/></div>

## Expect/Actual Mechanism

<div style="text-align:center"><img src="images/expect_actual.png" width="80%"/></div>


## Other Cross-Platform Frameworks

* poor performance of the resulting apps
* inconsistencies with the native user interfaces
* an inability to stay up-to-date with the latest iOS and Android features
* developer loyalty to and expertise with the native SDK


* On a larger app you can divide your team up into groups that work in different areas - shared module, Android/IOS UI

# Technologies & Libraries
* MOKO - share resources and architecture components such as ViewModel, [template](https://github.com/icerockdev/moko-template)
* SQLDelight - local data storing
* Kotlin Serialization - parsing
* Ktor - networking
* [FirestoreKMP](https://github.com/touchlab-lab/FirestoreKMP) - library wrapping the Firestore operations to use in shared module
* Koin (or Kodein) - dependency injection

# Sources
* Oficial documentation - [overview](https://kotlinlang.org/docs/multiplatform.html), [intro](https://kotlinlang.org/docs/mpp-intro.html), [getting started](https://kotlinlang.org/docs/mobile/getting-started.html), [hands on](https://play.kotlinlang.org/hands-on/Networking%20and%20Data%20Storage%20with%20Kotlin%20Multiplatfrom%20Mobile/01_Introduction): networking and data storage
* Ktor server in KotlinKonf app - [project](https://github.com/JetBrains/kotlinconf-app)
* KMP with MVI in DroidKaigi app - [project](https://github.com/DroidKaigi/conference-app-2021#Tech-Stacks)
* KMP with MVVM and Clean architecture (Moko for shared ViewModel) - [article](https://proandroiddev.com/kotlin-multiplatform-mvvm-clean-architecture-f20b99f90b95), [project](https://github.com/jarroyoesp/KotlinMultiplatform_MVVM)
* KMP with MVP and Clean architecture - [article](https://proandroiddev.com/clean-architecture-example-with-kotlin-multiplatform-c361bb283fd0)
* KMP with MVVM and Firebase in shared module - [article](https://proandroiddev.com/kotlin-multiplatform-firebase-mvvm-4cdcddd98893), [project](https://github.com/jarroyoesp/KotlinMultiplatform_Firebase_MVVM)
* KMP IceRock [codelabs](https://codelabs.kmp.icerock.dev)

### Included in this document
* Ray Wenderlich - Kotlin Apprentice - Section IV/Chapter 26 - [book](https://www.raywenderlich.com/books/kotlin-apprentice/v2.0/)

