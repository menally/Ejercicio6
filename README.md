import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Escribe una frase o un enunciado completo:");

        String entrada = sc.nextLine().trim();
        //nextLine(): Lee toda la frase//
        //trim(): Elimina espacios al inicio y al final//

        if (entrada.isEmpty()) {
            //isEmpty():Comprueba si está vacío//

            System.out.println("Resultado numérico: 0");
        } else {

            String[] bloques = entrada.split("\\s+");
            //split("\\s+"):Divide la frase utilizando los espacios//
            //bloques.length: Cuenta las partes obtenidas//

            System.out.println("Resultado numérico: " + bloques.length);
        }

        sc.close();
    }
}

//El programa recibe una frase y cuenta cuántas palabras contiene//