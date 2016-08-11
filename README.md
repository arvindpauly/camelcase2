# camelcase2
import java .util.Scanner;
public class Guvi1 {
public static void main(String[] args) {
	Scanner a=new Scanner(System.in);
	System.out.println("enter the  first string");
	String s1=a.nextLine();
	String s= " ";
	String [] array=s1.split(" ");
     int index=0;
	for(int i=0;i<array.length;i++)	
	{ 
		if(array[i].charAt(0)>96 && array[i].charAt(0)<123)
	   {
		array[i]= new StringBuffer(array[i]).replace(index,index+1,String.valueOf((char)(array[i].charAt(0)-32))).toString();
	   }
		s= s+" "+array[i];
	}	
	System.out.println(s.trim());
	}
}
