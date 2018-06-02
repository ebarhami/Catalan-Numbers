      #Catalan Numbers
      Ensof Barhami

>“Catalan numbers are the subject of [much] interest (sometimes known as Catalan disease)”
>~ Christian Aebi & Grant Cairns

Pernahkah mendengar istilah Bilangan Catalan atau Baris Catalan ? Bilangan Catalan memang bukan hal asing dalam dunia matematika. Bilangan ini juga banyak dikenal di dunia computer science (sangat berhubungan erat dengan triangulation problem atau salah satu persoalan graf di bidang computer science) . Bilangan ini sering kali muncul pada permasalahan-permasalahan enumerasi.
##Sejarah
Bilangan-bilangan Catalan terlihat sangat istimewa karena muncul di berbagai persoalan yang berbeda dengan solusi penyelesaian yang berbeda pula, namun memiliki solusi yang sama, yaitu bilangan-bilangan pada baris Catalan.
Seperti baris lain dalam dunia matematika, baris Catalan juga memiliki definisi. Uniknya, baris ini memiliki banyak sekali definisi dari banyak ahli matematika selama 200 tahun terakhir. Nama Catalan diambil dari nama seorang matematikawan asal Belgia, Eugene Charles Catalan yang mendefinisikan barisan ini pada tahun 1844 sebagai berikut.


Sehingga didapat barisan : 1, 1, 2, 5, 14, 42, 132, 429, 1430, ....
Sebenarnya, barisan ini sudah dikenal sejak tahun 1751 oleh Leonhard Euler. Euler menulis surat kepada salah satu sahabatnya yaitu Goldbach yang isinya adalah barisan yang kita kenal sekarang sebagai barisan Catalan. Didalam surat tersebut Euler mendefinisikan barisan bilangan Cn sebagai banyaknya triangulation dari (n+2)-gon (banyaknya cara membagi poligon menjadi segitiga-segitiga), di dalam surat tersebut ia juga menulis 8 bilangan pertama dari barisan ini yang dihitung secara manual olehnya. Pada awalnya, Euler memprediksi bilangan Cn ini sebagai :
C_(n-2) = (2 .6 .10 ...  (4n - 10))/(2 .  3 .  4 … (n-1))   . Contoh untuk C_4 = (2.6.10.14) / (2.3.4.5) = 14.
Goldbach membalas surat dari Euler dengan memberikan persamaan kuadrat yang bisa digunakan untuk menurunkan bilangan-bilangan catalan. Sejak saat itulah mereka membahas tentang bilangan ini, namun tidak langsung bisa mereka buktikan kebenaran dari formula yang ditulis Euler.
Selain Goldbach, terdapat juga tokoh yang semasa dengan Euler yaitu Johann Andreas von Segner yang berperan atas berkembangnya bilangan Catalan ini. Pada tahun 1750-an, Euler menceritakan tentang persoalan triangulation tadi kepada Segner namun tidak mengusulkan rumus yang dibuatnya kepada Segner. Euler “menantang” Segner untuk memecahkan persoalan ini secara matematis.
Pada tahun 1758, Segner menulis makalah yang sekaligus menjawab tantangan dari Euler. Ia menghasilkan relasi rekurens dengan pembuktian secara kombinatorik untuk mengenerate bilangan catalan sebagai berikut. 
C_(n+1) = C_0 C_n + C_1 C_(n-1) + ... + C_n C_0
Dengan formula ini, Segner dapat menentukan bilangan Catalan untuk n ≤ 18. Namun, ternyata ditemukan kesalahan pada C_13 dengan metode yang digunakan Segner.
	Setelah publikasi makalah oleh Segner, Euler menyadari bahwa tulisan Segner adalah “missing piece” yang dapat digunakan untuk memecahkan persoalan triangulation n-gon yang sedang menjadi fokusnya. Euler lalu menemukan letak kesalahan Segner dan pada akhirnya dapat menemukan bilangan Catalan sampai n ≤ 23. Menariknya, kombinasi dari hasil pikiran Euler, Goldbach, dan Segner pada akhirnya dapat membuktikan kebenaran formula yang diajukan Euler. Namun, pembuktian secara lengkap baru dipublikasi 80 tahun kemudian.
	Selain keempat orang diatas (Euler, Goldbach, Segner, dan tentu saja E.C Catalan) terdapat beberapa orang lagi yang berkontribusi untuk mengembangkan studi tentang barisan ini, antara lain Kotelnikov (menemukan pendekatan lain untuk membuktikan formula dari Euler), Fuss (mengenalkan apa yang sekarang kita kenal dengan Fuss-Catalan Numbers), Liouville (menggunakan Lagrange Inversion sebagai pembuktian), dan Gabriel Lame sampai pada akhirnya E.C Catalan terinspirasi dari tulisan Gabriel Lame dan merumuskan formula standar untuk bilangan Catalan seperti yang kita kenal sekarang. E.C Catalan jugalah yang menyadari bahwa persoalan triangulation ini ekivalen dengan persoalan bracket problem.
	Bilangan ini melewati perjalanan yang cukup panjang dalam perkembangannya. Pada literatur lama, kita tidak akan menemukan istilah “Catalan Numbers” tetapi Euler-Segners Numbers karena memang merekalah yang pertama mendiskusikan tentang bilangan ini. Berbagai teori tentang asal nama barisan ini pun kemudian bermunculan, namun pendapat yang paling kuat adalah nama “Catalan Numbers” ini mulai populer karena pada tahun 1968 seorang ahli kombinatorik asal Amerika menggunakan istilah ini di dalam bukunya, Combinatorial Identities sekaligus menjadi tulisan pertama yang menggunakan istilah “Catalan Numbers” untuk barisan yang sedang kita bahas.

##Aplikasi
Selain sejarahnya yang menarik, tentu saja barisan ini sendiri juga sangat menarik. Banyak sekali persoalan matematis yang banyak dikenal di dunia computer science saat ini yang mengandung Catalan Numbers. Berikut beberapa persoalan tersebut.
	Triangulation in polygon
Banyaknya triangulation yang dapat dibentuk dari sebuah poligon konvex dengan n+2 sisi adalah bilangan catalan ke-n 
Misal untuk n = 4, sisi poligon = 6, C_4=14
 
Triangulation digunakan di banyak bidang computer science salah satunya pada Art Gallery Problem. Dapat dilihat di makalah yang saya tulis di bit.ly/artgallerypaper
	Bracket Problem
Banyaknya ekspresi valid menggunakan n pasang tanda kurung adalah bilangan catalan ke-n (C_n).
Misal untuk n = 3, C_3=5
((())), ()(()), ()()(), (())(), (()())

	Dyck Words
Banyaknya Dyck words sepanjang 2n adalah bilangan catalan ke-n. Dyck words adalah string yang mengandung n-buah X dan n-buah Y sehingga tidak ada segmen awal dari string tersebut yang mengandung lebih banyak Y daripada X. Misal Dyck words valid dengan panjang 6 adalah : XXXYYY     XYXXYY     XYXYXY     XXYYXY     XXYXYY.

	Mountain Range
Banyaknya “pegunungan” dengan n-buah naikan dan n-buah turunan adalah bilangan catalan ke-n. Persoalana ini sama seperti persoalan Dyck Words.

 

	Noncrossing chords (Hands across a table)
Banyaknya jenis “salaman” dari 2n orang di meja bundar sedemikian hingga tidak ada tangan yang saling berpotongan.

 
Banyaknya salaman valid dengan n=4 adalah C_4=14

	Binary Trees
Banyaknya pohon biner yang memiliki n-buah internal node(s) adalah C_n.
Misal untuk n = 3, C_3=5

 
	Skew Polyominos
Banyaknya kumpulan petak yang membentuk suatu bentuk 2D dan memiliki keliling 2n+2 adalah C_n.
 

	Multiplication Orderings
Banyaknya susunan perkalian dengan n+1 bilangan adalah C_n.

 


##Hal unik lain :

 
Misal kita memiliki suatu titik R, Q dan P pada lingkaran dengan radius r seperti gambar diatas. OR = r , RP = 1 satuan , OQ = √(r^2-1). Panjang QP = r – OQ = r -  √(r^2-1). 
	Jika r = 5 QP = 0.10102051443364380..... Terlihat bilangan Catalan yang dipisahkan angka 0. 1,1,2,5,14.
	Jika r sangat besar, misal r = 5.000.000. QP = 0.00000010000000000000100000000000002000000000000050000000000001400000 00000004200000000000132000000000004290000000000143000000000004862000 00000016796000000000587860000000020801200000000742900000000026744400 00000096948450000003535767000000129644790000004776387000000176726319 00000656412042000024466267020000914825636400034305961365001289904147 32404861946401452183673530721526953355091600663747951750370022422166... Maka terlihat lebih banyak bilangan Catalan yang dipisahkan angka 0.

##Referensi
	- Makalah “Catalan Numbers” oleh Tom Davis, 2016
	- Makalah “Coding Object Related to Catalan Numbers” oleh Antal Bege & Zoltan Kasa, 2001
	- Makalah “History of Catalan Numbers” oleh Igor Pak UCLA, 2014
	- Makalah “Mencari Solusi Persamaan Rekursif Bilangan Catalan dengan Prinsip-prinsip Kombinatorial” oleh Ahmad Zaky, 2013.
	- https://www.geeksforgeeks.org/applications-of-catalan-numbers/

