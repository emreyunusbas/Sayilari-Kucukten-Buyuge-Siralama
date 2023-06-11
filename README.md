# Sayıları Küçükten Büyüğe sıralama

Bu repo, Patika.dev üzerinden aldığımız Kodluyoruz Java 101 Eğitimi kapsamında geliştirdiğimiz "Sayıları Küçükten Büyüğe sıralama" programının kodlarını içermektedir.

## Lisans

Bu projenin lisansı [MIT Lisansı](https://opensource.org/licenses/MIT) altında sunulmaktadır.

---

## Kullanılan Dil

Bu program, Java programlama dili kullanılarak geliştirilmiştir.

---

## Kodluyoruz Java 101 Eğitimi

Bu repo, Patika.dev üzerinden aldığımız Java 101 Eğitimi sürecindeki projeleri ve ödevleri içermektedir.

---

### Proje Açıklaması

Bu program, kullanıcının girdiği üç sayıyı küçükten büyüğe doğru sıralar.

---

### Dosyalar

Bu repo aşağıdaki dosyaları içermektedir:

- `README.md`: Proje hakkında genel bilgiler ve açıklamalar içeren dosya.
- `Main.java`: Programın kaynak kodunu içeren Java dosyası.

---

### Patika.dev Profilim

Proje sahibi: [Yunus Emre BAŞ](https://app.patika.dev/shqiptarbas)

Daha fazla bilgi için ilgili Patika.dev profilimi ziyaret edebilirsiniz.

---

Geliştirdiğimiz bu "Sayıları Küçükten Büyüğe sıralama" programının detaylı açıklamalarını ve kaynak kodunu incelemek için ilgili dosyalara göz atabilirsiniz.

---

### Nasıl Kullanılır

1. Program çalıştırıldığında, kullanıcıdan üç sayı istenir.
2. İstenilen her sayıyı girdikten sonra, Enter tuşuna basarak bir sonraki sayıya geçilir.
3. Program, girilen üç sayıyı karşılaştırarak küçükten büyüğe doğru sıralar ve sonucu ekrana yazdırır.

---

Örnek kullanım:

```java
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        int a, b, c;
        Scanner input = new Scanner(System.in);

        System.out.println("1. Sayı: ");
        a = input.nextInt();

        System.out.println("2. Sayı: ");
        b = input.nextInt();

        System.out.println("3. Sayı: ");
        c = input.nextInt();

        if ((a < b) && (a < c)) {
            if (b < c) {
                System.out.println("a < b < c");
            } else {
                System.out.println("a < c < b");
            }
        } else if ((b < a) && (b < c)) {
            if (a < c) {
                System.out.println("b < a < c");
            } else {
                System.out.println("b < c < a");
            }
        } else if ((c < b) && (c < a)) {
            if (a < b) {
                System.out.println("c < a < b");
            } else {
                System.out.println("c < b < a");
            }
        }
    }
}
