# Tutorial 5 Arrays

1.  Write statements for each of the following
    a.  Declare an array that used to store 12 floating point numbers. 
2.  float[] array = new float[12];
    b.  Initialize an array that used to store the value of A to E. 
3. char[] array = {'A', 'B', 'C', 'D', 'E'};
    c.  Declare an array that used to store 100 students name.  
4. String[] students = new String[100];
    d.  Declare an array for a table with 6 rows 2 columns that used to store integer value.  
5. int[][] table = new int[6][2];
    e.  Initialize an array with the following value:  
6. int[] array = {1, 2, 3, 4, 5, 6};
	```math
	\begin{pmatrix}
	6 & 9 \\
	2 & 5 \\
	4 & 6
	\end{pmatrix}
	```


    f.  After initialize the array, modify the value of the above array to  
	```math
	\begin{pmatrix}
	6 & 9 \\
	2 & 4 \\
	3 & 7
	\end{pmatrix}
	```
    g.  Display all the values of an array name contact in separate lines.

	---
    

1.  Correct the error for the following statements.   

	a.
	```java
	String[] code = {"AAA", "AAB", "AAC", "AAD"};
	```
	   
	  b.
	```java
	int[] num = new int[10]; 
	for(int k=0; k<=num.length(); k++) 
	sum+=num;
	```
	c.
	```java
	int [][]t = new int[3][10]; 
	t[1][2] = 5;
	```
	d.
	```java
	int i = 4;
	int []score = new int[6];
	score[1] = 78;
	score[++i] = 100;
	```
 ---

2.  Determine the values of each element of array marks. Assume the array was declared as:  
    ```java
    int[] marks = new int[5];
    int i = 0, j = 1;
    marks[i] = 12;
    marks[j] = marks[i] + 19;
    marks[j-1] = marks[j] * marks[j];
    marks[j*3] = marks[i+1];
    marks[++j] = marks[i] % 5;
    marks[2*j] = marks[j-1];
    [961,31,1,31,31]
    ```

---

3.  Write the statements that display the number of occurrence of the word "the" (case sensitive) in a string array name sentence.  
    String[] sen = {"the","sun","is","on","the","sky"}
4. for(int i =0;i<=sen.length;i++)
5. if (sentence[i].equals("the")) {
   count++;}
6. System.out.print(count)
---

4.  Write the statements that display the string array name sentence in reverse order. Each string element must be displayed in reverse order as well.  

---String[] sen=["apple","banana","cat"]
for (int i = sentence.length - 1; i >= 0; i--) {
String a = sentence[i];
String b = "";

    for (int j = a.length() - 1; j >= 0; j--) {
        reversed += a.charAt(j);
    }

    System.out.println(b);
}
5.  Write the statements that generate 1 random integer within 0-255. Convert the number to binary and store the bit into an 8-bit array. Then, display the binary number.  
import java.util.*;
6. Random ran =new Random();
   int s = ran.nextInt(256);
   System.out.println(s);
   int[] adf=new int[8];
   String binary = String.format("%8s", Integer.toBinaryString(s)).replace(" ","0");
   for (int i = 0; i < binary.length(); i++) {
   adf[i] = binary.charAt(i) - '0';  
   }
   System.out.println(binary);
6. 