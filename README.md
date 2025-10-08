# 🚀 Nivel 3 - Ejercicio de Postman

📄 **Descripción - Enunciado del Ejercicio**

Este ejercicio se centra en probar los proyectos anteriores de Spring Boot (**Maven** y **Gradle**) con **Postman**.
Crearás dos entornos diferentes en Postman, configurarás variables y realizarás llamadas a la API para verificar que ambas aplicaciones respondan correctamente.

---

## 💻 **Objetivo**

- Aprender a usar los **entornos de Postman** para probar las API REST.
- Probar los **endpoints HelloWorld** de los proyectos Maven y Gradle.
- Demostrar que ambos servidores responden correctamente al ejecutarse simultáneamente en puertos diferentes.

---

## ⚙️ **Configuración de Postman**

### 🌐 Crear dos entornos:

1. **Proyecto Maven**
2. **Proyecto Gradle**

Cada entorno debe incluir las siguientes variables:

| Variable | Valor (Maven) | Valor (Gradle) | Descripción |
|-----------|---------------|----------------|--------------|
| `servidor` | `http://localhost` | `http://localhost` | URL base del servidor |
| `puerto` | `9000` | `9001` | Número de puerto del servidor |

---

## 🔧 **Ejemplo de URL con variables de entorno**

Puedes probar los endpoints con el siguiente formato de URL dinámica:

```
{{servidor}}:{{puerto}}/HolaMundo/MiNombre
```

### ✅ Resultados del ejemplo

- **Proyecto Maven (puerto 9000):**
```
Hola, MiNombre. Estás ejecutando un proyecto Maven.
```

- **Proyecto Gradle (puerto 9001):**
```
Hola, MiNombre. Estás ejecutando un proyecto Gradle.
```

---

## ▶️ **Cómo probar**

1. Ejecuta ambos proyectos desde **Eclipse** (o IntelliJ):
- `S04T01N01` → Proyecto Maven (puerto **9000**)
- `S04T01N02` → Proyecto Gradle (puerto **9001**)

2. Abre **Postman** y crea los dos entornos descritos anteriormente.

3. Selecciona un entorno a la vez y ejecuta una solicitud `GET` a:
```
{{servidor}}:{{puerto}}/HelloWorld/MyName
```

4. Verifica que cada proyecto responda correctamente con su mensaje correspondiente.

---

## 📦 **Qué entregar**

Debes enviar **4 archivos en total**:

| Tipo de archivo | Descripción |
|------------|-------------|
| `MavenEnvironment.json` | Entorno de Postman exportado para el proyecto Maven |
| `GradleEnvironment.json` | Entorno de Postman exportado para el proyecto Gradle |
| `Maven_Test_Screenshot.png` | Captura de pantalla que muestra la ejecución del entorno Maven en Postman |
| `Gradle_Test_Screenshot.png` | Captura de pantalla que muestra la ejecución del entorno Gradle en Postman |
---
## 🧠 **Notas importantes**

- Asegúrese de que ambas aplicaciones se **ejecuten simultáneamente** en sus respectivos puertos.
- Use las **variables de entorno** en Postman en lugar de codificar las URL.
- Verifique que las respuestas coincidan con el mensaje esperado de cada proyecto.

- ---

## ✍️ **Autor**

Desarrollado por [Luriguso](https://github.com/luriguso)
Parte del sprint educativo en **IT Academy**