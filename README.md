package belajar_class_method;

import java.util.Scanner;

/**
 *
 * @author EC
 */
public class CafeCeria {
    public static void main(String[] args) {
        // Membuat objek Scanner untuk mengambil input dari pengguna
        Scanner sc = new Scanner(System.in);

        // Membuat variabel untuk menyimpan nama pembeli dan pilihan minuman
        String nama;
        int pilihan;
        String minuman;

        // Menampilkan informasi cafe
        System.out.println("CAFE CERIA ANEKA MINUMAN");
        System.out.println("SPECIAL MENU:");

        // Menampilkan daftar minuman
        System.out.println("1. Soft drinks");
        System.out.println("2. Mix juice");
        System.out.println("3. Nescafe");
        System.out.println("4. Soda milk");
        System.out.println("5. Tea");

        // Meminta input nama pembeli
        System.out.print("Masukkan nama pembeli: ");
        nama = sc.nextLine();

        // Meminta input pilihan minuman
        System.out.print("Silahkan masukkan pilihan anda: ");
        pilihan = sc.nextInt();

        // Menggunakan switch-case untuk menentukan minuman berdasarkan pilihan
        switch (pilihan) {
            case 1:
                minuman = "Soft drinks";
                break;
            case 2:
                minuman = "Mix juice";
                break;
            case 3:
                minuman = "Nescafe";
                break;
            case 4:
                minuman = "Soda milk";
                break;
            case 5:
                minuman = "Tea";
                break;
            default:
                minuman = "Tidak tersedia";
                break;
        }

        // Menampilkan minuman yang dipesan
        System.out.println("Minuman yang anda pesan adalah " + minuman);

        // Menampilkan pesan terima kasih
        System.out.println("Pesanan akan segera kami antar");
        System.out.println("Terima Kasih " + nama + " telah berkunjung di Cafe Ceria");
    }
}
