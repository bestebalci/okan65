package okan6;
import java.util.Scanner;
public class okan65 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int num1, num2, count;
		int girilensonuc, dogrucevap, dogrucevapsayaci;
		
		
		Scanner input = new Scanner(System.in);
		
		count = 0;
		dogrucevapsayaci = 0;
		while (count <5){
			num1 = (int) (Math.random() *10 );
			num2 = (int) (Math.random() *10 );
			
			System.out.println("sayilar" + num1 + " " + num2);
			
			System.out.println("cıkarma sonucu nedir yazin");
			girilensonuc = input.nextInt();
			dogrucevap = num1 - num2;
			if (girilensonuc == dogrucevap ){
				dogrucevapsayaci++;
			}
			count++;
		}
		System.out.println("dogru cevap sayisi" + dogrucevapsayaci);

	}

}
