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
```java
import java.io.*;
import java.util.*;
public class SortNumbers
{
int i,j,temp,n;
int a[]=new int[100];
public void getInput() throws Exception
{
DataInputStream dr=new DataInputStream(System.in);
System.out.println("Enter how many Numbers to sort");
n=Integer.parseInt(dr.readLine());
System.out.println("Enter the Numbers ");
for(i=0;i<n;i++)
{
a[i]=Integer.parseInt(dr.readLine());
}
System.out.println("Numbers before Sorting");
for(i=0;i<n;i++)
{
System.out.println(a[i]);
}
}
public void sort()
{
for(i=0;i<n;i++)
{
for(j=0;j<n;j++)
{
if(a[i]<a[j])
{
temp=a[i];
a[i]=a[j];
a[j]=temp;
}
}
}
}
public void dispResult()
{
System.out.println("The Sorted Numbers in ascending order are");
{
System.out.println(a[i]);
}
}
public static void main(String args[]) throws Exception
{
SortNumbers s=new SortNumbers();
s.getInput();
s.sort();
s.dispResult();
}
}
```

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
```java
import java.util.*;
import java.io.*;
public class FindReplaceText
{
int i,j,n;
String[] s1=new String[20];
String s2,s3;
DataInputStream dr=new DataInputStream(System.in);
public void getInput() throws Exception
{
System.out.println("Enter Number of strings");
n=Integer.parseInt(dr.readLine());
System.out.println("Enter strings");
for(i=0;i<n;i++)
{
s1[i]=dr.readLine();
}
}
public void findText() throws Exception
{
boolean val=false;
System.out.println("Enter the String to Search");
s2=dr.readLine();
for(i=0;i<n;i++)
{
val=s1[i].equals(s2);
if(val==true)
{
break;
}
}
if(val==true)
System.out.println("String Found");
else
System.out.println("String not Found");
}
public void replaceText() throws Exception
{
boolean val=false;
System.out.println("Enter the String to Search and Replace");
System.out.println("String to Search");
s2=dr.readLine();
System.out.println("String to Replace");
s3=dr.readLine();
for(i=0;i<n;i++)
{
val=s1[i].equals(s2);
if(val==true)
{
s1[i]=s3;
break;
}
}
if(val==true)
{
System.out.println("String Found and replaced");
}
else
System.out.println("String not Found");
}
public static void main(String args[]) throws Exception
{
FindReplaceText fr=new FindReplaceText();
fr.getInput();
fr.findText();
fr.replaceText();
}
}

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
