# SnaniOmar_Calculette_TP0

/*
Omar SNANI
Groupe A
exo 1
22/09/2026
*/
package exo1;

import java.util.Scanner;

/**
 *
 * @author snani
 */
public class Exo1 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        String prenom;
        
        System.out.println("Bonjour");
        System.out.println("Au revoir !");
        
        
        Scanner sc;
        sc = new Scanner(System.in);
        System.out.println("Bonjour, quel est votre prenom ?");
        prenom = sc.nextLine();
        if ( "Omar".equals(prenom)) System.out.println("BG");
    }
    
}

/*
Omar SNANI
Groupe A
exo 2
22/09/2026
*/
package exo2;

import java.util.Scanner;

/**
 *
 * @author snani
 */
public class Exo2 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        //Declaration des variables
        int nb; // nombre d'entiers a additionner
        int result; // resultat
        int ind; //indice
        //nb=5;
        result=0;
        
        Scanner sc = new Scanner(System.in);
        System.out.println("\n Entrer le nombre :");
        nb = sc.nextInt(); // On demande à sc de donner le prochain entier

        // Addition des nb premiers entiers
        ind=1;
        while (ind >= nb) {
            result=result+ind;
    }

    // Affichage du resultat
    System.out.println();
    System.out.println("La somme des " + nb + "entiers est: " + result);
    }
    
}


/*
Omar SNANI
Groupe A
Calculatrice
22/09/2026
*/
package calculator;

import java.util.Scanner;

/**
 *
 * @author snani
 */
public class Calculator {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        int operateur;
        int operande1, operande2;
        Scanner sc = new Scanner(System.in);
        
        System.out.println("Please enter the operator:\n1) add\n2) substract\n3) multiply\n4) divide\n5) modulo");
        operateur = sc.nextInt();
        
        System.out.println("Donne une première valeur :");
        operande1 = sc.nextInt();
        System.out.println("Donne une seconde valeur :");
        operande2 = sc.nextInt();
        
        
        switch (operateur) {

            case 1:
                System.out.println("Résultat de la somme : " + (operande1 + operande2));
                break;

            case 2:
                System.out.println("Résultat de la soustraction : " + (operande1 - operande2));
                break;

            case 3:
                System.out.println("Résultat de la multiplication : " + (operande1 * operande2));
                break;
                
            case 4:
                System.out.println("Résultat de la division : " + (float)operande1 / operande2);
                break;
                
            case 5:
                System.out.println("Résultat du modulo : " + (operande1 % operande2));
                break;   

            default:
                System.out.println("Erreur !");
                break;
        }
        
        
        
        
        
    }
    
}
