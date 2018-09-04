/////punto 1//////////
package punto_1;
import java.util.Scanner;

	public class punto_1 {
		
	public static void main(String[] args) {
	Scanner sc = new Scanner (System.in);

	int opcion;
	float n1,n2,resul;
	System.out.println("Suministre el numero 1: ");
	n1 = sc.nextFloat();
	System.out.println("Suministre el numero 2: ");
	n2 = sc.nextFloat();
	System.out.println("Ingrese la operacion a ejecutar: 1. Suma     2. Resta    3. Multiplicacion     4. Division ");
	opcion = sc.nextInt();
	switch(opcion) {
	case 1:
	resul = n1 + n2;
	System.out.println("La suma de los dos numeros es: " +resul);
	break;
	case 2:
		resul = n1 - n2;
		System.out.println("La esta de los dos numeros es: " +resul);
		
		break;
	case 3:
		resul = n1 * n2;
		System.out.println("La multiplicacion de los dos numeros es: " +resul);
		
		break;
	case 4:
		if(n2 == 0 ) {
			System.out.println("No es posible dividir por 0");
		}else {
			resul = n1 / n2;
			System.out.println(String.format("La division de los dos numeros es: %.2f ",resul));
		}
		
		break;
		
		}
	}	
}

/////////////////punto 2 /////////////////// 
package punto_2;
import java.util.Scanner;

class punto_2 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc = new Scanner (System.in);
		int grados, f;
		
		System.out.println("Suministre los grados a convertir");
		grados = sc.nextInt();
		
		f = 32 + (9 * grados / 5);
				
		System.out.println("grados Fahrenheit: "+ f);
		
	}

}
