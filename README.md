# general-information

## Overview

### Situasi saat ini
Saat ini Telkomsel masih mengandalkan vendor untuk membantu membangun sebagian besar sistem untuk mendukung pertumbuhan bisnisnya. Hal ini tidak dapat dihindari karena Telkomsel bukanlah perusahaan perangkat lunak yang memiliki tim pengembang dalam jumlah besar. Di sisi lain, hal ini membuat Telkomsel berada dalam posisi yang riskan karena ketergantungan terhadap vendor. 

Berdasarkan pengalaman, dari sisi vendor, terutama ketika kami membangun perangkat lunak khusus dan bukan produk COTS, hampir tidak ada standarisasi yang diterapkan di sisi mereka. Jika kita melihat sifat dari software house ketika programmer mereka datang dan pergi di luar kendali Telkomsel, hal ini dapat menyebabkan kualitas yang lebih buruk dari pengiriman dan peningkatan biaya pemeliharaan serta pengembangan lebih lanjut. 


Sebagai contoh: 

1. Vendor dapat memiliki beberapa proyek dan mengerahkan beberapa tim untuk menyelesaikannya. Dalam proyek-proyek tersebut, mereka mungkin menggunakan komponen perangkat lunak yang sama persis. Satu tim dapat menggunakan pendekatan yang berbeda, library yang berbeda, atau bahkan tech stack yang berbeda untuk memenuhi kebutuhan. Ini berarti kami tidak dapat mengelola konsistensi mereka. 

2. Para programmer berubah di luar kendali kita. Jika tidak ada standar yang harus diikuti, maka: 
    - Perekrutan akan sulit untuk fokus pada talenta teknologi tertentu sehingga akan sulit untuk mendapatkan talenta baru.

	- Anggota baru akan mengalami kesulitan untuk menyesuaikan diri dan membutuhkan kurva pembelajaran yang sangat curam terutama ketika mereka harus menggunakan stack yang berbeda dengan pekerjaan mereka sebelumnya.

	- Ketika mengalami kesulitan, anggota baru cenderung membangun kembali menggunakan apa yang mereka ketahui. Duplikasi proyek akan terjadi dan kualitas kode akan terancam. Hal yang sama juga terjadi ketika proyek/perangkat lunak diserahkan kepada vendor yang berbeda untuk melanjutkan pengembangan.

3. Pemilihan tech stack sebagian besar akan didasarkan pada apa yang mampu dilakukan oleh anggota tim, bukan pada apa yang paling cocok untuk kasus penggunaan tertentu.

4. Telkomsel tidak memiliki kontrol yang cukup untuk menentukan stack apa yang cocok untuk kebutuhan spesifik tersebut, pada akhirnya akan bergantung pada kesiapan dan kemampuan vendor (poin #3). 

5. Jika satu vendor dengan beberapa proyek dapat menggunakan stack yang berbeda, maka beberapa vendor dapat membawa stack mereka sendiri. Hal ini tentu menjadi tantangan yang signifikan dalam hal pemeliharaan, skalabilitas, dan kolaborasi dalam organisasi.

Dalam kondisi Telkomsel saat ini, beberapa aplikasi yang dibangun oleh vendor perlu dipelihara dan dilanjutkan oleh tim internal atau bahkan oleh vendor lain, standarisasi dalam bahasa pemrograman dan pemilihan tech stack menjadi hal yang sangat krusial dan penting. Hal ini membawa konsistensi, penyederhanaan pemeliharaan, dan menyederhanakan kolaborasi antar tim. Standardisasi meningkatkan skalabilitas, kesederhanaan proses orientasi, pengoptimalan biaya, serta menawarkan fleksibilitas dan ketahanan di masa depan.

### Pentingnya Standardisasi

- **Pemeliharaan yang Efisien**: Menstandarkan bahasa pemrograman dan komponen tumpukan teknologi di seluruh aplikasi akan menghadirkan konsistensi dan kesederhanaan dalam proses pemeliharaan. Ketika aplikasi yang berbeda menggunakan bahasa pemrograman, kerangka kerja, dan pustaka yang dipilih, akan lebih mudah bagi tim internal untuk memahami dan memeliharanya. Pengembang dapat memanfaatkan pengetahuan dan keahlian yang sudah ada, yang mengarah pada perbaikan bug yang lebih cepat, peningkatan sistem, dan peningkatan fitur, maka konsistensi akan tercapai. Tentu saja kami tidak berencana untuk mengadopsi satu bahasa pemrograman sebagai solusi untuk Telkomsel. Hal ini lebih kepada membuat pilihan berdasarkan apa yang sesuai dengan tujuan dalam aplikasi yang dibangun untuk Telkomsel.

- **Peningkatan Skalabilitas**: Standarisasi bahasa pemrograman dan tumpukan teknologi meningkatkan peluang skalabilitas. Ketika aplikasi dibangun menggunakan tech stack yang terstandardisasi, akan lebih mudah untuk mengintegrasikan dan menskalakan aplikasi tersebut seiring dengan pertumbuhan organisasi. Standardisasi mengurangi kerumitan yang terkait dengan pengintegrasian sistem yang beragam, memungkinkan komunikasi yang lancar dan pertukaran data antar aplikasi. Oleh karena itu, standarisasi memainkan peran penting dalam menskalakan aplikasi secara efektif.

- **Kemandirian Vendor**: Standarisasi bahasa pemrograman dan tumpukan teknologi memberikan lapisan kemandirian vendor, mengurangi ketergantungan pada vendor tertentu dan mengurangi risiko yang terkait dengan penguncian vendor. Dengan menggunakan teknologi yang umum diadopsi dan didukung dengan baik, organisasi dapat memastikan aplikasi mereka di masa depan dan menghindari potensi tantangan yang terkait dengan teknologi khusus vendor yang menjadi usang atau tidak didukung.

- **Kolaborasi yang Efisien**: Kolaborasi adalah landasan pengembangan perangkat lunak yang sukses. Ketika tim internal mewarisi aplikasi buatan vendor dengan berbagai tumpukan teknologi, hal ini dapat menghambat kolaborasi yang efektif di antara anggota tim. Standarisasi bahasa pemrograman dan tumpukan teknologi mendorong komunikasi yang lebih baik, berbagi pengetahuan, dan penggunaan ulang kode dalam organisasi. Pengembang dapat memanfaatkan keahlian kolektif mereka dan berkolaborasi dengan lancar, menghasilkan siklus pengembangan yang lebih cepat, mengurangi duplikasi upaya, dan meningkatkan koordinasi lintas tim. Kolaborasi ini juga dapat diperluas ke vendor kami, di mana dalam hal ini mereka harus mengikuti standar kami. Di sisi lain, sebagai bagian dari ekosistem Telkomsel, vendor juga dapat berkontribusi kepada Telkomsel untuk memenuhi standar ini.

- **Optimalisasi Biaya**: Standarisasi dapat mengarah pada optimalisasi biaya dengan mengurangi waktu dan upaya yang diperlukan untuk kegiatan pemeliharaan dan pengembangan. Ketika aplikasi berbagi tumpukan teknologi yang sama, akan lebih mudah untuk melatih dan mengalokasikan sumber daya secara efisien. Proses pengembangan dapat disederhanakan, dan sumber daya dapat digunakan bersama, sehingga mengurangi duplikasi upaya dan memaksimalkan produktivitas.

- **Orientasi dan Pengembangan Keterampilan yang Disederhanakan**: Standarisasi bahasa pemrograman dan komponen tech stack menyederhanakan proses orientasi untuk pengembang baru yang bergabung dengan organisasi. Dengan tech stack yang konsisten, anggota tim baru dapat dengan cepat beradaptasi, belajar, dan menjadi produktif karena mereka tidak perlu mempelajari berbagai bahasa atau framework. Selain itu, standarisasi memfasilitasi pengembangan keterampilan dalam organisasi, karena pengembang dapat mengkhususkan dan memperdalam keahlian mereka dalam bahasa atau kerangka kerja tertentu.

- **Pemeriksaan masa depan dan Fleksibilitas**: Menstandarkan bahasa pemrograman dan komponen tumpukan teknologi juga menawarkan pemeriksaan dan fleksibilitas di masa depan. Dengan memilih teknologi yang diadopsi dan didukung secara luas, organisasi mengurangi risiko penguncian vendor atau ketergantungan pada vendor tertentu. Tumpukan teknologi yang terstandardisasi memungkinkan integrasi yang lebih mudah dengan layanan dan teknologi pihak ketiga, sehingga organisasi dapat beradaptasi dan mengembangkan sistem mereka dengan lebih efisien. 

Dengan berinvestasi dalam standardisasi, organisasi dapat meletakkan fondasi yang kuat untuk pemeliharaan dan pengembangan aplikasi yang efisien, memberdayakan tim internal untuk memberikan solusi berkualitas tinggi secara efektif dan beradaptasi dengan perubahan kebutuhan bisnis yang sering terjadi. Dengan menerapkan standardisasi, organisasi dapat memanfaatkan manfaat dari tumpukan teknologi terpadu, sehingga mereka dapat mengelola dan mengembangkan portofolio aplikasi mereka secara efektif dengan percaya diri dan mudah.


## How to Define

Untuk membuat pedoman standarisasi library, Telkomsel membutuhkan framework dan workflows untuk memastikan kelancaran dan konsistensi operasional. Langkah pertama adalah menentukan apakah sebuah library cocok untuk dipilih sebagai library standar. Sebuah matriks diperlukan untuk memproses library baru menjadi library terpilih. Selain itu, workflow juga diperlukan untuk menyesuaikan standar yang ada dan untuk mengesampingkannya.

### Library Selection

For library selection, we utilize a matrix to gauge the library's market strength:

| Aspect        | Criteria                                       | Weight | Score     |
|---------------|------------------------------------------------|--------|-----------|
| Maintenance   | - 4 → within weeks                             | 0.1 - 1| 1 - 4     |
|               | - 3 → last month                               |        |           |
|               | - 2 → last 6 months                            |        |           |
|               | - 1 → last year                                |        |           |
| Reputable     | - 4 → worldwide known company                  | 0.1 – 1| 1 – 4     |
|               | - 3 → local known company                      |        |           |
|               | - 3 → worldwide known developer/team           |        |           |
|               | - 2 → local known developer/team               |        |           |
|               | - 1 → unknown developer                        |        |           |
| Compatibility | - 4 → very compatible                          | 0.1 – 1| 1 - 4     |
|               | - 3 → moderate compatible                      |        |           |
|               | - 2 → compatible with workaround               |        |           |
|               | - 1 → not compatible                           |        |           |
| Community     | - 4 → worldwide and local user                 | 0.1 – 1| 1 - 4     |
|               | - 3 → worldwide user                           |        |           |
|               | - 2 → local user                               |        |           |
|               | - 1 → few user                                 |        |           |
| Documentation | - 4 → web documented                           | 0.1 – 1| 1 - 4     |
|               | - 3 → md documented                            |        |           |
|               | - 2 → in source code documented                |        |           |
|               | - 1 → no documentation                         |        |           |
| Licensing     | - 4 → opensource                               | 0.1 – 1| 1 – 4     |
|               | - 3 → opensource with support                  |        |           |
|               | - 2 → pay to get the source                    |        |           |
|               | - 1 → pay not getting source                   |        |           |
| Extensible    | - 4 → easily extended                          | 0.1 – 1| 1 - 4     |
|               | - 3 → moderately extended                      |        |           |
|               | - 2 → hard to extend                           |        |           |
|               | - 1 → cannot be extended                       |        |           |
| Size          | - 4 → <10mb                                    | 0.1 – 1| 1 - 4     |
|               | - 3 → <100mb                                   |        |           |
|               | - 2 → <500mb                                   |        |           |
|               | - 1 → <1gb                                     |        |           |

Berikut adalah elaborasi dari setiap aspek yang tercantum di atas :

1. **Maintenance (Pemeliharaan)**  
   Menjelaskan seberapa sering library diperbarui dan status build terkini.

2. **Reputable (Reputasi)**  
   Mencerminkan seberapa dikenal pemelihara library, baik di tingkat lokal maupun internasional, serta persepsi publik.

3. **Compatibility (Kesesuaian)**  
   Menunjukkan kesesuaian library dengan arsitektur saat ini dan sistem warisan yang telah ada di Telkomsel.

4. **Community (Komunitas)**  
   Mendeskripsikan keterlibatan komunitas dengan library, apakah secara luas digunakan atau hanya digunakan oleh sekelompok kecil pengguna.

5. **Documentation (Dokumentasi)**  
   Menilai kelengkapan dokumentasi library, termasuk tutorial dan konsep dasar.

6. **Licensing (Lisensi)**  
   Membahas tentang syarat lisensi library, apakah bersifat open-source atau memerlukan pembayaran untuk mengaksesnya.

7. **Extensible (Keekstensifan)**  
   Mengevaluasi potensi library untuk dikembangkan dengan teknologi yang akan datang.

8. **Size (Ukuran)**  
   Memperhitungkan ukuran pustaka, karena ukuran yang lebih besar dapat meningkatkan biaya dalam lingkungan berbasis cloud.

## Tech Radar

Tech Radar adalah konsep atau alat yang digunakan untuk memantau dan mengkategorikan teknologi berdasarkan tingkat adopsi dan kelayakan penggunaannya dalam suatu organisasi atau industri. Konsep ini membantu organisasi dalam pengambilan keputusan terkait teknologi dengan menyediakan pandangan visual yang jelas tentang tren dan perkembangan dalam dunia teknologi.

Radar ada dalam bentuk grafis, mengelompokkan item-item ke dalam techniques, tools, platforms, dan languages and frameworks. Ketika item Radar bisa berada di banyak kuadran, maka pilih salah satu yang tampak paling tepat. Selanjutnya kelompokkan item dalam empat cincin untuk mencerminkan posisi mereka.

- Adopt: Teknologi yang telah terbukti berhasil dan diadopsi secara luas. Organisasi diharapkan untuk mengadopsi teknologi ini dengan percaya diri.
- Trial: Teknologi yang menunjukkan potensi nilai tinggi dan layak diuji dalam proyek-proyek kecil atau lingkup terbatas.
- Assess: Teknologi yang mungkin memiliki nilai, tetapi belum matang atau diuji sepenuhnya. Perlu dilakukan evaluasi lebih lanjut sebelum diadopsi secara luas.
- Hold: Teknologi yang telah mengalami pergeseran tren atau tidak lagi dianggap sebagai pilihan yang baik untuk diadopsi.

![tech radar](images/tech-radar.png)

### Reference
- [Tech Radar](https://www.thoughtworks.com/radar)
