---
layout: post
title:  "Segitiga Pascal"
categories: java
---
Segitiga Pascal adalah suatu aturan geometri pada koefisien binomial dalam sebuah segitiga. Ia dinamakan seperti Blaise Pascal dalam kebanyakan dunia barat, meskipun ahli matematika lain telah mengkajinya berabad-abad sebelum dia yaitu orang-orang di India, Persia, Cina, dan Italia. Barisan segitiga Pascal umumnya dihitung dimulai dengan baris kosong, dan nomor-nomor dalam barisan ganjil biasanya diatur agar terkait dengan nomor-nomor dalam baris genap. Konstruksi sederhana pada segitiga dilakukan dengan cara berikut. Di barisan teratas, hanya tulis nomor 1. Kemudian, untuk membangun unsur-unsur barisan berikutnya. Tambahkan nomor di atas dan di kiri dengan nomor secara langsung, kemudian bagian kosongnya merupakan hasil penjumlahan 2 bilangan ini diatasnya. Berikut ini contoh source codenya:

{% highlight java %}
package pascal;

public class Pascal {

    public void triangle(int maxRows) {
        int r, num;
        for (int i = 0; i  0; j--) {
                System.out.printf("%3s", " ");
            }
            for (int col = 0; col  0) {
                    num = num * (r - col) / col;
                }
                System.out.printf("%3d%3s", num, " ");
            }
            System.out.println();
        }
    }

    public static void main(String[] args) {
        Pascal p = new Pascal();
        p.triangle(12);
    }
}
{% endhighlight %}

*Catatan:* Jika kalian mengisikan lebih dari 12 baris segitiga Pascal maka output segitiganya akan sedikit berantakan, kalian bisa mengedit pada fungsi printf untuk memperbaikinya.
