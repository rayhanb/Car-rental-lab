import java.util.Scanner;

public class Main
{

  public static void main (String[]args)
  {

    Scanner s = new Scanner (System.in);
      System.out.println ("Please give the make for the car:");
    String carmake = s.next ();
      System.out.println ("Next, give use the car model:");
    String carmodel = s.next ();
      System.out.println
      ("please put int license plate (three letters and a space with 3 numbers)");
    String lincentplate = s.next ();
    int lincentnum = s.nextInt ();
    int firstL = lincentplate.charAt (0);
    int secondL = lincentplate.charAt (1);
    int thirdL = lincentplate.charAt (2);
    int sum = firstL + secondL + thirdL;
    int idnum = sum + lincentnum;
    int idnum2 = idnum % 26;
    int idletter = idnum2 + 65;
    char letteraftera = (char) idletter;
      System.out.println ("make: " + carmake);
      System.out.println ("model: " + carmodel);
      System.out.println ("car ID: " + lincentplate + " " + lincentnum +
			  " = " + letteraftera + idnum);


  }
}
