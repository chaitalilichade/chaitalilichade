package ObjectAndMethods;

import java.time.Clock;
import java.util.Scanner;
import java.time.LocalTime;
public class Kartin1 {
	
   
			public void Above65() {
			try {
				System.out.println("Press 1 if You Have Any diease like diabetes,blood pressure otherwise Press 2");
				Scanner sc = new Scanner(System.in);
				int diease = sc.nextInt();
				if (diease == 1) {
					System.out.println("Press 1 If you join your Medicine course otherwise Press 2");
					Scanner sc2 = new Scanner(System.in);
					int course = sc.nextInt();
					if (course == 1) {
						System.out.println("You need to Wake up at 07:00am and go for a walk");
						Thread.sleep(1000);
						System.out.println("After a Walk you need take Light Break Fast ");
						Thread.sleep(1000);
						System.out.println("Than Start your  medicine course as per schedule (in a days) ");
						Thread.sleep(1000);
						System.out.println("Than medicine should be continue (yes/No) as per schedule is completed for a months");
						
						
					} else {
						System.out.println(" You need to get a checkup done,and keep the prescribed scheduled continued(better health)");
						}
					}
						
								
					 else {
				}
			} catch (Exception e) {
				System.out.println("Exception thrown :" + e);
			} finally {
				System.out.println("Thank You");
			}

		}

		public void Below65() {
			System.out.println(" You need to get a checkup done, and keep the prescribed scheduled continued(better health)");

		}

		public static void main(String[] args) {
			Kartin k = new Kartin();
			System.out.println("Welcome to the Kartin Hospital");
			System.out.println("Please Enter your name");
			Scanner sc = new Scanner(System.in);
			String name = sc.next();
			System.out.println("Thank You " + name);
			System.out.println("Please Enter Your Age");
			Scanner sc1 = new Scanner(System.in);
			int age = sc1.nextInt();
			if (age >= 65) {
				k.Above65();
			} else {
				k.Below65();
			}

		}

	

}



