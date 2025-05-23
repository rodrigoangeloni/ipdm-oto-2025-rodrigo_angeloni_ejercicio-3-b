# ✅ Task Manager App - Ejercicio 3

[![Kotlin](https://img.shields.io/badge/Kotlin-1.9.0-blue.svg)](https://kotlinlang.org)
[![Compose](https://img.shields.io/badge/Jetpack%20Compose-1.6.0-brightgreen)](https://developer.android.com/jetpack/compose)

Aplicación Android que muestra una pantalla de confirmación cuando se completan todas las tareas diarias, desarrollada con Jetpack Compose.

<div align="center">
  <img src="app/src/main/res/drawable-nodpi/captura_ejercicio_3_b.png" width="200" alt="Pantalla de tareas completadas">
</div>

## ✨ Características
- Diseño 100% declarativo con Jetpack Compose
- Imagen personalizada `ic_task_completed` integrada
- Textos con estilos Material Design 3
- Previsualización interactiva con `@Preview`
- Totalmente responsive para distintos dispositivos

## 🛠 Tecnologías utilizadas
- **Lenguaje**: Kotlin
- **UI Toolkit**: Jetpack Compose
- **Arquitectura**: ComponentActivity + Composable
- **Compatibilidad**: Android 7.0+ (API 24)

## 🎨 Componentes principales
```kotlin
@Composable
fun TaskCompletedScreen() {
    Column(
        verticalArrangement = Arrangement.Center,
        horizontalAlignment = Alignment.CenterHorizontally
    ) {
        Image(
            painter = painterResource(R.drawable.ic_task_completed),
            contentDescription = "Tarea completada"
        )
        // Textos con estilos...
    }
}
