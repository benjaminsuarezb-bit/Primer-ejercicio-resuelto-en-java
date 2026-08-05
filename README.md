# Primer-ejercicio-resuelto-en-java
1. En un hospital existen tres áreas: Ginecología, Pediatría, Traumatología. El presupuesto anual del hospital se reparte conforme a la siguiente tabla: Área Porcentaje de Presupuesto Ginecología 40% Pediatría 30% Traumatología 30% Obtener e imprimir la cantidad de dinero que recibirá cada área, para cualquier, monto presupuestal.

import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
		Scanner valorPresupuesto = new Scanner (System.in);
		Double presupuesto;
		Double valorGinecologia;
		Double valorPediatria;
		Double valorTraumatologia;
		
		System.out.println("Ingrese el presupuesto anual: ");
		presupuesto = valorPresupuesto.nextDouble();
		
		valorGinecologia = presupuesto * 40/100;
		valorPediatria = presupuesto * 30/100;
		valorTraumatologia = presupuesto * 30/100;
		
		System.out.println("Monto asignado a cada área: ");
		System.out.println("Ginecología: "+ valorGinecologia);
		System.out.println("Pediatría: "+ valorPediatria);
		System.out.println("Traumatología: "+ valorTraumatologia);
	}
}
