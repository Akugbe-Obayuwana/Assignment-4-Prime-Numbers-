# Assignment-4-Prime-Numbers-
In summary An arbitrary number was entered to run the code and the result obtained is in the bracket (Enter any number: 759 759 is a composite factor and the factors are:759)
import java.util.Scanner;
class PrimeCheck
{
   public static void main(String args[])
   {		
	int temp;
	boolean isPrime=true;
	Scanner scan= new Scanner(System.in);
	System.out.println("Enter any number:");
	//capture the input in an integer
	int num=scan.nextInt();
        scan.close();
	for(int i=2;i<=num/2;i++)
	{
           temp=num%i;
	   if(temp==0)
	   {
	      isPrime=false;
	      break;
	   }
	}
	//If isPrime is true then the number is prime else not
	if(isPrime)
	   System.out.println(num + " is a Prime Number and the factors are:" + num);
	else
	   System.out.println(num + " is a composite factor and the factors are:" + num);
   }
}
