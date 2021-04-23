public class Main {

    public static java.util.Scanner input = new java.util.Scanner(System.in);

    public static Dekripsi method = new Dekripsi();

    public static char[] array;

    public static String str = "";

    public static char[] huruf = {
            'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm',
            'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z'
    };

    public static void main(String[] args) {

        System.out.print("Silakan masukkan kata : ");
        array =(input.next().toCharArray());

        String[] opsi = {
                "1. Enkripsi", "2. Dekripsi"
        };

        for(int i = 0; i < 2; i++){
            System.out.println(opsi[i]);
        }
        System.out.print("Silakan pilih opsi di atas(nomor 1-2) : ");
        int pilih = input.nextInt();

        if(pilih == 1){
            enkripsi();
        }else if(pilih == 2){
            method.dekripsi();
        }

    }

    static void enkripsi(){
        for (char value : array){
            for(int i=0; i <= 25; i++){
                if(value == huruf[i]){
                    i = i + 29;
                    if(i >= 26){
                        i = i - 27;
                    }
                    value = huruf[i];
                    str = str + value;
                }
            }
        }
        System.out.println("Hasil Enkripsi adalah : " + str);
    }
}

class Dekripsi extends Main{

    public void dekripsi(){
        for (char value : array){
            for(int i=0; i <= 25; i++){
                if(value == huruf[i]){
                    i = i - 29;
                    if(i < 0){
                        i = i + 27;
                    }
                    value = huruf[i];
                    str = str + value;
                }
            }
        }
        System.out.println("Hasil Dekripsi adalah : " + str);
    }
}
