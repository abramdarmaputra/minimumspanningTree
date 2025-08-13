# Kruskal's Algorithm in Python

Program ini mengimplementasikan **Algoritma Kruskal** untuk mencari **Minimum Spanning Tree (MST)** pada sebuah graf terhubung, tidak berarah, dan berbobot.  
Algoritma Kruskal adalah salah satu algoritma *greedy* yang populer untuk menyelesaikan masalah MST.

---

## 📋 Fitur
- Representasi graf menggunakan struktur data berbasis list.
- Implementasi **Union-Find (Disjoint Set Union)** dengan:
  - **Path Compression** untuk optimisasi pencarian.
  - **Union by Rank** untuk optimisasi penggabungan himpunan.
- Sortir edge berdasarkan bobot menggunakan *lambda sorting*.
- Menampilkan semua edge yang membentuk MST beserta total bobotnya.

---

## ⚙️ Cara Kerja
1. Semua edge pada graf diurutkan berdasarkan bobot secara ascending.
2. Iterasi setiap edge dari bobot terkecil.
3. Cek apakah penambahan edge akan membentuk siklus menggunakan Union-Find.
4. Jika tidak membentuk siklus, edge ditambahkan ke MST.
5. Proses berlanjut hingga jumlah edge di MST = **V-1** (V = jumlah simpul).

---

## 🚀 Contoh Penggunaan

```bash
python kruskal.py
```

Output:

```
Edges in the constructed MST
2 -- 3 == 4
0 -- 3 == 5
0 -- 1 == 10
Minimum Spanning Tree 19
```

---

## 📚 Referensi

* [GeeksforGeeks - Kruskal's Algorithm](https://www.geeksforgeeks.org/kruskals-algorithm-simple-implementation-for-adjacency-matrix/)
* [Wikipedia - Kruskal's Algorithm](https://en.wikipedia.org/wiki/Kruskal%27s_algorithm)

---

## 📝 Lisensi

```
Proyek ini menggunakan lisensi **MIT**.
```
