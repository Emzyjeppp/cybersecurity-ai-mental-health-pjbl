# DRAFT LAPORAN PROJECT-BASED LEARNING (PjBL)
**UNIVERSITAS TEKNOLOGI DIGITAL INDONESIA**

---

## 1. HALAMAN SAMPUL (TEMPLATE)

```
                       PROJECT-BASED LEARNING
             MATA KULIAH: CYBERSECURITY DAN THREAT INTELLIGENCE

             
      KETIKA SOLUSI MENJADI BEBAN: PARADOKS OTOMASI AI DALAM 
     KESEHATAN MENTAL MAINTAINER OPEN SOURCE (STUDI KASUS:
                   MAINTAINER CURL & LINUX KERNEL)



                               Oleh:
                       MUHAMMAD JEPRI                 - 255410014
                       JUNSO SUAT                     - 215410133
                       BRIDGETTE DIANITA P. L.        - 225410012
                       YOSEFINA EMA                   - 215410113
                       HENDRI AGUNG PERMANA           - 235410035
                       OPAN SAPUTRA NAINGGOLAN        - 225410021



                        PROGRAM STUDI INFORMATIKA
                      FAKULTAS TEKNOLOGI INFORMASI
             UNIVERSITAS TEKNOLOGI DIGITAL INDONESIA
                                YOGYAKARTA
                                  2026
```

---

## 2. HALAMAN PENGESAHAN (TEMPLATE)

```
                        HALAMAN PENGESAHAN

JUDUL PROYEK PjBL   : Ketika Solusi Menjadi Beban: Paradoks Otomasi AI
                      Dalam Kesehatan Mental Maintainer Open Source 
                      (Studi Kasus: Maintainer Curl & Linux Kernel)
MATA KULIAH         : Cybersecurity Dan Threat Intelligence
PROGRAM STUDI       : Informatika
ANGGOTA KELOMPOK    : 1. Nama: MUHAMMAD JEPRI             NIM: 255410014
                      2. Nama: JUNSO SUAT                 NIM: 215410133
                      3. Nama: BRIDGETTE DIANITA P. L.    NIM: 225410012
                      4. Nama: YOSEFINA EMA               NIM: 215410113
                      5. Nama: HENDRI AGUNG PERMANA       NIM: 235410035
                      6. Nama: OPAN SAPUTRA NAINGGOLAN    NIM: 225410021

Menyatakan bahwa Laporan Project-Based Learning (PjBL) ini telah diperiksa, disetujui, dan disahkan sebagai salah satu syarat pemenuhan tugas mata kuliah Cybersecurity Dan Threat Intelligence pada Program Studi Informatika, Fakultas Teknologi Informasi, Universitas Teknologi Digital Indonesia.


                                            Yogyakarta, 11 Juli 2026
                                            Menyetujui,
                                            Dosen Pengampu Cybersecurity Dan
                                            Threat Intelligence




                                            Yudhi Kusnanto, S.Kom., M.Kom.
                                            NIDN/NIK. ...................
```

---

## 3. KATA PENGANTAR (TEMPLATE)

Puji syukur kami panjatkan ke hadirat Tuhan Yang Maha Esa atas berkat, rahmat, dan karunia-Nya, sehingga kami dapat menyelesaikan laporan tugas *Project-Based Learning* (PjBL) yang berjudul **"Ketika Solusi Menjadi Beban: Paradoks Otomasi AI Dalam Kesehatan Mental Maintainer Open Source"** tepat pada waktunya.

Tujuan dari penyusunan laporan ini adalah untuk memenuhi salah satu syarat kelulusan tugas mata kuliah Cybersecurity Dan Threat Intelligence pada Program Studi Informatika Universitas Teknologi Digital Indonesia. Proyek ini mengeksplorasi pergeseran paradigma keamanan siber dengan lahirnya pemindai kerentanan berbasis AI (*AI vulnerability scanner*) dan bagaimana hal tersebut berdampak langsung pada kesejahteraan mental pengembang yang memelihara infrastruktur digital dunia secara sukarela.

Dalam kesempatan ini, penulis ingin menyampaikan ucapan terima kasih yang tulus kepada:
1. Ibu Prof. Dr. LN. Harnaningrum, S.Si., M.T. selaku Wakil Rektor 1 Universitas Teknologi Digital Indonesia.
2. Bapak Yudhi Kusnanto, S.Kom., M.Kom., selaku Dosen Pengampu mata kuliah Cybersecurity Dan Threat Intelligence yang telah memberikan bimbingan, arahan, dan saran-saran berharga selama perencanaan dan penyusunan proyek ini.
3. Rekan-rekan anggota kelompok yang telah bekerja keras dan bekerja sama secara solid di sepanjang semester ini.

Kami menyadari bahwa laporan ini masih jauh dari kesempurnaan. Oleh karena itu, kritik dan saran yang membangun sangat kami harapkan guna perbaikan di masa mendatang. Akhir kata, semoga laporan PjBL ini dapat memberikan manfaat, wawasan, dan inspirasi bagi pembaca.

Yogyakarta, 11 Juli 2026

Tim Penulis

---

## 4. DAFTAR ISI (TEMPLATE)

```
HALAMAN SAMPUL ........................................................................ i
HALAMAN PENGESAHAN ................................................................... ii
KATA PENGANTAR ....................................................................... iii
DAFTAR ISI ............................................................................ iv
DAFTAR TABEL .......................................................................... v
DAFTAR GAMBAR ......................................................................... vi

BAB I PENDAHULUAN ..................................................................... 1
   1. Latar Belakang .................................................................. 1
   2. Rumusan Masalah ................................................................. 3
   3. Tujuan Perencanaan Project Based Learning ....................................... 3
   4. Batasan Masalah ................................................................. 4

BAB II TINJAUAN PUSTAKA ................................................................ 5
   1. Proyek Open Source dan Peran Maintainer ......................................... 5
   2. Large Language Models (LLM) dalam Pencarian Kerentanan Keamanan .................. 6
   3. Stres Kerja, Beban Kognitif, dan Burnout ........................................ 7

BAB III METODE PERENCANAAN ............................................................. 8
   1. Alur Penelitian ................................................................. 8
   2. Penjelasan Tahapan .............................................................. 9

BAB IV HASIL DAN PEMBAHASAN ........................................................... 11
   1. Studi Kasus 1: Proyek Curl & Timeline Keluhan (Februari - Mei 2026) .............. 11
   2. Studi Kasus 2: Linux Kernel & Risiko Chaining Celah Keamanan ..................... 12
   3. Ketimpangan Kerja AI (AI Labor Asymmetry) ....................................... 13
   4. Dampak Mental: Stres Kronis, Kecemasan Eksistensial, dan Burnout ................. 14
   5. Langkah Mitigasi Riil (Respons Curl & Linux Kernel) ............................. 15
   6. Usulan Kebijakan Lanjutan & Saran (Komunitas, UTDI, Peneliti) ................... 16

BAB V PENUTUP .......................................................................... 17
   1. Simpulan ........................................................................ 17
   2. Saran ........................................................................... 18

DAFTAR PUSTAKA ........................................................................ 19
LAMPIRAN .............................................................................. 20
```

---

## 5. DRAFT ISI UTAMA LAPORAN

### BAB I PENDAHULUAN

#### 1. Latar Belakang
Teknologi informasi global saat ini berdiri di atas fondasi perangkat lunak sumber terbuka (*Free and Open Source Software* atau FOSS). Proyek-proyek seperti Linux Kernel dan perangkat pustaka transfer data seperti `curl` ditanamkan di hampir setiap perangkat komputasi di dunia, mulai dari peluncur luar angkasa, infrastruktur perbankan, hingga gawai konsumen. Mayoritas proyek open source ini dikelola secara sukarela oleh sekelompok kecil pengembang (*maintainers*) yang bekerja atas dasar dedikasi, hati nurani, dan kebanggaan profesional.

Namun sejak awal tahun 2026, kemunculan kecerdasan buatan berbasis *Large Language Models* (LLM) seperti Claude Code dari Anthropic telah mengubah lanskap penemuan celah keamanan (*vulnerability discovery*). Dengan menggunakan perintah (*prompt*) yang sangat sederhana, siapapun kini dapat secara otomatis memindai seluruh direktori proyek open source berskala raksasa untuk menemukan kelemahan kode. 

Alih-alih mengurangi pekerjaan pengembang, kemudahan ini memicu fenomena penumpukan kerja yang belum pernah terjadi sebelumnya. Laporan celah keamanan otomatis membanjiri kotak masuk *maintainer*. Banyak laporan yang ternyata merupakan hasil halusinasi AI (*false positives*) atau laporan duplikat berkualitas rendah yang dikirimkan tanpa pemahaman teknis dari pengirimnya. Tekanan psikologis meningkat drastis karena pengembang merasa memiliki kewajiban moral untuk segera memverifikasi dan memperbaiki setiap celah demi menjaga keamanan miliaran perangkat pengguna global. Oleh karena itu, penting untuk menganalisis secara mendalam dampak teknologi AI/LLM terhadap kesehatan mental developer open source sebagai dasar merumuskan kebijakan perlindungan kontributor.

#### 2. Rumusan Masalah
Berdasarkan latar belakang di atas, rumusan masalah dalam PjBL ini adalah:
1. Bagaimana penetrasi teknologi AI/LLM dalam pencarian celah keamanan mengubah beban kerja developer proyek open source?
2. Apa saja dampak psikologis dan mental yang dialami oleh pengembang open source akibat banjir laporan keamanan otomatis berbasis AI?
3. Metode mitigasi dan kebijakan apa yang dapat diterapkan untuk melindungi kesehatan mental *maintainer* di era akselerasi AI?

#### 3. Tujuan Perencanaan Project-Based Learning
Tujuan dari perencanaan proyek pembelajaran ini adalah:
1. Menganalisis secara kualitatif dinamika beban kerja pengembang open source setelah kehadiran pemindai kerentanan berbasis LLM.
2. Mengidentifikasi spektrum gangguan kesehatan mental (seperti kecemasan kronis, beban kognitif berlebih, dan *burnout*) yang dihadapi kontributor open source.
3. Merumuskan rekomendasi kebijakan penanganan laporan berbasis AI yang etis dan ramah terhadap kesehatan mental pengembang.

#### 4. Batasan Masalah
Kajian dalam PjBL ini dibatasi pada ruang lingkup sebagai berikut:
1. Studi kasus berfokus pada dua proyek open source skala besar dan kritis, yaitu proyek `curl` (berdasarkan laporan Daniel Stenberg, 2026) dan Linux Kernel (berdasarkan data pindaian Anthropic Mythos, 2026).
2. Analisis dampak kesehatan mental didasarkan pada studi kualitatif literatur sekunder dari rilis pers, utas diskusi pengembang di forum LWN.net, dan catatan publikasi pribadi *maintainer*.
3. Fokus bahasan adalah dampak psikososial pada pengembang, bukan analisis statistik mendalam mengenai kode pemrograman siber itu sendiri.

---

### BAB II TINJAUAN PUSTAKA

#### 1. Proyek Open Source dan Peran Maintainer
Perangkat lunak open source dikembangkan secara kolaboratif. Pengembang utama yang memegang hak untuk menyetujui dan menggabungkan perubahan kode disebut sebagai *maintainer*. Peran *maintainer* sangat kompleks: mereka bertanggung jawab menguji kode kiriman komunitas, merilis versi terbaru, mengelola komunitas, dan yang paling krusial, mengatasi masalah keamanan. Karena sifatnya yang sukarela, keterbatasan tenaga kerja adalah kendala utama dalam FOSS.

#### 2. Large Language Models (LLM) dalam Pencarian Kerentanan Keamanan
Menurut investigasi Google Project Zero (2024) dan Anthropic (2026), model bahasa besar modern memiliki kemampuan penalaran kontekstual yang kuat untuk menganalisis kode sumber. Dengan perintah sederhana seperti instruksi pemindaian berbasis skrip shell (menggunakan model seperti Claude Opus dan Mythos Preview), pengguna dapat menemukan bug rumit seperti *buffer overflow* atau *use-after-free*. Namun, model ini tetap rentan memproduksi *hallucinated code*—masalah keamanan yang terdengar meyakinkan tetapi secara praktis salah.

#### 3. Stres Kerja, Beban Kognitif, dan Burnout
Dalam psikologi kerja, *burnout* adalah kondisi kelelahan emosional, fisik, dan mental yang disebabkan oleh stres berlebih dan berkepanjangan. Beban kognitif terjadi ketika kapasitas memori kerja manusia kewalahan oleh stimulasi informasi yang datang bertubi-tubi. Bagi pengembang open source, tuntutan untuk selalu siap siaga memperbaiki celah kritis tanpa dukungan finansial atau emosional memicu "sindrom tanggung jawab moral" (*moral responsibility syndrome*) yang mempercepat keputusasaan dan kelelahan mental.

---

### BAB III METODE PERENCANAAN

#### 1. Alur Penelitian (Flowchart)

Berikut adalah flowchart metodologi analisis data dalam proyek PjBL ini:

```mermaid
graph TD
    A[Mulai] --> B[Identifikasi Masalah: Penetrasi AI & Stres Developer]
    B --> C[Pengumpulan Data Sekunder: Artikel LWN.net & Catatan Daniel Stenberg]
    C --> D[Analisis Studi Kasus 1: Kasus Curl - Lonjakan CVE 2026]
    C --> E[Analisis Studi Kasus 2: Linux Kernel - Scan Anthropic Mythos]
    D --> F[Identifikasi Dampak Kualitatif: Beban Kerja vs Kesehatan Mental]
    E --> F
    F --> G[Sintesis Rekomendasi Mitigasi & Proteksi Maintainer]
    G --> H[Penyusunan Laporan & Simpulan Akhir]
    H --> I[Selesai]
```

#### 2. Penjelasan Tahapan
1. **Identifikasi Masalah**: Mengkaji awal fenomena penggunaan AI untuk meluncurkan laporan bug massal ke repositori FOSS.
2. **Pengumpulan Data**: Melacak dokumen resmi rilis siber, esai blog maintainer (*Daniel's blog*), serta komentar-komentar kontributor di portal LWN.net.
3. **Analisis Kasus**: Membagi analisis ke dalam dua kategori: proyek berorientasi utilitas spesifik (`curl`) dan sistem operasi masif (Linux Kernel).
4. **Sintesis Rekomendasi**: Menyusun pedoman bagaimana komunitas menyikapi laporan dari AI agar meminimalkan kelelahan kontributor.

---

### BAB IV HASIL DAN PEMBAHASAN

#### 1. Studi Kasus 1: Proyek Curl & Timeline Keluhan (Februari - Mei 2026)
Curl adalah pustaka transfer data yang dirawat oleh satu karyawan penuh waktu, Daniel Stenberg, namun ditanam di miliaran perangkat. Dampak otomasi AI memicu pergeseran drastis pada beban kerja:
* **Februari 2026 (FOSDEM Keynote)**: Keluhan awal berkisar pada rendahnya kualitas laporan AI (*AI slop*). Pengembang menghabiskan waktu berjam-jam untuk membantah laporan keamanan yang salah (*false positives*) dan tidak berdasar.
* **Mei 2026 (Esai "The Pressure")**: Kualitas laporan AI meningkat tajam menjadi "benar-benar bagus" dan sulit dibantah kebenarannya. Namun, hal ini justru memicu rekor buruk berupa **12 kerentanan terkonfirmasi dalam satu siklus rilis** (proyeksi ~60 CVE sepanjang 2026). Waktu pengembang tersedot habis hanya untuk memverifikasi laporan-laporan valid yang membanjiri kotak masuk.

#### 2. Studi Kasus 2: Linux Kernel & Risiko Chaining Celah Keamanan
Sebagai sasaran utama otomasi ofensif, Linux Kernel menghadapi volume laporan mentah yang luar biasa besar:
* **Banjir Laporan Rekor**: Meskipun laporan CVE kernel sempat melandai, volume laporan mentah sebelum triase tetap melonjak tinggi. Secara industri lintas perangkat lunak, Maret 2026 memecahkan rekor dengan **6.243 CVE baru** (171 di antaranya adalah CVE kernel Linux, melonjak dari 64 di bulan Januari).
* **Risiko Chaining (Perangkaian Celah)**: Tim riset Anthropic memegang kendali atas lebih dari **500 potensi crash kernel** dari model Claude Mythos Preview. Bahaya terbesar adalah kemampuan AI untuk **merangkai (chaining) belasan celah kecil** (seperti *buffer overflow*, *use-after-free*, *double-free*) yang jika berdiri sendiri tidak berbahaya karena tertahan pertahanan *defense-in-depth*, namun secara kolektif dapat dieksploitasi untuk meraih akses root penuh ke kernel. Hal ini menambah beban mental tim keamanan karena mereka tidak bisa hanya menguji bug secara terpisah.

#### 3. Ketimpangan Kerja AI (AI Labor Asymmetry)
Analisis membuktikan adanya ketimpangan beban kerja (*labor asymmetry*) yang ekstrem:
* **Sisi Ofensif (Pencari Celah)**: Memanfaatkan skrip shell otomatis dan prompt bergaya CTF (*Capture the Flag*) dengan biaya token murah (di bawah $20 per pemindaian) tanpa perlu memahami arsitektur kode secara mendalam.
* **Sisi Defensif (Maintainer Manusia)**: Menanggung seluruh beban fisik dan mental untuk mereproduksi crash secara manual, membaca ratusan halaman dokumen keluaran AI, menulis kode penambal (*patch*), hingga berdebat kusir dengan pengirim laporan yang tidak memahami isinya dan membalas argumen menggunakan LLM.

#### 4. Dampak Mental: Stres Kronis, Kecemasan Eksistensial, dan Burnout
Dampak psikologis yang dirasakan pengembang sukarela mencakup:
1. **Stres Tanggung Jawab Moral**: Kecemasan konstan terhadap risiko kegagalan infrastruktur digital dunia yang bertumpu pada kode mereka.
2. **Kelelahan Kognitif Akut**: Kejenuhan mental akibat membaca gaya bahasa AI yang seragam, berulang, dan minim keaslian emosional.
3. **Keputusasaan Eksistensial**: Perasaan bahwa kapasitas linear manusia tidak akan pernah mampu mengimbangi laju pertumbuhan laporan siber eksponensial dari mesin AI.

#### 5. Langkah Mitigasi Riil (Respons Curl & Linux Kernel)
Bukan sekadar wacana, langkah-langkah konkret yang telah terjadi di lapangan meliputi:
1. **Curl Summer of Bliss**: Proyek `curl` menghentikan sementara penerimaan laporan bug keamanan baru di HackerOne dan email (1 Juli - 3 Agustus 2026) agar tim keamanan memiliki waktu istirahat dari tekanan triase harian.
2. **Penutupan Program Bug Bounty**: `curl` resmi menghentikan skema bug bounty berbayar sejak awal 2026 untuk menghentikan banjir kiriman laporan AI berorientasi finansial yang membebani mental pengembang.
3. **Perubahan Kebijapan Embargo Kernel Linux**: Kebijakan diubah agar temuan kerentanan siber berbasis AI langsung dipublikasikan sejak awal (tidak dirahasiakan), guna meminimalkan koordinasi ganda yang rumit dan melelahkan.
4. **Penciutan Kode (Code Deprecation)**: Kernel Linux mengusulkan penghapusan beberapa subsistem kuno rawan bug yang jarang dipakai (seperti ISA/PCMCIA, AX.25, ATM, ISDN) untuk memperkecil luas serangan.
5. **Project Glasswing**: Kemitraan industri dipimpin Linux Foundation untuk menyalurkan dana dan memberikan akses LLM pertahanan termutakhir bagi maintainer.

#### 6. Usulan Kebijakan Lanjutan & Saran (Komunitas, UTDI, Peneliti)
Bagi proyek open source lain yang belum bertindak, proyek PjBL ini merekomendasikan:
1. **Moratorium Berkala**: Mengadopsi jeda triase terjadwal secara periodik untuk pemulihan mental tim developer.
2. **Evaluasi Insentif Bug Bounty**: Menyesuaikan atau meniadakan hadiah tunai pada laporan siber otomatis tanpa pembuktian manual yang kuat.
3. **Aturan Triase yang Tegas**: Kebijakan formal untuk menolak langsung laporan yang dikirimkan tanpa langkah reproduksi dan verifikasi manual dari pengirim.
4. **Asisten Triase AI Terpercaya**: Penggunaan AI defensif internal yang dilatih khusus untuk menyaring laporan duplikat dan halusinasi AI sebelum dibaca pengembang manusia.

---

### BAB V PENUTUP

#### 1. Simpulan
Berdasarkan hasil analisis kualitatif dalam proyek PjBL ini, dapat ditarik simpulan:
1. Pemanfaatan AI/LLM dalam pencarian bug telah mengganggu stabilitas ekosistem open source secara drastis melalui peningkatan volume laporan CVE hingga rekor tertinggi pada paruh pertama tahun 2026.
2. Dampak kesehatan mental yang dialami oleh pengembang bersifat nyata dan merusak, ditandai dengan stres akibat tuntutan tanggung jawab moral yang besar, keletihan kognitif, serta kecemasan konstan terhadap serangan *zero-day*.
3. Masalah utama terletak pada ketimpangan kerja (*asymmetry of labor*) antara pelapor yang menggunakan otomasi mesin dan maintainer yang menyaring secara manual.

#### 2. Saran
Adapun saran yang dapat dirumuskan melalui proyek PjBL ini ditujukan kepada:
1. **Komunitas Open Source**: Membuka diri terhadap adopsi jeda periodik (moratorium), memperjelas kebijakan penanganan bug AI, serta menerapkan filter ketat untuk laporan tanpa verifikasi manual.
2. **Kita sebagai Mahasiswa**: Meningkatkan kesadaran moral sejak masa perkuliahan mengenai pentingnya etika penggunaan otomasi AI, tidak mengeksploitasi alat pemindai AI secara instan tanpa verifikasi manual yang dapat membebani pengembang, serta aktif mengkampanyekan pentingnya kesehatan mental dalam ekosistem rekayasa perangkat lunak.
3. **Peneliti Selanjutnya**: Melakukan studi kuantitatif klinis berupa penyebaran kuesioner stres kerja secara acak langsung kepada para pengembang aktif FOSS di tingkat global untuk mendapatkan data objektif yang lebih presisi.

---

## 6. DAFTAR PUSTAKA (GAYA PENULISAN UTDI)

Alden, Daroc, 2026, *A flood of useful security reports*, LWN.net, https://lwn.net/Articles/1066581/ (diakses pada 8 Juli 2026 pukul 21.05 WIB).

Corbet, Jonathan, 2026, *Stenberg: The pressure*, LWN.net, https://lwn.net/Articles/1074449/ (diakses pada 8 Juli 2026 pukul 21.05 WIB).

Stenberg, Daniel, 2026, *The Pressure*, Daniel's Blog, https://daniel.haxx.se/blog/2026/05/26/the-pressure/ (diakses pada 8 Juli 2026 pukul 21.10 WIB).

Google Project Zero, 2024, *Project Naptime: Evaluating LLMs on Vulnerability Research*, Project Zero Blog, https://projectzero.google/2024/06/project-naptime.html (diakses pada 8 Juli 2026 pukul 21.15 WIB).
