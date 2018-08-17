---
layout: post
title:  "Konversi Desimal ke Romawi"
categories: java
---

Bilangan Romawi adalah bilangan unik yang memiliki aturan-aturan yang berlaku dan terdiri dari huruf-huruf CAPITAL seperti I, X, C, M, V, L, dan v. Di Indonesia bilangan ini sangat jarang digunakan sekali, tapi untuk hal-hal tertentu saja. <!--more--> Pada dasarnya, bilangan Romawi memiliki bilangan dasar dan maksimal perulangan ganda pada huruf-huruf dalam suatu angka yaitu 3. Misal XXX = 30 bukan XXXX=40.

Pada dasarnya adapun aturan dari bilangan romawi tersebut adalah sebagai berikut :

1. Angka romawi memiliki arti : I = 1 , V = 5, X = 10, L = 50, C = 100, D = 500, M = 100
2. Romawi tidak mengenal 4 buah symbol yang di lakukan secara berurutan. Misal, IIII itu seharusnya IV, XXXX seharusnya LX, dsb
3. Lambang romawi seperti IV, MC, CD, dsb, memiliki ciri khas yaitu Simbol pertama memiliki nilai Lebih Kecil dari pada simbol kedua
4. Jika ditemukankondisi nomor 3 maka pembacaanya adalah lambang kedua dikurangi lambang pertama
5. Jika ditemukan Lambang seperti contoh pada nomor 3 maka yang di bandingkan maju 2 langkah, misal: CMII pertama-tama kita bandingkan karakter pertama dan kedua dahulu yaitu C dan M. C memiliki nilai yang kurang dari M. Selanjutnya, kita membandingkan I dengan I bukan M dengan I
6. Berdasarkan nomor 4 dan 5 diperoleh pembacaan bila CMII maka akan dibaca M – C + I + I
7. Jika kondisi Lambang Kedua Lebih besar dari pada lambang pertama, maka pembacaan tinggal dijumlahkan saja misal: MVII maka M + V + I + I

{% highlight java %}
package dectorome;

public class DectoRomawi {

    public void toRomawi(int des) {
        String romawi[] = {"M", "CM", "D", "CD", "C", "XC", "L", "XL", "X", "IX", "V", "IV", "I"};
        int decimal[] = {1000, 900, 500, 400, 100, 90, 50, 40, 10, 9, 5, 4, 1};

        if (des > 0 && des < 4000) {
            System.out.println("Desimal = " + des);
            String str = "";
            for (int i = 0; i = decimal[i]) {
                    des = des - decimal[i];
                    str = str + romawi[i];
                }
            }
            System.out.println("Romawi = " + str);
        } else {
            System.out.println("Anda angka diluar range [1-3999]");
        }
    }

    public static void main(String[] args) {
        DectoRomawi r = new DectoRomawi();
        r.toRomawi(168);
    }
}
{% endhighlight %}
