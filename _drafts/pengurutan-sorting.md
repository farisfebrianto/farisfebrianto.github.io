Sorting adalah proses menyusun elemen – elemen dengan tata urut tertentu dan proses tersebut terimplementasi dalam bermacam aplikasi. Kita ambil contoh pada aplikasi absensi yang diurutkan berdasarkan NIM mahasiswa UB. Aplikasi tersebut mampu menampilkan daftar mahasiswa yang aktif dengan daftar berurutan NIM secara ascending demi kenyamanan dalam penelusuran data.
Dalam artian sorting digunakan untuk mengurutkan sesuatu (seperti kamus, buku telepon). Sorting yang kita terapkan menggunakan tipe data array agar pemahaman serta pengimplementasiannya lebih  mudah. Pada umumnya terdapat dua jenis pengurutan :
Ascending (Naik)
Descending (Turun)
Contoh :
Data Acak : 22, 10, 15, 3, 8, 2
Terurut Ascending : 2, 3, 8, 10, 15, 22
Terurut Descending : 22, 15, 10, 8, 3, 2
Untuk melakukan proses pengurutan tersebut dapat digunakan berbagai macam cara/metode. Beberapa macam-macam sorting yaitu :
1.  Bubble Sort
Bubble sort ada metode sorting termudah dan sederhana dalam pengimplementasinya dengan keefektifan O(n2). Diberikan nama “bubble” karena konsep dari algoritmanya diibaratkan seperti gelembung air untuk elemen struktur data yang seharusnya pada posisi awal.
Bubble sort mengurut data dengan cara membandingkan elemen sekarang dengan elemen berikutnya. Dimana cara kerjanya adalah dengan berulang-ulang melakukan proses looping terhadap elemen-elemen struktur data yang belum diurutkan. Nilai dari masing-masing elemen akan dibandingkan selama proses looping tersebut. Jika selama proses looping tersebut ditemukan ada urutannya tidak sesuai dengan permintaan, maka akan dilakukan proses penukaran.
2. Insertion Sort
Algoritma insertion sort pada dasarnya memilah data yang akan diurutkan menjadi dua bagian dengan keefektifan O(n2), yang belum diurutkan (meja pertama), dan yang telah diurutkan (meja kedua). Elemen pertama yang diambil dari bagian array yang belum diurutkan dan kemudian diletakkan pada posisinya sesuai dengan bagian lain dari array yang telah diurutkan. langkah ini dilakukan secara berulang hingga tidak ada lagi elemen yang tersisa pada bagian array yang belum diurutkan. Pola dari Insertion Sort menggurutkan n atau 2 elemen dari terdepan dan seterusnya.
3. Selection sort
Merupakan Kombinasi antara sorting dan searching dengan keefektifan O(n2). Metode selection sort merupakan perbaikan dari metode bubble sort dengan mengurangi jumlah perbandingan. Selection sort merupakan metode pengurutan dengan mencari nilai data terkecil dimulai dari data diposisi 0 hingga diposisi N-1. Jika terdapat N data dan data terkoleksi dari urutan 0 sampai dengan N-1. Selama proses, perbandingan dan pengubahan, hanya dilakukan pada indeks permbandingnya saja, pertukaran data secara fisik terjadi pada akhir proses.sesuai dengan itu maka algoritma pengurutan data secara Selection adalah sebagai berikut :

    Cari data terkecil dalam interval j = 0 sampai dengan j = N-1
    Jika pada posisi pos ditemukan data yang terkecil, maka tukarkan data diposisi pos dengan data di posisi i jika k
    Ulangi langkah pertama

4. Marge Sort
Pengurutan algoritma Merge Sort membuat pengurutan dengan membagi 2 dan menggabungkannya dengan keefektifan O(n log n). Metoda ini cukup efisien untuk diterapkan. Sama dengan Quick Sort, algoritma Merge Sort adalah dasar pembagian dan penyelesaiannya. Pertama urutan atau elemen data awal diurutkan dengan membaginya menjadi 2 bagian (Devide) setengahnya diurutkan dengan bebas (Conquer), kemudian 2 bagian itu digabungkan dengan cara diurut sesuai dengan urutan.

    Devide, yakni memilih masalah menjadi sub-masalah.
    Conquer, yakni menyelesaikan sub-masalah tersebut secara rekursi.
    Penggabungan, menggabungkan solusi dari sub-masalah

5. Quick Sort
Pengerian Quick Sort adalah algoritma yang dijalankan sebagai akibat dari terlalu banyaknya daftar yang diurutkan dengan keefektifan O(n log n), Algoritma dibuat tahun 1960 oleh Tony Hoare dan dianasila lebih lanjut oleh Robert Sedgewick dalam thesisnya. Quicksort mendapatkan adaptasi yang luas contohnya Unix menggunakannya sebagai fungsi pengurutan library secara default. Quick sort secara teori adalah mempartisi data dengan menemukan pivot (data ditengah) kemudian menggabungkannya (hampir sama seperti mergesort)

Berikut ini adalah contoh mergesort ascending dan quicksort descending

package sort;

public class Mergesort {

    public void mergeSort(int[] list) {
        if (list.length > 1) {
            int[] firstHalf = new int[list.length / 2];
            System.arraycopy(list, 0, firstHalf, 0, list.length / 2);
            mergeSort(firstHalf);
            int secondHalfLength = list.length - list.length / 2;
            int[] secondHalf = new int[secondHalfLength];
            System.arraycopy(list, list.length / 2, secondHalf, 0, secondHalfLength);
            mergeSort(secondHalf);
            merge(firstHalf, secondHalf, list);
        }
        for (int i = 0; i < list.length; i++) {

            System.out.printf("%1s%1d%1s", "[", i, "]");
            System.out.printf("%2d%1s", list[i], " ");
        }
        System.out.println();
    }

    public void merge(int[] list1, int[] list2, int[] temp) {
        int current1 = 0;
        int current2 = 0;
        int current3 = 0;

        while (current1 < list1.length && current2 < list2.length) {

            if (list1[current1] < list2[current2]) {
                temp[current3++] = list1[current1++];
            } else {
                temp[current3++] = list2[current2++];
            }

            while (current1 < list1.length) {
                temp[current3++] = list1[current1++];
            }

            while (current2 < list2.length) {
                temp[current3++] = list2[current2++];
            }
        }
    }
}

package sort;

public class Quicksort {

    public void quickSort(int[] list) {
        quickSort(list, 0, list.length - 1);
    }

    private void quickSort(int[] list, int first, int last) {
        if (first < last) {
            int pivotIndex = partition(list, first, last);
            quickSort(list, first, pivotIndex);
            quickSort(list, pivotIndex + 1, last);
        }
    }

    private int partition(int[] list, int first, int last) {
        int pivot = list[first];
        int low = first;
        int high = last;

        for (int i = 0; i < list.length; i++) {
            System.out.printf("%1s%1d%1s", "[", i, "]");
            System.out.printf("%2d%1s", list[i], " ");
        }
        System.out.println();

        while (low  pivot) {
                low++;
            }

            while (list[high] < pivot) {
                high--;
            }

            if (low < high) {
                int temp = list[low];
                list[low] = list[high];
                list[high] = temp;
            }
        }
        return high;
    }
}

package sort;

public class SortTest {

    public static void print(int[] list) {
        for (int i = 0; i < list.length; i++) {
            System.out.printf("%1s%1d%1s", "[", i, "]");
            System.out.printf("%2d%1s", list[i], " ");
        }
        System.out.println();
    }

    public static void main(String[] args) {
        Mergesort m = new Mergesort();
        Quicksort q = new Quicksort();

        int[] list1 = {9, 3, 7, 46, 76, 83, 17};
        int[] list2 = {9, 3, 7, 46, 76, 83, 17};

        System.out.println("Data Sebelum Diurutkan");
        print(list1);
        System.out.println("Proses Mergesort Ascending");
        m.mergeSort(list1);
        System.out.println("Proses Quicksort Descending");
        q.quickSort(list2);
    }
}
