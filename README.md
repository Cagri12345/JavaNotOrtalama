# JavaNotOrtalama
Java ile girilen derslerin ortalamasını hesaplayan program
import java.util.Scanner;      //Girilen Notların Ortalamsını ALma Programı
public class Main {
    public static void main(String[] args) {
        // Değikenleri oluştur
        int mat,fizik,kimya,turkce,tarih,muzik;

        // Scanner sınıfımızı tanımlayalım
        Scanner inp = new Scanner(System.in);

        // Kullanıcıdan değerleri al
        System.out.print("Maths mark: ");
        mat = inp.nextInt();

        System.out.print("Physics mark: ");
        fizik = inp.nextInt();

        System.out.print("Chemistry mark: ");
        kimya = inp.nextInt();

        System.out.print("Turkish mark: ");
        turkce = inp.nextInt();

        System.out.print("History mark: ");
        tarih = inp.nextInt();

        System.out.print("Music mark: ");
        muzik = inp.nextInt();

        int total = (mat + fizik + kimya +turkce + tarih+ muzik) ;
        double result = total / 6;
        System.out.println("Ortalamanız: "+ result);

        String durum = result >= 60 ? "Geçti" : "Kaldı";
        System.out.println(durum);
    }
}
