---
layout: post
title:  "Bilangan Prima"
categories: java
---

Bilangan Prima adalah bilangan yang habis dibagi dengan 1 dan bilangan itu sendiri. Bilangan prima dimulai dari 2, 3, 5, 7, 11, 13, dst. Inti dasar penentuan bilangan prima adalah dengan melakukan perhitungan modulus terhadap bilangan tersebut dengan perulangan antara 2 sampai bilangan tersebut. <!--more--> Namun sebelumnya ada variabel counter misal count dengan nilai awal 1 kemudian ketika bilangan dimodulus ke-bilangan tersebut counter tersebut ditambah 1.

Lakukan pengecekan apakah count = 2, bila iya maka bilangan tersebut adalah bilangan prima, bila tidak sama dengan 2 maka bilangan tersebut bukan bilangan prima. Berikut ini source code untuk operasi bilangan prima yaitu :

1. Menentukan bilangan prima atau bukan
2. Mencari bilangan prima diantara 2 bilangan
3. Mencari bilangan prima sebanyak n

{% highlight java %}
package prime;

import java.util.Scanner;

public class Prime {

    private boolean prime(int data) {
        if (data <= 1) {
            return false;
        }
        for (int i = 2; i <= Math.sqrt(data); i++) {
            if (data % i == 0) {
                return false;
            }
        }
        return true;
    }

    private void isPrime(int data) {
        if (prime(data)) {
            System.out.println(data + " = prime");
        } else {
            System.out.println(data + " = not prime");
        }
    }

    private void primeBetween(int start, int end) {
        int count = 0;
        System.out.println("Prime between " + start + " - " + end + " = ");
        for (int i = start; i <= end; i++) {
            if (prime(i)) {
                System.out.print(i + " ");
                count++;
            }
        }
        System.out.println("\nThere are " + count + " prime");
    }

    private void nPrime(int n) {
        int num = 0;
        System.out.println("First " + n + " prime number =");
        for (int count = 1; count <= n; num++) {
            if (prime(num)) {
                System.out.print(num + " ");
                count++;
            }
        }
        System.out.println();
    }

    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        Prime p = new Prime();
        do {
            System.out.println("1. Prime or not prime");
            System.out.println("2. Prime between 2 number");
            System.out.println("3. First n prime");
            System.out.print("Choose menu = ");
            switch (in.nextInt()) {
                case 1:
                    System.out.print("Insert number = ");
                    p.isPrime(in.nextInt());
                    break;
                case 2:
                    System.out.println("Insert start and end number!");
                    p.primeBetween(in.nextInt(), in.nextInt());
                    break;
                case 3:
                    System.out.print("How many first prime number? ");
                    p.nPrime(in.nextInt());
                    break;
            }
            System.out.println("**********************");
            System.out.print("Do again?y/n ");
        } while (in.next().equalsIgnoreCase("y"));
    }
}
{% endhighlight %}
