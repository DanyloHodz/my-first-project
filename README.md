package org.exemple;
import java.math.BigDecimal;
import java.util.Scanner;
class Калькулятор{
    public static void main(String[]args){
        Scanner scan = new Scanner(System.in);
        System.out.println("Напишіть першу цифру>");
        Double user1 = scan.nextDouble();
        System.out.println("Напишіть другу цифру>");
        Double user2 = scan.nextDouble();
        System.out.println("Напишіть  дію>");
        String  user3 = scan.next();
        if(user3.equals("+")) {
            System.out.println("Сума> " + (user1 + user2));
        }else if(user3.equals("-")){
            System.out.println("Різниця> " +( user1 - user2 ));
        }else if(user3.equals("*")){
            System.out.println("Добуток> " +( user1 * user2 ));
        }else if(user3.equals("/")){
            if (user2 != 0) {
                System.out.println("Частка> " +( user1 / user2 ));
            }else {
                System.out.println("Помилка. Ділення на 0 неможливе");
            }
        }else{
            System.out.println("Невірна операція");
       }
    }
}
