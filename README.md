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
```
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
```java
public class Calc
{
int a=10,b=5,c;
public void add()
{
c=a+b;
System.out.println("The Result of add "+c);
}
public void sub()
{
c=a-b;
System.out.println("The Result of Subraction "+c);
}
public void mult()
{
c=a*b;
System.out.println("The Result of Multiplication "+c);
}
public void div()
{
c=a/b;
System.out.println("The Result of Division "+c);
}
public void modulo()
{
c=a%b;
System.out.println("The Result of Modulus "+c);
}
public void square()
{
c=a*a;
System.out.println("The Result of Square "+c);
}
public void cube()
{
c=a*a*a;
System.out.println("The Result of Cube "+c);
}
public static void main(String args[])
{
Calc c=new Calc();
c.add();
c.sub();
c.mult();
c.div();
c.modulo();
c.square();
c.cube();
}}
```
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
```java
import java.util.*;
import java.io.*;
public class AreaRect
{
int l,b,a;
AreaRect()
{
l=10;
b=10;
}
AreaRect(int l1,int b1)
{
l=l1;
b=b1;
}
void dispArea()
{
a=l*b;
System.out.println("The area for length lenght= "+l+"b="+b+" is "+a );
}
public static void main(String args[])
{
AreaRect ar1=new AreaRect();
AreaRect ar2=new AreaRect(20,20);
ar1.dispArea();
ar2.dispArea();
}
}
```
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
```java
public class StudentGrade
{
public static void main(String args[])
{
String name,grade="";
int rollno,m1,m2,m3,m4,m5,total,avg;
rollno=Integer.parseInt(args[0]);
name=args[1];
m1=Integer.parseInt(args[2]);
m2=Integer.parseInt(args[3]);
m3=Integer.parseInt(args[4]);
m4=Integer.parseInt(args[5]);
m5=Integer.parseInt(args[6]);
total=m1+m2+m3+m4+m5;
avg=total/5;
if(avg>=90)
{
grade="A";
}
else if(avg>70&&avg<90)
{
grade="B";
}
else if(avg>50&&avg<70)
{
grade="B";
}
System.out.println();
System.out.println("StudentName Rollno Total Percentage Grade");
System.out.println();
System.out.println(" "+name+" "+ rollno+" "+total+" "+avg+" +grade);
}
}
```
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
