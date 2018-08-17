---
layout: post
title:  "Mencari Bilangan Ganjil dan Genap"
categories: java
---

Pada dasarnya bilangan ganjil adalah bilangan yang jika dibagi dua maka akan menghasilkan sisa satu untuk bilangan bulat positif dan sisa -1 untuk bilangan bulat negatif. Untuk menentukan bilangan genap yaitu dengan membagi bilangan tersebut dengan dua dengan sisa nol dan selain bilangan 0 yang dibagi (bilangan netral).

<!--more-->

Dalam mengeimplementasikannya kedalam bahasa java maka digunakanlah operator % (modulus) untuk mencari sisa dari pembagian suatu bilangan, berikut ini source codenya:

{% highlight java %}
package ganjilgenap;

import java.util.Scanner;

public class GanjilGenap {

    public boolean ganjil(int data) {
        return data % 2 == 1 || data % 2 == -1;
    }

    public boolean genap(int data) {
        return data % 2 == 0 && data != 0;
    }

    public void isGanjil(int data) {
        if (ganjil(data)) {
            System.out.println(data + " = ganjil");
        } else if (genap(data)) {
            System.out.println(data + " = genap");
        } else {
            System.out.println(data + " = netral");
        }
    }

    public void antara(int start, int end) {
        int nGanjil = 0, nGenap = 0;
        System.out.println("Ganjil = ");
        for (int i = start; i <= end; i++) {
            if (ganjil(i)) {
                System.out.print(i + " ");
                nGanjil++;
            }
        }
        System.out.println("\nJumlah = " + nGanjil);
        System.out.println("Genap = ");
        for (int i = start; i <= end; i++) {
            if (genap(i)) {
                System.out.print(i + " ");
                nGenap++;
            }
        }
        System.out.println("\nJumlah = " + nGenap);
    }

    public static void main(String[] args) {
        GanjilGenap GG = new GanjilGenap();
        Scanner in = new Scanner(System.in);
        do {
            System.out.println("1. Menentukan bilangan ganjil atau genap");
            System.out.println("2. Mencari ganjil genap antara 2 bilangan");
            System.out.print("Pilih = ");
            switch (in.nextInt()) {
                case 1:
                    System.out.print("Masukkan bilangan = ");
                    GG.isGanjil(in.nextInt());
                    break;
                case 2:
                    System.out.println("Masukkan bilangan pertama dan kedua");
                    GG.antara(in.nextInt(), in.nextInt());
                    break;
                default:
                    System.out.println("Pilihan salah");
                    break;
            }
            System.out.print("Lanjutkan? y/n ");
        } while (in.next().equals("y"));
    }
}
{% endhighlight %}
