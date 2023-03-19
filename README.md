# actividad2_punto7_poo
package cantidaddinero;
import java.util.Scanner;
public class Cantidaddinero {

    public static void main(String[] args) {
       double  horas,valorhora,het,hee8,salario;
       Scanner ingresotecl = new Scanner (System.in);
       
        System.out.println("Ingrese el nombre:  ");
        String nombres = ingresotecl.next();
        
        System.out.println("Ingrese las horas trabajadas en la semana:  ");
        horas = ingresotecl.nextDouble();
        
        System.out.println("Ingrese el valor de la hora de trabajo:  ");
        valorhora = ingresotecl.nextDouble();
        
        if (horas>40){
            het=horas-40;
            if(het>8){
                hee8=het-8;
                salario=(40*valorhora)+(16*valorhora)+(hee8*3*valorhora);
            }
            else{
                salario=(40*valorhora)+(het*2*valorhora);
            }
        }        
        else{
            salario=valorhora*horas;
        }
        System.out.println("el trabajador: "+ nombres +" devengo: $"+ salario);
        
        
        
    }
    
}
