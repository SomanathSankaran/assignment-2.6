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
