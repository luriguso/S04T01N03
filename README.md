# 🚀 Level 3 - Postman Exercise

📄 **Description - Exercise Statement**

This exercise focuses on testing the previous Spring Boot projects (**Maven** and **Gradle**) with **Postman**.
You will create two different environments in Postman, configure variables, and make API calls to verify that both applications respond correctly.

---

## 💻 **Objective**

- Learn how to use **Postman environments** to test REST APIs.
- Test the **HelloWorld** endpoints of Maven and Gradle projects.
- Demonstrate that both servers respond correctly when running simultaneously on different ports.

---

## ⚙️ **Postman Configuration**

### 🌐 Create two environments:

1. **Maven Project**
2. **Gradle Project**

Each environment must include the following variables:

| Variable | Value (Maven) | Value (Gradle) | Description |
|-----------|---------------|----------------|--------------|
| `server` | `http://localhost` | `http://localhost` | Server base URL |
| `port` | `9000` | `9001` | Server port number |

---

## 🔧 **URL Example with Environment Variables**

You can test endpoints with the following dynamic URL format:

```
{{server}}:{{port}}/HelloWorld/MyName
```

### ✅ Example Results

- **Maven Project (port 9000):**
```
Hello, MyName. You are running a Maven project.
```

- **Gradle Project (port 9001):**
```
Hello, MyName. You are running a Gradle project.
```

---

## ▶️ **How ​​to test**

1. Run both projects from **IntelliJ** (or Eclipse):
- `S04T01N01` → Maven Project (port **9000**)
- `S04T01N02` → Gradle Project (port **9001**)

2. Open **Postman** and create the two environments described above.

3. Select one environment at a time and execute a `GET` request to:
```
{{server}}:{{port}}/HelloWorld/MyName
```

4. Verify that each project responds correctly with its corresponding message.

---

## 🧠 **Important Notes**

- Make sure both applications are **running simultaneously** on their respective ports.
- Use **environment variables** in Postman instead of hardcoding URLs.
- Verify that responses match the expected message for each project.

- ---

## ✍️ **Author**

Developed by [Luriguso](https://github.com/luriguso)
Part of the educational sprint at **IT Academy**