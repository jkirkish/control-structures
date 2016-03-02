# control-structures
/**
 * @author jk
 * Created on 03/01/2016
 */
public class howControlStructuresWork {

	static int balance;
	static int bankStandard;
	
	howControlStructuresWork(int bal,int bank){
		
		this.balance = bal;
		this.bankStandard = bank;
	}
	public int getBalance() {
		return balance;
	}
    public static void EvalCeditScore(int balance){
    	if (balance >= 10000)
    		System.out.println("CreditScore = 800");
    	else if (balance >= 9000)
    		System.out.println("CreditScore = 700");
    	else if (balance >= 7000)
    		System.out.println("CreditScore = 600");
    	else if (balance >= 6000)
    		System.out.println("CreditScore = 500");
    	else if (balance >= 5000)
    		System.out.println("CreditScore = 400");
    	else if (balance >= 4000)
    		System.out.println("CreditScore = 300");
    	else if (balance >= 3000)
    		System.out.println("CreditScore = 200");
    	else if (balance >= 2000)
    		System.out.println("CreditScore = 100");
    	else
    		System.out.println("NA");
    }
	public void setBalance(int balance) {
		this.balance = balance;
	}
	public static void main(String[]args)
	{
		
	   balance = 2500;
	   bankStandard = 4000;
	   if(balance < bankStandard)	
	   System.out.println("You have insufficient funds. Please add money");
	   System.out.println("Current Balance: " + balance);
	   EvalCeditScore(balance);
	}
	/*statements in a program are executed one after the other in what is known as sequential execution
	*Three control structures the sequence structure, selection structure and repetition structure.
	*The if statements i a single-entry/single exit control statement
	*The if/else double-selection statement 
	*The conditional operator(?:) symbol form a conditional expression-->System.out.println(StudentGrade>= ? "Passed : "Failed");
	*The dangling else is when the compiler always associates an else with the immediately preceding if unless told to do otherwise by the placement of braces({and})
	*
	*/
}
