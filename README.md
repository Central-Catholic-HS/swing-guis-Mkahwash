[![Work in Repl.it](https://classroom.github.com/assets/work-in-replit-14baed9a392b3a25080506f3b7b6d57f295ec2978f6f33ec97e36a161684cbe9.svg)](https://classroom.github.com/online_ide?assignment_repo_id=3320319&assignment_repo_type=AssignmentRepo)
package com.central.practice;
import javax.swing.JOptionPane;


public class DialogBoxPractice {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		String temp1, temp2, temp3;
		
		temp1 = JOptionPane.showInputDialog("Enter your temperature from Monday: ");
		double actualTemp1 = Double.parseDouble(temp1);
		
		temp2 = JOptionPane.showInputDialog("Enter your temperature from Tuesday: ");
		double actualTemp2 = Double.parseDouble(temp2);
		
		temp3 = JOptionPane.showInputDialog("Enter your temperature from Wednesday: ");
		double actualTemp3 = Double.parseDouble(temp3);
		
		double averageTemp = (actualTemp1 + actualTemp2 + actualTemp3)/3;
		
		
		if(averageTemp > 98.6){
		
			JOptionPane.showMessageDialog(null, "DONT COME TO SCHOOL! Your average tempature (" + averageTemp + ") is too high." );

		}
		
		else {
			JOptionPane.showMessageDialog(null, "You are okay to come to school today. Your average temperature is " + averageTemp); 
		}
		
		System.exit(0);
		
	}

}
