# 💻 Java-CMD-Programs

This repository contains 8 basic Java programs that can be compiled and executed using Command Prompt (CMD).

---

## 🔧 Requirements

- Java JDK installed
- Windows Command Prompt (CMD)

Check Java installation:

```cmd
java -version
javac -version
```

If version is displayed, Java is installed successfully.

---

# 📂 How to Run the Programs in CMD

## Step 1️⃣ : Create a Folder in Any Drive

Open CMD and type:

```cmd
D:
mkdir JavaPrograms
cd JavaPrograms
```

Now save all `.java` files inside this folder.

---

# 1️⃣ Sort Numbers Program

## Save File As:
```
SortNumbers.java
```

## Compile:
```cmd
javac SortNumbers.java
```

## Run:
```cmd
java SortNumbers
```

---

# 2️⃣ Find & Replace Program

## Save File As:
```
FindReplaceText.java
```

## Compile:
```cmd
javac FindReplaceText.java
```

## Run:
```cmd
java FindReplaceText
```

---

# 3️⃣ Calculator Program

## Save File As:
```
Calc.java
```

## Compile:
```cmd
javac Calc.java
```

## Run:
```cmd
java Calc
```

---

# 4️⃣ Area of Rectangle (Constructor)

## Save File As:
```
AreaRect.java
```

## Compile:
```cmd
javac AreaRect.java
```

## Run:
```cmd
java AreaRect
```

---

# 5️⃣ Student Grade Program

## Save File As:
```
StudentGrade.java
```

## Compile:
```cmd
javac StudentGrade.java
```

## Run (Command Line Arguments Required):
```cmd
java StudentGrade 101 SUBHA 99 90 67 78 89
```

Format:
```
java StudentGrade RollNo Name M1 M2 M3 M4 M5
```

---

# 6️⃣ Draw Objects (Inheritance & Polymorphism)

## Save File As:
```
DrawObjects.java
```

## Compile:
```cmd
javac DrawObjects.java
```

## Run:
```cmd
java DrawObjects
```

---

# 7️⃣ Multiple Inheritance Using Interface

## Save File As:
```
MultipleInheritanceUsingInterface.java
```

## Compile:
```cmd
javac MultipleInheritanceUsingInterface.java
```

## Run:
```cmd
java MultipleInheritanceUsingInterface
```

---

# 8️⃣ Thread with Priority

## Save File As:
```
TestMultiPriority1.java
```

## Compile:
```cmd
javac TestMultiPriority1.java
```

## Run:
```cmd
java TestMultiPriority1
```

---

# 🚀 Compile All Programs at Once

```cmd
javac *.java
```

Run any program:

```cmd
java ClassName
```

Example:

```cmd
java SortNumbers
```

---

# 📁 Project Structure

```
JavaPrograms/
│
├── SortNumbers.java
├── FindReplaceText.java
├── Calc.java
├── AreaRect.java
├── StudentGrade.java
├── DrawObjects.java
├── MultipleInheritanceUsingInterface.java
├── TestMultiPriority1.java
└── README.md
```

---

✅ Important Notes:

- File name must match the public class name
- Always compile before running
- Make sure CMD is inside correct folder
- Use `dir` command to check files

---

👨‍💻 Author: Ranjith Kumar p  
📌 Basic Java Programs using CMD
