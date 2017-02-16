# assignment-2.6
QN 1) Write a program to accepts two numbers from stdin and find all the odd as well as even
numbers present in between them.

public class acad {

public static void main(String[] args) {
    // TODO Auto-generated method stub
Scanner in=new Scanner(System.in); 
System.out.println("enter numbers between which you want to find odd and even(inclusive of those 2 numbers)"); 
int number1=in.nextInt();//getting input int number2=in.nextInt();
//getting input ArrayList odd=new ArrayList<>();//used arraylist as there is no size related problem; ArrayList even=new ArrayList<>();

for(int a=number1;a<=number2;a++)//running for loop {

if(a%2==0)//getting even numbers
{
    even.add(a);

}


if(a%2!=0)//getting odd numbers
{
    odd.add(a);
}
}
System.out.println("Even numbers between "+number1+" and "+number2);//printing even numbers for(int m=0;m<even.size();m++) { System.out.print(even.get(m)+" "); } System.out.println(); System.out.println("Odd numbers between "+number1+" and "+number2);//printing odd numbers for(int m=0;m<odd.size();m++) { System.out.print(odd.get(m)+" "); } } } 

QN 2) Joe is scared to go to school. When her dad asked the reason, joe said she is unable to
complete the task given by her teacher. The task was to find the “first 10 multiples” of the
number entered from stdin.



public class acad {

public static void main(String[] args) {
    // TODO Auto-generated method stub
Scanner in=new Scanner(System.in);
System.out.println("enter numbers between which joe want to find multiples"); 
int number1=in.nextInt();//getting input 
int sum=0; //since we want to find multiples first 10 multiples running a for loop and I am adding 10 times the given number 
for(int a=1;a<=10;a++) 
{ sum=sum+number1;
System.out.println(number1+"*"+a+"="+sum);//printing the tables
}
}

QN 3) Write a program consisting method sum() and demonstrate the concept of method
overloading using this method.


using this method OVERLOADING helps to modify the same method according to our wish.This helps in acheiving one of the concepts of OOPS "polymorphism" overloading could be done by changing 1. Number of parameters. 2. Data type of parameters. 3.Sequence of Data type of parameters.

public class acad {

public static void main(String[] args) {
    // TODO Auto-generated method stub
Scanner in=new Scanner(System.in);//scanner used for getting input from user through keybaord System.out.println("Enter name"); String name=in.next(); System.out.println("Enter marks"); int number1=in.nextInt();//getting input at runtime int number2=in.nextInt();//getting input at runtime int number3=in.nextInt();

acad a=new acad();//creating object a to call non staic method sum inside static method acad a1=new acad(); acad a2=new acad(); acad a3=new acad(); a.sum(number1,number2);//calling the static method sum which accepts 2 parameters(number1,number2) a1.sum(number1,number2,number3); a2.sum(name,number1,number2,number3); a3.sum(number1,number2,number3,name);

}

// Overloading – Different Number of parameters

public void sum(int a,int b)
{
    int sum=a+b;

    System.out.println("Sum of 2 main subject:"+sum);
}
public void sum(int a,int b,int c)
{
    int sum=a+b+c;
    System.out.println("Sum of 3 subjects(including optional subject):"+sum);

}
public void sum(String name,int a,int b,int c)//Overloading – Data type of parameters.
{
    int sum=a+b+c;
    System.out.println("Marks of "+name+" and his marks");
    System.out.println("Sum of 3 subjects(including optional subject):"+sum);

}
public void sum(int a,int b,int c,String name)//Overloading –Sequence of Data type of parameters.
{
    int sum=a+b+c;
    System.out.println("Marks of "+name+" and his marks");
    System.out.println("Sum of 3 subjects(including optional subject):"+sum);

}
}
