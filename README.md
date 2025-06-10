import java.util.Scanner;
public class Main{
    public static void main(String[] args){
Scanner scanner = new Scanner(System.in);


        System.out.println("-----------------------------------------------------");
        System.out.println("Bankamiza hosgeldiniz. Faiz oranimiz %6'dir.");
        System.out.println("-----------------------------------------------------");
        
        int vade,para;
        System.out.println("Bankamiza yatirmak istediginiz tutari giriniz:  ");
        para=scanner.nextInt();
        System.out.println("Kac yillik vade yapmak istiyorsunuz ?");
        vade=scanner.nextInt();
        
        
        double toplampara=para;
        double faiz_Orani=0.06;
        
        for(int i =1; i<=vade; i++){
            
            toplampara=(toplampara*faiz_Orani)+toplampara;
            
            System.out.println(i+". yilin sonunda toplam para: "+(int)toplampara);
            
            
        }
        
        
        








    }
    
    
}
