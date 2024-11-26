# Lab Activity 2 - State Management
- Mata Kuliah: Visual Programming
- Materi Minggu ke: 9

## **Tentang Proyek**
Proyek ini berisikan dua impelementasi State Management di Flutter yaitu:
1. **Ephemeral State Management** dengan menggunakan `StatefulWidget`
2. **App State Management** dengan menggunakan `scoped_model`

State Management merupakan salah satu komponen penting dalam pengembangan suatu aplikasi Flutter, terutama ketika bekerja dengan aplikasi yang lebih kompleks.

---
## **Perbedaan Utama**
Adapun perbedaan utama ketika kita menggunakan `StatefulWidget` dan `scoped_models` sebagai berikut:
| **Karakteristik**       | **Ephemeral State (StatefulWidget)**                          | **App State (Scoped Model)**                                 |
|--------------------------|--------------------------------------------------------------|-------------------------------------------------------------|
| **Penggunaan**           | Digunakan untuk state lokal sementara dalam satu widget.      | Digunakan untuk state global yang dibagikan antar widget.    |
| **Skalabilitas**         | Cocok untuk state sederhana seperti animasi atau form input. | Cocok untuk state kompleks seperti user authentication.      |
| **Reusability**          | Kurang reusable karena terikat langsung pada widget.         | Reusable, dapat digunakan di berbagai widget dalam aplikasi. |
| **Implementasi**         | Menggunakan `setState` untuk memperbarui UI.                 | Menggunakan `notifyListeners` untuk memperbarui seluruh UI. |
| **Kompleksitas**         | Mudah diterapkan untuk kebutuhan sederhana.                  | Lebih kompleks tetapi sangat fleksibel untuk aplikasi besar. |

---
## **Kesimpulan**
Kesimpulannya yaitu bahwa Ephemeral State Management cocok untuk kasus sederhana dengan state lokal yang sementara. Namun, App State Management seperti `scoped_model` lebih kuat dan fleksibel untuk aplikasi yang berskala besar dan kompleks. Dengan menggunakan Scoped Model, developer dapat mengelola state aplikasi secara efisien dan terstruktur, terutama dalam kasus penggunaan seperti **user authentication*, keranjang belanja (**shopping cart*), atau data global lainnya
