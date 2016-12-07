# Assignment8.4
package com.session8;

import java.io.*;
import java.util.Scanner;

public class VowelsFileCount {
	

	public static void main(String[] args) throws FileNotFoundException {
		// TODO Auto-generated method stub
		String fileContent = "";
		 FileInputStream fin = new FileInputStream("C:\\Users\\Unni\\Desktop\\Emp.txt");
			//int data = fin.read();
	        Scanner input = new Scanner(fin);
	        
	        while (input.hasNext()) {
	        fileContent += input.next() + " ";
	        }
	        
	        input.close();

	        char[] charArr = fileContent.toCharArray();
	        int counter = 0;
	        for(char c : charArr)
	         {
	           if(c == 'a' || c == 'e' || c == 'i' || c == 'o' || c == 'u' || c == 'y')
	        
	        	                   counter++;
	       
       	        }
	        
	                System.out.println("Number of Vowels: " + counter);
}}
