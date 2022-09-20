package com.gl.main;

import java.util.Scanner;

import com.gl.model.Employee;
import com.gl.service.Credentialservice;

public class CredentialApp {

	public static void main(String[] args) {
		
    Employee employee=new Employee("Diana", "Spencer");
    Credentialservice credentialservice=new Credentialservice();
    String generatedEmail="";
    char[] generatedPwd;
 
   System.out.println("Please enter the department from the following:");
   System.out.println("1. Technical");
   System.out.println("2. Admin");
   System.out.println("3. Human Resource");
   System.out.println("4. Legal");
   
   Scanner scanner=new Scanner(System.in);
   int option=scanner.nextInt();
   
   if(option==1) {
	   generatedEmail=Credentialservice.generateEmailAddress(employee.getFirstName(),employee.getLastName(),"tech");
   
  
   } else if(option==2) {
	    generatedEmail=Credentialservice.generateEmailAddress(employee.getFirstName(),employee.getLastName(),"adm");
   
	   
   }else if(option==3) {
	    generatedEmail=Credentialservice.generateEmailAddress(employee.getFirstName(),employee.getLastName(),"hr");
	   
	    
   }else if(option==4) {
	    generatedEmail=Credentialservice.generateEmailAddress(employee.getFirstName(),employee.getLastName(),"lg");
	
	
   
   }else {
		System.out.println("Enter a valid option");
     	scanner.close();
		System.exit(-1);
   }
   generatedPwd=Credentialservice.generatePassword();
   Credentialservice.showCredentials(employee.getFirstName(),generatedEmail,generatedPwd);
   
    scanner.close();
    
	}
}
	
    
    
