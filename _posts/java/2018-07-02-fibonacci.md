---
layout: post
title:  "Fibonacci"
categories: Java
image: fibonacci.png
permalink: /fibonacci/
comments: true
---

Deret Fibonacci adalah deret yang dimulai dari angka 0 dan 1, kemudian deret selanjutnya merupakan penjulahan 2 deret sebelumnya. Sejarah deret fibonacci berawal dari Gopala dan Hemachandra, matematikawan dari India pada tahun 1150. Namun di eropa deret ini diperkenalkan oleh Leonardo da Pisa  sekitas pada tahun 1200 dan perlu diketahui deret ini sangat unik. <!--more--> Setiap perbandingan dari deret ke n dan deret n-1 selalu mendekati nilai 1.6, misal deret ke-7 dan deret ke 6, 8 dibanding dengan 5 maka hasilnya adalah 1.6. Untuk algoritma dan source code deret fobonacci ada dua cara yaitu:

1. Rekursif : melakukan pemanggilan diri sendiri untuk mencari deret Fibonacci
2. Iteratif : melakukan perulangan untuk mencari deret Fibonacci

{% highlight java %}
package fibonacci;

public class Fibonacci {

    private int fiboRekursif(int n) {
        if (n < 2) {
            return n;
        } else {
            return fiboRekursif(n - 1) + fiboRekursif(n - 2);
        }
    }

    private void fiboRekursif() {
        for (int i = 0; i <= 10; i++) {
            System.out.print(fiboRekursif(i) + " ");
        }
        System.out.println();
    }

    private void fiboIteratif(int n) {
        int prev1 = 0, prev2 = 1;
        for (int i = 0; i <= n; i++) {
            int hasil = prev1;
            prev1 = prev2;
            prev2 = hasil + prev2;
            System.out.print(hasil + " ");
        }
    }

    public static void main(String[] args) {
        Fibonacci fibo = new Fibonacci();
        fibo.fiboRekursif();
        fibo.fiboIteratif(10);
    }
}
{% endhighlight %}
