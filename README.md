Sebastian Lozano- Andres Gaviria

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
////////////////////punto 3 /////////////////////

package punto_3;
import java.util.Scanner;
public class punto_3 {

	public static void main(String[] args) {
	Scanner sc = new Scanner (System.in);
	
	String nombre;
	int ht, sh, he, tipo, sueldo;
	double salario_minimo = 781242;
	double salario_final;
	
	System.out.println("Ingrese nombre: ");
	nombre = sc.nextLine();
	System.out.println("Ingrese horas trabajadas: ");
	ht = sc.nextInt();
	if(ht>48) {
	System.out.println("No se puede trabajar mas de 48 horas ");
	}else {
	
	System.out.println("Ingrese sueldo por hora: ");
	sh = sc.nextInt();
	System.out.println("Ingrese las horas extras laboradas: ");
	he = sc.nextInt();
	System.out.println("Ingrese el tipo de las horas extras laboradas:  1. Diurna 2. Nocturna 3. Dominical 4. Festivos 0. Ninguna");
	tipo = sc.nextInt();

		switch(tipo) {
			case 1:
			sueldo = he * 4069;
			salario_final = salario_minimo + sueldo;
			System.out.println("Nombre: "+nombre);
			System.out.println("Horas trabajadas: "+ht);
			System.out.println("Sueldo por hora: "+sh);
			System.out.println("Horas extras laboradas: "+he);
			System.out.println("Tipo de horas extras laboradas: "+tipo);
			System.out.println("Sueldo: "+salario_final);
		break;
			case 2:
			sueldo = he * 5697;
			salario_final = salario_minimo + sueldo;
			System.out.println("Nombre: "+nombre);
			System.out.println("Horas trabajadas: "+ht);
			System.out.println("Sueldo por hora: "+sh);
			System.out.println("Horas extras laboradas: "+he);
			System.out.println("Tipo de horas extras laboradas: "+tipo);
			System.out.println("Sueldo: "+salario_final);
		break;
			case 3:
			sueldo = he * 6510;
			salario_final = salario_minimo + sueldo;
			System.out.println("Nombre: "+nombre);
			System.out.println("Horas trabajadas: "+ht);
			System.out.println("Sueldo por hora: "+sh);
			System.out.println("Horas extras laboradas: "+he);
			System.out.println("Tipo de horas extras laboradas: "+tipo);
			System.out.println("Sueldo: "+salario_final);
			break;
			case 4:
			sueldo = he * 8138;
			salario_final = salario_minimo + sueldo;
			System.out.println("Nombre: "+nombre);
			System.out.println("Horas trabajadas: "+ht);
			System.out.println("Sueldo por hora: "+sh);
			
		}
		}
	}
}
