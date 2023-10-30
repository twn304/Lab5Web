1. Buat file baru dengan nama lab_javascript.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
        document.write("Hello World");
        console.log("Hello World");
    </script>
</body>
</html>
```
Output 
![image](https://github.com/twn304/Lab5Web/assets/115573041/c4bfc0ba-be26-4d8a-ae72-03fa941b7edb)


2. Pemakaian Alert sebagai property window

```html 
<html>
    <head>
        <title>alert box</title>
    </head>
    <body>
        <script language = "java script">
            window.alert("ini merupakan pesan untuk anda");
        </script>
    </body>
</html>
```
Output 
![image-2](https://github.com/twn304/Lab5Web/assets/115573041/c6e9eefe-721c-4435-8a2f-a4409b4b10e7)


3. Pemakaian method dalam object

```html 
<html>
    <head>
        <title>skrip javascript</title>
    </head>
    <body>
        percobaan pemakaian javascript
        <script language = "javascript">
            document.write("selamat mencoba java<br>");
            document.write("semoga sukses!")
        </script>
    </body>
</html>
```
Output : 
![image-3](https://github.com/twn304/Lab5Web/assets/115573041/4fc9ca4f-52ac-4476-aa3c-f6a08a31ed4e)


4. Pemakaian Prompt
```html 
<html>
    <head>
        <title>pemasukan data</title>
    </head>
    <body>
        <script language = "javascript">
            var nama = prompt("siapa nama anda?","masukkan nama anda");
            document.write("hai, "+ nama);
        </script>
    </body>
</html>
```
Output :
![image-4](https://github.com/twn304/Lab5Web/assets/115573041/db5c72c5-bd8e-4054-b934-fc643ebd388b)



5. Pembuatan fungsi dan cara memanggilnya

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<title>contoh program javascript</title>
		<script language = "javascript">
			function pesan(){
			    alert ("memanggil javascript lewat body onload")
			}
		</script>
	</head>
	<body onload=pesan()>
	</body>
</html>
```
Output :

![image-5](https://github.com/twn304/Lab5Web/assets/115573041/0dcc6d8e-3c1e-4bad-9b63-8bc993899a20)


6. Operasi dasar aritmatika

```html
<head>
    <title>Mengenal JavaScript</title>
    <script>
        function test (val1,val2){
			document.write("<br>"+"perkalian : val1 * val2 "+"<br>")
			document.write(val1*val2)
			document.write("<br>"+"pembagian : val1 / val2 "+"<br>")
			document.write(val1/val2)
			document.write("<br>"+"penjumlahan : val1 + val2 "+"<br>")
			document.write(val1+val2)
			document.write("<br>"+"pengurangan : val1 - val2 "+"<br>")
			document.write(val1-val2)
			document.write("<br>"+"modulus : val1 % val2 "+"<br>")
			document.write(val1%val2)
		}
    </script>
</head>
<body>
    <input type="button" name="button1" value="arithmetic" onclick=test(9,4)>
</body>
</html>
```
Output : 
 
![image-6](https://github.com/twn304/Lab5Web/assets/115573041/076697c2-1efd-4d57-a05f-784ede681194)



7. Seleksi Kondisi if-else

```html
<script>
    var nilai = prompt("nilai (0-100): ",0);
	var hasil = "";
	if (nilai >= 60)
	hasil = "lulus";
	else
	hasil = "tidak lulus";
	document.write("hasil: " + hasil);  
</script>
```
![image-7](https://github.com/twn304/Lab5Web/assets/115573041/c06b32bb-914c-4f8e-86c4-3f9c0581e517)

8. Penggunaan Operator switch untuk seleksi kondisi

```html
<html>
    <head>
        <title>contoh program javascript</title>
        
        <script language="javascript">
            function test ()
            {
                val1=window.prompt("input nilai (1-5):")
                switch (val1)
                {
                case "1" :
                    document.write("bilangan satu")
                    break
                case "2" :
                    document.write("bilangan dua")
                    break
                case "3" :
                    document.write("bilangan tiga")
                    break
                case "4" :
                    document.write("bilangan empat")
                    break
                case "5" :
                    document.write("bilangan lima")
                    break
                default :
                    document.write("bilangan lainnya")
            }
        }
        </script>
    </head>
    <body>
        <h3>contoh program javascript</h3>
        <input type="button" name="button1" value="switch" onclick=test()>
    </body>
</html>
```
Output :

![image-8](https://github.com/twn304/Lab5Web/assets/115573041/df055f3d-d7a4-4554-b0dd-9868b9cb31ed)


9. Pembuatan Form
```html
<html>
    <head>
        <script language="javascript">
            function test () {
                var val1=document.kirim.T1.value
                if (val1%2==0)
                    document.kirim.T2.value="Bilangan Genap"
                else
                    document.kirim.T2.value="Bilangan Ganjil"
            }
        </script>
    </head>
    <body>
        <form method="POST" name="kirim">
            <p>BIL <input type="text" name="T1" size="20">
            MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
            <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
        </form>
    </body>
</html>
```
Output : 

![image-9](https://github.com/twn304/Lab5Web/assets/115573041/d13cf9e8-d631-42da-a5fa-b32018eb62d2)

![image-10](https://github.com/twn304/Lab5Web/assets/115573041/ed23d7ad-652e-4df1-9e7a-6049bdb311ba)

10. Form Button

```html
<html>
    <head>
        <title>objek document</title>
    </head>
    <body>
        <script language="javascript">
                function ubahWarnaLB(warna) {
                    document.bgColor = warna;
                }
                function ubahWarnaLD(warna) {
                    document.fgColor = warna;
                }
        </script>

        <h1>Hai</h1>
        <form>
            <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
            <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
            <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
            <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
        </form>
        <script language="javascript">
            document.write("Dimodifikasi terakhir pada " +
            document.lastModified);
        </script>
        
    </body>
</html>
```
Output :

![image-11](https://github.com/twn304/Lab5Web/assets/115573041/28733bb4-4610-44b0-9c34-e81728358b70)


11. HTML DOM 
```html
<!DOCTYPE html>
<html>
<head>
    <title>Datar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total');
            var harga = parseInt(ele.value);

            if (ele.checked) {
                total.value = parseInt(total.value) + harga;
            } else {
                total.value = parseInt(total.value) - harga;
            }
        }
    </script>
</head>
<body>
    <h1>Datar Menu makanan</h1>
    <label> <input type="checkbox" value="5000" id="menu1" onclick="hitung(this);"/> Ayam Goreng Rp.5000</label><br />
    <label> <input type="checkbox" value="2000" id="menu2" onclick="hitung(this);"/> Paku Rp.2000</label><br />
    <label> <input type="checkbox" value="21000" id="menu3" onclick="hitung(this);"/> Goreng Rp.21000</label><br />
    <strong>Total Bayar : Rp <input id="total" type="text" value="0" readonly></strong>
</body>
</html>
```
Output :

![image-12](https://github.com/twn304/Lab5Web/assets/115573041/90611095-8b27-445b-9a6f-5c2ef18f55a9)
