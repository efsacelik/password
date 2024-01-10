# password
Takes input from user as password and evaluates whether it is true or not. 
package patikaAcademy;

import java.util.Scanner;

public class password {

	public static void main(String[] args) {

		Scanner scanner = new Scanner(System.in);
		String password, userName, selection, newPassword;
		
		System.out.println("Please enter your username");
		userName = scanner.nextLine();
		
		System.out.println("Please enter your password");
		password = scanner.nextLine();
		
		if (password.equals("efsa123")&& userName.equals("efsa") ) {
		System.out.println("You looged in!");
	}   else {
			System.out.println("Incorrect login. Forgot your password?");
			selection = scanner.nextLine();
			  if(selection.equals("no")) {
				  System.out.println("Try again");
		  }   else if (selection.equals("yes")) {
				      System.out.println("Enter your new password");
				          newPassword = scanner.nextLine();
				            if(newPassword.equals("efsa123") ) {
				           System.out.println("You cannot enter same password."); 
				             }else {
				           System.out.println("You recreated your password. ");
				           }
		  }  
				    else    {
		    System.out.println("Invalid choice, please try again.");	 
		    	 
		     }
		     
		     
		     }
		  
		  }
			  
			  
			  
		
	
	
	
	}
	


