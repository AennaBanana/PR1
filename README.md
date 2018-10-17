import java.util.*;

public class eurodollar {

	public static void main(String[] args) {
		// currency translation
		
		Scanner sc = new Scanner(System.in);
		String menupunkt = "ja";
		do {
			System.out.println("Wählen Sie einen Menüpunkt aus \n 1. Euro in Dollar \n 2. Dollar in Euro");
			
			float i = sc.nextFloat();
			// Choose an option from the menu
			
			if (i==1) {
				//The first option
				System.out.println("(1) Bitte geben Sie einen Eurobetrag ein.");
				float euro = sc.nextFloat();
				//calculation
				float dollar = euro * 1.34f;
				System.out.println("Der Dollarbetrag beträgt:" + dollar + "$");
			}
			
			else if (i==2) {
				//The second option
				System.out.println("(2) Bitte geben Sie einen Dollarbetrag ein:");
				float dolla = sc.nextFloat();
				//calculation
				float eur = (float) (dolla * (1/1.34));
				System.out.println("Der Eurobetrag beträgt:" + eur + "€");
				
			}
			System.out.println("Wollen Sie eine weitere Umrechnung durchführen?");
			menupunkt = sc.next();
		}while (menupunkt.equals("ja"));
		

	}

}
