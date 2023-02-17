
## Tinjauan Singkat PBO

OOP atau Object-Oriented Programming adalah paradigma pemrograman yang memungkinkan pengembang perangkat lunak untuk memodelkan dunia nyata dalam program. Paradigma ini berfokus pada konsep objek dan data, bukan hanya pada fungsi dan logika. Dalam OOP, suatu program terdiri dari objek yang saling berinteraksi untuk mencapai tujuan tertentu.

Dalam OOP, objek dibuat dari kelas, yang mendefinisikan struktur dan perilaku objek. Suatu kelas dapat memiliki properti atau variabel dan metode atau fungsi yang dapat digunakan untuk memanipulasi objek tersebut. Properti dapat digunakan untuk menyimpan data, sementara metode dapat digunakan untuk melakukan tugas tertentu.

OOP memiliki konsep pewarisan (inheritance), yang memungkinkan kelas untuk mewarisi properti dan metode dari kelas lain. Konsep ini memungkinkan pengembang untuk memanfaatkan kode yang sudah ada dan mencegah duplikasi kode yang tidak perlu.

OOP juga memiliki konsep polimorfisme, yang memungkinkan pengembang untuk menggunakan objek dari kelas yang berbeda secara bersamaan dengan cara yang sama. Konsep ini memungkinkan pengembang untuk membuat kode yang lebih fleksibel dan mudah dipelihara.

Dalam OOP, data dan fungsi terkait dibungkus dalam suatu objek, yang membuatnya lebih mudah untuk dimengerti dan dipelihara. OOP juga memungkinkan pengembang untuk memisahkan kode ke dalam modul yang terpisah, yang memungkinkan kode untuk dikelola secara lebih efisien.

Karakteristik OOP dan prosedural memang memiliki perbedaan mendasar. Berikut adalah perbedaan antara karakteristik OOP dan prosedural:

1. Pemrograman Berbasis Objek: OOP berfokus pada objek yang memiliki properti dan metode. Pada prosedural, program terdiri dari serangkaian prosedur atau fungsi yang beroperasi pada data.
2. Encapsulation: OOP menggunakan konsep encapsulation, di mana data dan fungsi terkait dibungkus dalam suatu objek, yang membuatnya lebih mudah untuk dimengerti dan dipelihara. Pada prosedural, data dan fungsi terpisah dan tidak dibungkus bersama.
3. Inheritance: OOP memungkinkan kelas untuk mewarisi properti dan metode dari kelas lain. Konsep ini memungkinkan pengembang untuk memanfaatkan kode yang sudah ada dan mencegah duplikasi kode yang tidak perlu. Prosedural tidak memiliki konsep pewarisan ini.
4. Polymorphism: OOP juga memiliki konsep polimorfisme, yang memungkinkan pengembang untuk menggunakan objek dari kelas yang berbeda secara bersamaan dengan cara yang sama. Konsep ini memungkinkan pengembang untuk membuat kode yang lebih fleksibel dan mudah dipelihara. Prosedural tidak memiliki konsep ini.
5. Fokus pada Data: Dalam OOP, program berfokus pada data dan objek. Sementara pada prosedural, program berfokus pada prosedur atau fungsi.
6. Keterbacaan kode: Kode yang ditulis dengan paradigma OOP cenderung lebih mudah dibaca dan dimengerti karena objek dan metode yang terkait dibungkus bersama. Sedangkan pada paradigma prosedural, fungsi-fungsi terpisah dan tidak memiliki hubungan antara satu dengan yang lainnya.

Perbedaan-perbedaan tersebut menjadikan OOP lebih mudah digunakan, dipelihara dan dikembangkan dalam skala besar. Namun, pemrograman prosedural masih lebih cocok digunakan pada skala kecil dan sederhana.

### Contoh Kode Pemrograman Berorientasi Obyek
Berikut ini adalah contoh perbedaan program yang dibuat dengan menggunakan metode prosedural dan OOP dengan menggunakan bahasa Python:

1. Program dengan metode prosedural:
```python
# Fungsi untuk menghitung luas segitiga
def hitung_luas_segitiga(alas, tinggi):
    luas = (alas * tinggi) / 2
    return luas

# Input alas dan tinggi dari user
alas = float(input("Masukkan alas segitiga: "))
tinggi = float(input("Masukkan tinggi segitiga: "))

# Panggil fungsi hitung_luas_segitiga
luas_segitiga = hitung_luas_segitiga(alas, tinggi)

# Cetak hasil perhitungan
print("Luas segitiga adalah:", luas_segitiga)

```
Pada program di atas, fungsi `hitung_luas_segitiga` digunakan untuk menghitung luas segitiga dengan menggunakan rumus `0.5 * alas * tinggi`. Data input diperoleh dari user melalui fungsi `input()`. Setelah itu, fungsi `hitung_luas_segitiga` dipanggil dengan argumen yang diperoleh dari user, dan hasil perhitungan dicetak ke layar.

2. Program dengan metode OOP:
```python
# Definisikan kelas Segitiga
class Segitiga:
    def __init__(self, alas, tinggi):
        self.alas = alas
        self.tinggi = tinggi
        
    def hitung_luas(self):
        return 0.5 * self.alas * self.tinggi

# Input alas dan tinggi dari user
alas = float(input("Masukkan alas segitiga: "))
tinggi = float(input("Masukkan tinggi segitiga: "))

# Buat objek dari kelas Segitiga
segitiga = Segitiga(alas, tinggi)

# Panggil metode hitung_luas
luas_segitiga = segitiga.hitung_luas()

# Cetak hasil perhitungan
print("Luas segitiga adalah:", luas_segitiga)

```
Pada program di atas, terdapat kelas `Segitiga` yang memiliki atribut `alas` dan `tinggi`, serta metode `hitung_luas` untuk menghitung luas segitiga. Data input diperoleh dari user dengan fungsi `input()`. Setelah itu, objek `segitiga` dibuat dengan argumen yang diperoleh dari user, dan metode `hitung_luas` dipanggil dari objek `segitiga`. Hasil perhitungan kemudian dicetak ke layar.

Perbedaan utama antara program dengan metode prosedural dan OOP adalah pada pendekatan yang digunakan. Pada program dengan metode prosedural, fungsi digunakan sebagai unit terkecil yang memproses data. Sedangkan pada program dengan metode OOP, objek digunakan sebagai unit terkecil yang memiliki sifat dan perilaku. Pendekatan OOP lebih modular dan memungkinkan untuk membuat program yang lebih mudah dipelihara dan dikembangkan.

## Pilar OOP

### Abstraksi 

Abstraksi dalam OOP adalah konsep yang memungkinkan kita untuk memisahkan informasi penting dan hanya menampilkan informasi yang diperlukan kepada pengguna. Dalam konteks pemrograman, abstraksi mengacu pada pembuatan representasi yang lebih sederhana dan lebih mudah dipahami dari suatu objek. Dalam OOP, objek dapat dianggap sebagai wujud nyata dari sebuah kelas, dan abstraksi dapat membantu dalam membuat kelas tersebut lebih mudah dipahami dan digunakan.

Salah satu contoh abstraksi dalam OOP adalah penggunaan metode. Sebuah kelas dapat memiliki beberapa metode yang melakukan tugas tertentu pada objek yang dihasilkan dari kelas tersebut. Namun, ketika menggunakan objek, kita tidak perlu mengetahui detail bagaimana metode bekerja di dalam kelas, tetapi hanya perlu mengetahui cara mengakses dan menggunakan metode tersebut.

Abstraksi juga dapat membantu dalam membangun hierarki kelas yang lebih kompleks. Misalnya, dalam membuat sebuah game, kita dapat membangun kelas yang merepresentasikan objek-objek dalam game, seperti karakter, musuh, atau item. Kita dapat membuat kelas-kelas ini lebih abstrak dan mudah digunakan dengan menetapkan properti dan metode yang cocok untuk setiap kelas, serta mengelompokkannya ke dalam hierarki kelas yang lebih besar.

Di Python, abstraksi dapat dilakukan dengan menggunakan konsep class. Berikut adalah contoh implementasi abstraksi di Python:

```python
class Shape:
    def area(self):
        pass

    def perimeter(self):
        pass

class Rectangle(Shape):
    def __init__(self, length, breadth):
        self.length = length
        self.breadth = breadth

    def area(self):
        return self.length * self.breadth

    def perimeter(self):
        return 2 * (self.length + self.breadth)

class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return 3.14 * self.radius * self.radius

    def perimeter(self):
        return 2 * 3.14 * self.radius

r = Rectangle(4, 5)
print("Area of rectangle:", r.area())
print("Perimeter of rectangle:", r.perimeter())

c = Circle(7)
print("Area of circle:", c.area())
print("Perimeter of circle:", c.perimeter())
```

Pada contoh di atas, terdapat sebuah class `Shape` yang merupakan sebuah abstraksi dari bentuk geometri. Di dalam class `Shape` terdapat dua method yang belum diimplementasikan, yaitu `area()` dan `perimeter()`. Kemudian, terdapat dua class lain, yaitu `Rectangle` dan `Circle`, yang mewarisi class `Shape` dan mengimplementasikan method `area()` dan `perimeter()` sesuai dengan karakteristik masing-masing bentuk geometri.

Dengan menggunakan abstraksi seperti ini, kita dapat membuat objek yang merepresentasikan bentuk geometri tertentu tanpa perlu memikirkan detail implementasi dari method `area()` dan `perimeter()`.

### Enkapsulasi

Enkapsulasi dalam OOP adalah konsep untuk menyembunyikan informasi yang tidak perlu dipublikasikan, dan hanya memperbolehkan akses ke informasi tersebut melalui metode atau properti tertentu. Dalam enkapsulasi, data dan fungsionalitas di dalam suatu objek dikemas bersama dan dilindungi dari akses atau modifikasi dari luar. Dalam OOP, enkapsulasi sering dianggap sebagai salah satu pilar utama, selain abstraksi, pewarisan (inheritance), dan polimorfisme.

Konsep enkapsulasi memungkinkan programmer untuk membatasi akses ke informasi penting dalam objek, sehingga dapat mencegah perubahan yang tidak diinginkan atau kesalahan dalam program. Hal ini juga memungkinkan kita untuk memperbarui atau mengubah struktur internal objek tanpa mempengaruhi kode yang menggunakannya, karena kode tersebut hanya menggunakan antarmuka publik objek dan tidak terpengaruh oleh perubahan di dalamnya.

Dalam OOP, enkapsulasi biasanya diimplementasikan menggunakan access modifiers seperti private, protected, dan public pada properti dan metode dalam sebuah class. Dengan menentukan access modifiers, kita dapat mengatur level akses yang dibutuhkan oleh pengguna kode terhadap informasi dalam objek.

Contoh penggunaan enkapsulasi adalah dengan menentukan properti sebagai private, yang hanya dapat diakses melalui metode publik. Dengan begitu, data dalam objek tetap terlindungi dan pengguna kode hanya dapat mengakses dan memodifikasi data melalui metode yang telah ditetapkan oleh programmer.

Berikut ini adalah contoh implementasi enkapsulasi dalam OOP menggunakan bahasa pemrograman Python:

```python
class Mobil:
    def __init__(self, merk, warna):
        self.__merk = merk
        self.__warna = warna

    def set_merk(self, merk):
        self.__merk = merk

    def set_warna(self, warna):
        self.__warna = warna

    def get_merk(self):
        return self.__merk

    def get_warna(self):
        return self.__warna

mobil1 = Mobil("Toyota", "Merah")
print(mobil1.get_merk()) # Output: Toyota
print(mobil1.get_warna()) # Output: Merah

mobil1.set_merk("Honda")
mobil1.set_warna("Biru")
print(mobil1.get_merk()) # Output: Honda
print(mobil1.get_warna()) # Output: Biru

```

Dalam contoh tersebut, terdapat class `Mobil` yang memiliki dua atribut yaitu `merk` dan `warna`. Atribut tersebut di-set menggunakan method `set_merk` dan `set_warna`, sedangkan untuk mendapatkan nilai atribut digunakan method `get_merk` dan `get_warna`.

Namun, terdapat karakter `_` (underscore) ganda sebelum nama atribut `merk` dan `warna`. Ini menandakan bahwa atribut tersebut bersifat `private`, sehingga tidak dapat diakses dari luar class. Oleh karena itu, diperlukan method `set` dan `get` untuk mengakses dan mengubah nilai atribut tersebut dari luar class. Dengan cara ini, enkapsulasi tercapai dan data yang terdapat pada class `Mobil` dapat lebih aman terjaga dari perubahan yang tidak diinginkan.

### Pewarisan

Pewarisan (inheritance) dalam OOP adalah konsep di mana sebuah class dapat mewarisi properti dan metode dari class lain yang sudah ada. Class yang mewarisi disebut subclass atau child class, sementara class yang diwarisi disebut superclass atau parent class.

Dalam pewarisan, subclass dapat memiliki semua properti dan metode dari superclass, serta dapat menambahkan properti dan metode khusus mereka sendiri. Konsep ini memungkinkan penggunaan kembali kode dan mempermudah pengembangan program.

Pewarisan juga memungkinkan adanya hubungan antar kelas yang lebih kompleks, seperti hierarki class, sehingga dapat membantu mengorganisir dan memahami struktur program secara lebih baik.

Berikut adalah contoh sederhana pewarisan dalam OOP dengan Python:

```python
class Animal:
    def __init__(self, name):
        self.name = name
        
    def move(self):
        print(f"{self.name} is moving.")
        
class Cat(Animal):
    def __init__(self, name):
        super().__init__(name)
        
    def meow(self):
        print("Meow!")
```

Dalam contoh ini, terdapat dua class, yaitu `Animal` dan `Cat`. Class `Cat` mewarisi semua properti dan metode dari class `Animal` menggunakan sintaksis `class ChildClass(ParentClass):`.

Pada class `Animal`, terdapat properti `name` dan metode `move()`, yang berfungsi untuk menampilkan pesan bahwa hewan tersebut sedang bergerak.

Class `Cat` kemudian mewarisi properti `name` dan metode `move()` dari class `Animal` melalui sintaksis `class Cat(Animal):`. Selain itu, class `Cat` juga memiliki metode `meow()`, yang digunakan untuk menampilkan pesan "Meow!".

Dengan pewarisan, class `Cat` dapat menggunakan properti dan metode dari class `Animal` tanpa perlu menuliskan ulang kode yang sudah ada pada class `Animal`. Sebagai contoh, jika ingin membuat objek `Cat`, dapat dilakukan dengan sintaksis sebagai berikut:

```python
my_cat = Cat("Whiskers")
my_cat.move()  # Output: Whiskers is moving.
my_cat.meow()  # Output: Meow!
```

### Polimorfisme

Polimorfisme adalah konsep dalam OOP yang memungkinkan suatu objek untuk memiliki banyak bentuk atau perilaku yang berbeda. Dalam konteks ini, suatu objek dapat diperlakukan sebagai objek yang berbeda tergantung pada konteks penggunaannya.

Dalam OOP, polimorfisme dapat dicapai melalui konsep pewarisan dan antarmuka (interface). Pewarisan memungkinkan objek turunan (child class) untuk mewarisi properti dan metode dari objek induk (parent class), sementara antarmuka memungkinkan objek untuk mengimplementasikan perilaku yang berbeda pada waktu yang berbeda.

Sebagai contoh, dalam sebuah program aplikasi perpustakaan, polimorfisme dapat dicapai dengan membuat kelas induk "Item" yang memiliki beberapa metode dan properti, seperti "judul", "penulis", dan "penerbit". Kemudian, kelas turunan seperti "Buku" dan "CD" dapat mewarisi properti dan metode dari kelas induk ini. Setelah itu, dapat dipanggil metode seperti "cetakDetail" yang akan menghasilkan output yang berbeda tergantung pada objek yang dipanggil.

Berikut adalah contoh implementasi polimorfisme pada Python menggunakan konsep pewarisan dan antarmuka:

```python
# Contoh polimorfisme dengan pewarisan pada Python

class Hewan:
    def suara(self):
        pass

class Kucing(Hewan):
    def suara(self):
        print("Meow")

class Anjing(Hewan):
    def suara(self):
        print("Guk guk")

hewan = [Kucing(), Anjing()]

for h in hewan:
    h.suara()
    
# Output:
# Meow
# Guk guk

# Contoh polimorfisme dengan antarmuka pada Python

class Kendaraan:
    def naik(self):
        pass

class Mobil(Kendaraan):
    def naik(self):
        print("Naik mobil")

class Motor(Kendaraan):
    def naik(self):
        print("Naik motor")

def naik_kendaraan(kendaraan):
    kendaraan.naik()

mobil = Mobil()
motor = Motor()

naik_kendaraan(mobil) # Output: Naik mobil
naik_kendaraan(motor) # Output: Naik motor
```

Dalam contoh-contoh tersebut, polimorfisme dicapai melalui implementasi metode "suara" dan "naik" yang berbeda pada kelas turunan "Kucing", "Anjing", "Mobil", dan "Motor". Selanjutnya, objek "hewan" dan "kendaraan" dipanggil melalui metode "suara" dan "naik" yang sama, tetapi menghasilkan output yang berbeda tergantung pada objek yang dipanggil.

## Hubungan Antar Objek

### Generalization

Dalam OOP, generalisasi mengacu pada membuat kelas induk atau superclass yang memiliki atribut dan metode yang sama dengan kelas anak atau subclass. Kelas anak mewarisi atribut dan metode dari kelas induk, tetapi juga dapat memiliki atribut dan metode tambahan yang unik untuk kelas anak.

Berikut ini adalah contoh generalisasi menggunakan bahasa pemrograman Python:

```python
class Shape:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def area(self):
        pass

class Rectangle(Shape):
    def __init__(self, x, y, width, height):
        super().__init__(x, y)
        self.width = width
        self.height = height

    def area(self):
        return self.width * self.height

class Circle(Shape):
    def __init__(self, x, y, radius):
        super().__init__(x, y)
        self.radius = radius

    def area(self):
        return 3.14 * (self.radius ** 2)

r = Rectangle(0, 0, 10, 5)
print(r.area())  # Output: 50

c = Circle(0, 0, 5)
print(c.area())  # Output: 78.5
```

Dalam contoh di atas, `Shape` adalah kelas induk atau superclass, sedangkan `Rectangle` dan `Circle` adalah kelas anak atau subclass. Kedua kelas anak mewarisi atribut `x` dan `y` dari kelas induk, tetapi memiliki metode `area` yang berbeda. Metode `area` di kelas anak menghitung luas dari bentuk yang sesuai (persegi panjang untuk `Rectangle` dan lingkaran untuk `Circle`).

### Specialization

Di dalam pemrograman berorientasi objek, konsep specialisasi mengacu pada pembuatan kelas baru dari kelas yang sudah ada. Kelas baru yang dihasilkan, disebut sebagai subclass, mewarisi seluruh atribut dan metode dari kelas yang menjadi induk atau superclass, kemudian dapat menambahkan atribut atau metode baru atau mengubah atribut atau metode yang telah diwarisi.

Berikut ini adalah contoh sederhana dari konsep specialization menggunakan bahasa pemrograman Python:

```python
class Kendaraan:
    def __init__(self, nama, jenis):
        self.nama = nama
        self.jenis = jenis

    def informasi(self):
        print(f"Nama kendaraan: {self.nama}")
        print(f"Jenis kendaraan: {self.jenis}")

class Mobil(Kendaraan):
    def __init__(self, nama, jenis, warna):
        super().__init__(nama, jenis)
        self.warna = warna

    def informasi(self):
        super().informasi()
        print(f"Warna kendaraan: {self.warna}")

mobil1 = Mobil("Avanza", "MPV", "Silver")
mobil1.informasi()
```

Dalam contoh tersebut, terdapat dua kelas yaitu `Kendaraan` dan `Mobil`. Kelas `Mobil` merupakan subclass dari kelas `Kendaraan`. Kelas `Mobil` mewarisi atribut dan metode dari kelas `Kendaraan`, yaitu `nama` dan `jenis`, serta metode `informasi()`. Selain itu, kelas `Mobil` menambahkan atribut baru yaitu `warna` dan mengubah metode `informasi()` dengan menambahkan informasi mengenai warna kendaraan.

Kemudian, kita membuat objek mobil1 dengan menggunakan kelas `Mobil`. Objek `mobil1` memiliki atribut `nama`, `jenis`, dan `warna` serta dapat memanggil metode `informasi()` yang telah diwarisi dari kelas `Kendaraan` dan diubah oleh kelas `Mobil`.

### Composition

Composition dalam OOP adalah ketika sebuah objek terdiri dari beberapa objek lainnya dan tidak dapat berfungsi secara independen. Contohnya adalah ketika sebuah mobil terdiri dari beberapa bagian seperti mesin, roda, pintu, jendela, dll. Ketika mobil dibuat, bagian-bagian ini dipasang bersama-sama dan membentuk sebuah entitas tunggal, mobil itu sendiri. Jika mobil dihancurkan, maka bagian-bagiannya juga akan hancur.

Berikut ini adalah contoh implementasi composition dalam Python:

```python
class Mesin:
    def __init__(self):
        self.kecepatan = 0
        self.status = "mati"

    def hidupkan(self):
        self.status = "hidup"

    def matikan(self):
        self.status = "mati"

class Mobil:
    def __init__(self):
        self.mesin = Mesin()
        self.roda = 4

    def hidupkan_mesin(self):
        self.mesin.hidupkan()

    def matikan_mesin(self):
        self.mesin.matikan()

    def cek_status_mesin(self):
        print("Status mesin:", self.mesin.status)

mobil = Mobil()
mobil.hidupkan_mesin()
mobil.cek_status_mesin()
```

Pada contoh di atas, terdapat kelas `Mesin` dan `Mobil`. Kelas `Mobil` memiliki objek `Mesin` dan properti `roda`. Ketika sebuah objek `Mobil` dibuat, sebuah objek `Mesin` juga dibuat dan disimpan di dalam objek `Mobil`. Kemudian, terdapat tiga metode di dalam kelas `Mobil`: `hidupkan_mesin()`, `matikan_mesin()`, dan `cek_status_mesin()`. Metode-metode ini memanipulasi objek `Mesin` yang terdapat di dalam objek `Mobil`.

### Aggregation

Aggregation adalah hubungan antara objek yang merupakan bagian dari objek lain, tetapi dapat eksis sendiri tanpa objek induknya. Contoh dari aggregation dalam Python adalah sebagai berikut:

```python
class Mahasiswa:
    def __init__(self, nama, nim):
        self.nama = nama
        self.nim = nim

class Dosen:
    def __init__(self, nama, nip, daftar_mahasiswa=None):
        self.nama = nama
        self.nip = nip
        self.daftar_mahasiswa = daftar_mahasiswa

mahasiswa1 = Mahasiswa("Asep", 1234)
mahasiswa2 = Mahasiswa("Budi", 5678)

daftar_mahasiswa = [mahasiswa1, mahasiswa2]

dosen1 = Dosen("Dr. Anton", 12345, daftar_mahasiswa)
```

Dalam contoh ini, terdapat dua kelas yaitu `Mahasiswa` dan `Dosen`. Kelas `Dosen` memiliki atribut `daftar_mahasiswa` yang merupakan daftar objek `Mahasiswa`. Objek-objek `Mahasiswa` ini bukanlah bagian dari objek `Dosen`, karena mereka dapat eksis sendiri dan tidak hanya terikat pada satu objek `Dosen`. Oleh karena itu, hubungan antara `Dosen` dan `Mahasiswa` ini merupakan contoh dari aggregation dalam OOP.

### Dependency

Dalam OOAD, dependency adalah hubungan antara dua kelas di mana satu kelas membutuhkan kelas lain untuk melakukan tugas tertentu. Salah satu contoh dari dependency dalam Python adalah sebagai berikut:

```python
class DatabaseConnector:
    def __init__(self):
        pass

    def connect(self):
        print("Connecting to the database...")

    def disconnect(self):
        print("Disconnecting from the database...")

class User:
    def __init__(self, name, database_connector):
        self.name = name
        self.database_connector = database_connector

    def get_user_info(self):
        self.database_connector.connect()
        print(f"Fetching user info from the database for user {self.name}...")
        self.database_connector.disconnect()
```

Dalam contoh di atas, kelas `User` bergantung pada kelas `DatabaseConnector` untuk terhubung ke database dan mengambil informasi pengguna. Kelas `User` memiliki objek `database_connector` sebagai salah satu argumen konstruktor, yang kemudian digunakan dalam metode `get_user_info()` untuk terhubung ke database. Ketergantungan ini menunjukkan adanya hubungan dependency antara kelas `User` dan `DatabaseConnector`.