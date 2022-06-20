# RECURSIVE

- Recursive ini merupakan function yang memanggil dirinya sendiri sampai kondisi tertentu.
- Recursive digunakan untuk pemecahan masalah yg besar agar menjadi masalah kecil.
  > contohnya : yang berhubungan dengan calculation seperti case matematika, fisika atau kimia.
  ```js
  //mencari hasil dari nilai pangkat
  function pow(x, n) {
    if (n == 1) {
      return x;
    } else {
      return x * pow(x, n - 1);
    }
  }
  console.log(pow(4, 3));
  ```
- Ciri Recursive
  1. selalu memiliki kondisi yang menghentikan function dari memanggil dirinya sendiri.
  2. selalu memanggil dirinya sendiri sambil memecahkan data masukan setiap panggilannya.

# WEB STORAGE

- **Web Storage** : menyimpan data secara sementara di luar dari variabel.
  > Data pengguna seperti : pencarian, artikel, berita, cll.
- Macam - macam web storage :

  1. Cookies
  2. Local storage
  3. Session storage
     :one: **COOKIES**

  - Data kecil yang dikirim dari situs web dan disimpan di komputer.
  - Data dalam cookies :
    - acces login pengguna.
    - history pencarian situs web :arrow_right: melacak pencarian untuk menampilkan iklan yang berhubungan.
  - Kekurangan Cookies

    - cookies dikirim berulang saat mengakses situs.
    - mengirimkan data yang tidak dienkripsi.
    - hanya dapat menyimpan data max 4KB.
    - memiliki tanggal kadaluarsa.

    :two: **LOCAL STORAGE**

  - Karakteristik Local Storage :
    - menyimpan data tanpa tanggal kadaluarsa.
    - data terus tersimpan selama tidak dihapus pada web browser.
    - menyimpan data hingga 5MB.
    - hanya menyimpan data string.
  - **setItem()** : method untuk menyimpan data pada local storage.
    - menggunakan 2 parameter : key & value
      ```js
      localStorage.setItem("key", value);
      ```
  - **JSON.stringify()** : merubah array menjadi string.
  - **JSON.parse()** : merubah string menjadi array.
  - Cara **mengambil** data local storage
    ```js
    localStorage.getItem("key");
    ```
  - Cara **menghapus** data local storage

    ```js
    // menghapus key tertentu
    localStorage.removeItem("key");

    // menghapus semua key
    localStorage.clear();
    ```

  - Cara melihat data yang tersimpan dalam local storage browser kita :

    - klik kanan pada web
    - pilih inspect
    - klik **_Application_**
    - klik **_Local Storage_** di sisi tab sebelah kiri.

    :three: **SESSION STORAGE**

  - Karakteristik Session Storage :
    - data terus tersimpan selama browser terbuka.
    - menciptakan session storage berbeda meskipun URL sama.
    - data terhapus saat tab/window di tutup.
    - data harus berbentuk string.
    - menyimpan data max 5MB.
  - Contoh kegunaannya :
    - menyimpan data keranjang belanja situs e-commerce.
  - Sintaks = local storage
    ```js
    sessionStorage.setItem("key", value);
    ```
  -

# RESPONSIVE WEB DESIGN

- RWD ini merupakan styling layout sebuah web agar dapat menyesuaikan dengan ukuran device pengguna sehingga tampilan tetap bagus dan rapi.
  > Device : Smartphone, Tablet, Laptop, PC.
- Tools RWD pada browser chrome : Chrome Dev Tools. cara menggunakannya :
  > 1. klik kanan pada web.
  > 2. klik inspect dibagian paling akhir.
  > 3. klik toggle device pada bagian atas.
  >    ![Tools RWD](./assets/tools%20rwd.png)
  >    > Untuk cara lebih simple :wink: gunakan keyword :point_down:
  >    > **ctrl + shift + J**
- Untuk memudahkan menggunakan RWD itu pakai : **_Media query_**
  - :speech*balloon: Jenis \*\*\_media query*\*\* : min-width dan max-width
    ```css
    @media only screen and (max-width: 1200px) {
    }
    ```
    ```css
    @media only screen and (min-width: 600px) {
    }
    ```
- :anger: **_Breakpoint_** : perubahan yang terjadi pada tampilan saat berganti width (device).
- :anger: **_Complex Breakpoint_** : media query untuk tampilan device pada ukuran range tertentu.
  ```css
  @media only screen and (min-width: 480px) and (max-width: 720px) {
  }
  ```

# BOOTSTRAP

- **_Bootstrap_** :
  - salah satu CSS Framework.
  - hasil formula codingan website yang telah siap digunakan.
  - programmer tidak perlu menghabiskan banyak waktu dan tenaga untuk membuat formula CSS website baru dari awal.
  - Cara penggunaan bootstrap :
    1.  buka website Bootstrap
    2.  klik bagian 'Read the docs'
    3.  Pada bagian introduction Get Started with bootstrap, copy code nomer 2. Include Bootstrap's CSS and JS.
    4.  Paste code include bootstrap tersebut pada file html pada sebuah folder di VS Code.
    5.  masukan code bootstrap yg diinginkan dibagian tag <body>. code component bisa di search pada web bootstrap nya itu sendiri.
