# Writing Test Week 2 Front-end Bootcamp

<center> Topik Materi : ReactJS Lanjutan</center>

<br/>
<br/>

## **Proptypes**

- Inputan data adalah hal / aspek penting untuk menentukan proses selanjutnya dari keseuaian data yang akan diberikan oleh user 

- Dalam Reactjs ada yang namanya Proptypes, digunakan untuk membantu mengecek dan menentukan tipe data yang akan digunakan dalam suatu kondisi. 

### Cara Menggunakan Proptypes 

- Pertama install proptypes menggunakan terminal ataupun command prompt npm `install prop-types`

- Selanjutnya import prop-types kedalam react dengan cara `import PropTypes form 'prop-types'`. Code ini dituliskan didalam component yang menerima props 

- Setelah itu, kita bisa menentukan tipe data yang diinginkan

- Didalam proptypes terdapat beberapa element untuk menyesuaikan tipe data berdasarkan dari yang diinginkan 

    - **Any** , digunakan saat data yang diinput bebas, jadi bisa berupa number dan string ataupun yang laiinya 
    - **isRequired** , digunakan saat user **HARUS** melakukan input data dan **TIDAK** boleh kosong 
    - **oneOfType** , digunakan disaat kita ingin memberikan opsi pilihan tipe data pada props, jadi data dapat berupa number atau string. jika tipe data yang dimasukan tidak termasuk kedalam ketentuan maka code akan menjalankan error.

### Proptypes pada Array

- Proptypes juga dapat digunakan untuk data bertipe array.
- Kita dapat memberikan code `data:PropTypes.array` untuk mengecek inputan value yang berupa array.
- Lalu proptypes pada array juga dapat diberikan berbagai tipe data didalamnya. 

### Proptypes pada Object

- _.shape_ digunakan untuk mengecek dan mengatur isian dari tipe data object. 
- _.exact_ digunakan untuk melihat key dan value dari object agar sesuai dengan ketentuan yang adam jika menggunakan .exact maka inputan yang diberikan harus sesuai dengan yang ditentukan.


<br>
<br>

## **Router**

- Router digunakan untuk berpindah halaman didalam react
   
- Router perlu diinstal terlebih dahulu sebelum dapat digunakan
  
- setelah itu import kedalam file main/index.js
  
- Didalam main file, bungkus app menggunakan browserrouter
  
> Beberapa element router memiliki sifat yang sama seperti tag HTML


- react mengunakan tag link untuk mengarah ke halaman lain
- route path dan link to = a href 
- dengan router halaman utama hanya dituliskan dengan / 
- lalu dalam router ada *params* digunakan untuk mengirim data kehalaman lain 
- Alternatif lain dari *params* adalah useNavigation, digunakan untuk berpindah dan dapat mengirim data juga 


<BR>
<br>


## **State Managment (REDUX)**

- Adanya redux menghindarkan kita untuk melakukan *props drilling* yaitu disaat component props diberikan atau dioper ke element child secara berlebihan.

- Konsep dari State management sendiri adalah dimana komponent yang akan digunakan berulang hanya diberikan ke child yang membutuhkan 


    1. Intall redux 
    2. set-up store `createstore` 
    3. membuat reducer - initial state 
    4. memanggil reducer ke store
    5. membuat provider - react-redux ( digunakan agar dapat diketahui bahwa store tersedia untuk komponent yang ada )
    6. ambil state menggunakan useSelector

- Action, adalah function yang memiliki object 
- useDispatch, digunakan untuk mengirim action kedalam reducer 









