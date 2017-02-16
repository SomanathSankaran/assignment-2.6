# assignment-2.6

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
