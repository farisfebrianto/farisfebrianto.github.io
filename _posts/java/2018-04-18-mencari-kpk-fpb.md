---
layout: post
title:  "Mencari KPK dan FPB"
categories: java
---

KPK adalah singkatan dari Kelipatan Persekutuan Terkecil dari dua atau lebih bilangan. Manfaat dari KPK antara lain untuk menyamakan dua atau lebih penyebut pecahan sehingga memudahkan menjumlahkan atau mengurangkannya. <!--more--> Contoh KPK dari 2, 3, dan 5 adalah 30.

FPB atau faktor persekutuan terbesar dari dua atau lebih bilangan yang berfungsi untuk mencari bilangan terbesar yang sama untuk membagi dua atau lebih bilangan tersebut. Manfaat dari FPB diantaranya untuk menyederhanakanya pecahan. Contoh FPB dari 20, 36, dan 12 adalah .

Jika diimplementasikan dalam bahasa java sebagai berikut

{% highlight java %}
package kpkfpb;

public class KpkFpb {

    public void kpk(int first, int second) {
        int x = first, y = second;
        while (first != second) {
            if (first  second) {
                second += y;
            }
        }
        System.out.println("KPK = " + first);
//        System.out.println("KPK adalah : " + second);
    }

    public void fpb(int first, int second) {
        int k = 2, m = 2;
        int x = first, y = second;
        while (x != y) {
            if (x > y) {
                while ((first % k) != 0) {
                    k++;
                }
                x = first / k;
                k++;
            } else {
                while ((second % m) != 0) {
                    m++;
                }
                y = second / m;
                m++;
            }
        }
        System.out.println("FPB = " + x);
//        System.out.println("FPB = " + y);
    }

    public static void main(String[] args) {
        KpkFpb kf = new KpkFpb();
        kf.kpk(3, 4);
        kf.fpb(6, 24);
    }
}
{% endhighlight %}
