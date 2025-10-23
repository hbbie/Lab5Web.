# Lab5Web.
PerogramanWEB Pertemuan 6

Nama    : Dhani Naufal Habibie

Kelas   : TI.24.A4

NIM     : 312410300

1.Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut:

<img width="444" height="201" alt="image" src="https://github.com/user-attachments/assets/5514235d-d9c2-4bd4-8166-e07f3453c6e4" />

[Uploading Screenshot 2025-10-23 133041.png…]()

2. Pemakaian Alert sebagai property window.

<img width="1913" height="1069" alt="image" src="https://github.com/user-attachments/assets/9f55e8b4-b5b4-4424-bbdd-c4394568d412" />

3.Pemakaian method dalam objek

<img width="1919" height="1012" alt="image" src="https://github.com/user-attachments/assets/b5e50477-e268-4db5-9aa8-f18070d8ea09" />

4.Pemakaian Prompt

<img width="1919" height="1077" alt="image" src="https://github.com/user-attachments/assets/06e6ff3c-832c-4219-9065-38eadc9cd2b9" />

<img width="796" height="452" alt="image" src="https://github.com/user-attachments/assets/4826cfe0-779f-4630-b2e5-0d54791869bc" />

5.Pembuatan fungsi dan cara pemanggilannya

<img width="1916" height="931" alt="Screenshot 2025-10-23 135731" src="https://github.com/user-attachments/assets/2e651c14-6de5-4a6e-93a6-8c87e9c76019" />

6.Dasar Pemrograman Di Javascript
Operasi dasar aritmatika

<img width="158" height="253" alt="image" src="https://github.com/user-attachments/assets/23432558-a89b-4e76-a9d2-811d4ce0e420" />


<img width="332" height="274" alt="image" src="https://github.com/user-attachments/assets/635cf2bc-854b-45c9-91e3-cff6a34d768d" />

7.Seleksi kondisi (if..else)


<img width="1903" height="1014" alt="image" src="https://github.com/user-attachments/assets/2a50ec47-ec2d-41a9-8ac8-a98e6197df97" />

 Masukan angka yang anda inginkan >60 lulus dan sebaliknya :89 maka hasilnya lulus
 
<img width="412" height="182" alt="image" src="https://github.com/user-attachments/assets/02fc31ae-95e7-4d9e-ade4-56531e625883" />

8.Penggunaan operator switch untuk seleksi kondisi


<img width="1061" height="406" alt="image" src="https://github.com/user-attachments/assets/0dd6ce0c-0587-4b55-8a28-eac02f56a7a0" />

masukaan angka yang anda inginkan (1-5) : contoh 3


<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/e8e0f5f0-9dd3-45b6-9ba4-f9f3c3108349" />

apabila lebih dari : 6 sampai seterusnya


<img width="494" height="340" alt="image" src="https://github.com/user-attachments/assets/071a0ac7-164e-45ce-a0b1-f72a81fcae3e" />

9.Pembuatan Form
Form Input


<img width="550" height="252" alt="image" src="https://github.com/user-attachments/assets/69917021-fd89-44a6-a338-4a0691e2655c" />

apabila angka 1 (ganjil) akan terisi otomatis : bilangan ganjil

apabila angka 2 (genap) akan terisi otomatis : bilangan genap

10.Form Button


<img width="1354" height="582" alt="image" src="https://github.com/user-attachments/assets/f82241e0-0eec-45f7-a8dc-6b8459c31b3b" />

dia akan berubah sesuai tombol yang diinginkan

11.HTML DOM
Pilihan menggunakan checkBox dengan perhitungan otomatis

<img width="672" height="371" alt="image" src="https://github.com/user-attachments/assets/4f1a60ef-010e-4fb3-bb15-f06cc38885d1" />

ketika kamu milih menu dia akan otomatis tertotal harganya sendiri

# Soal Dan Pertanyaan

<img width="521" height="83" alt="image" src="https://github.com/user-attachments/assets/43ca820b-5e9e-46f9-818d-06b5e47b662b" />

Kode Program :
```html
<!DOCTYPE html>
<html>
<head>
<title>Validasi Form</title>
<script>
function validasiForm() {
    var nama = document.forms["formData"]["nama"].value;
    var email = document.forms["formData"]["email"].value;
    var umur = document.forms["formData"]["umur"].value;

    // Validasi nama tidak boleh kosong
    if (nama == "") {
        alert("Nama tidak boleh kosong!");
        return false;
    }

    // Validasi email dengan pola sederhana
    var polaEmail = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    if (!polaEmail.test(email)) {
        alert("Format email tidak valid!");
        return false;
    }

    // Validasi umur harus angka dan minimal 17 tahun
    if (isNaN(umur) || umur < 17) {
        alert("Umur harus berupa angka dan minimal 17 tahun!");
        return false;
    }

    alert("Form berhasil dikirim!");
    return true;
}
</script>
</head>

<body>
<h2>Formulir Pendaftaran</h2>
<form name="formData" onsubmit="return validasiForm()">
    Nama: <input type="text" name="nama"><br><br>
    Email: <input type="text" name="email"><br><br>
    Umur: <input type="text" name="umur"><br><br>
    <input type="submit" value="Kirim">
</form>
</body>
</html>
```
Hasilnya :

<img width="1061" height="372" alt="image" src="https://github.com/user-attachments/assets/cac7739c-5d82-4eba-8e85-32cce9145584" />

harus diisi seperti, contoh jika benar :

<img width="1917" height="894" alt="image" src="https://github.com/user-attachments/assets/e8598cc1-b6a4-427f-b677-d24ff1900bc8" />

document.forms["formData"]["nama"].value mengambil nilai input.

alert() menampilkan pesan kesalahan jika ada isian yang tidak valid.

return false mencegah form dikirim jika validasi gagal.

return true hanya dijalankan jika semua isian valid.













