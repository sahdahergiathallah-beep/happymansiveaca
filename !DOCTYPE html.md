<!DOCTYPE html>  
<html lang="id">  
<head>  
  <meta charset="UTF-8">  
  <title>For Aca 🤍</title>  
</head>  
  
<body style="  
  background: linear-gradient(135deg, #ff9a9e, #fad0c4);  
  height: 100vh;  
  margin: 0;  
  display: flex;  
  justify-content: center;  
  align-items: center;  
  font-family: Arial, sans-serif;  
  text-align: center;  
">  
  
  <div style="padding:20px; max-width:360px;">  
    <h1 id="title">Happy 3 Months, Aca 🤍</h1>  
  
    <p id="text" style="font-size:17px;">  
      Tiga bulan ini bukan tentang lamanya waktu,    
      tapi tentang kamu yang selalu berhasil    
      bikin aku betah.  
    </p>  
  
    <br>  
  
    <button id="btn" onclick="nextStep()" style="  
      font-size:18px;  
      padding:12px 26px;  
      border:none;  
      border-radius:30px;  
      background:#ff4d6d;  
      color:white;  
      cursor:pointer;  
    ">  
      Play & Continue 🤍  
    </button>  
  </div>  
  
  <!-- Musik -->  
  <audio id="music">  
    <source src="https://dl.sndup.net/d6wq/Mangu.mp3" type="audio/mpeg">  
  </audio>  
  
  <script>  
    let step = 0;  
  
    function nextStep() {  
      const text = document.getElementById("text");  
      const title = document.getElementById("title");  
      const btn = document.getElementById("btn");  
      const music = document.getElementById("music");  
  
      if (step === 0) {  
        music.play();  
        title.innerHTML = "Kenapa aku milih kamu 🤍";  
        text.innerHTML =  
          "Karena kamu datang di saat aku nggak lagi nyari siapa-siapa, tapi malah bikin aku takut kehilangan.";  
        btn.innerHTML = "Lanjut 🤍";  
        step++;  
      }   
      else if (step === 1) {  
        text.innerHTML =  
          "Kamu bukan yang paling sempurna, ca. Tapi kamu yang paling aku usahain.";  
        step++;  
      }   
      else if (step === 2) {  
        text.innerHTML =  
          "Aku suka caramu bertahan, caramu peduli, dan caramu tetap ada walau capek.";  
        step++;  
      }   
      else if (step === 3) {  
        title.innerHTML = "Untuk Aca 🤍";  
        text.innerHTML =  
          "Aku nggak tau kita bakal sejauh apa, tapi selama kamu masih mau di sini, aku nggak akan pergi.";  
        btn.innerHTML = "Terakhir 🤍";  
        step++;  
      }   
      else {  
        title.innerHTML = "Aku sayang kamu, Aca 🤍";  
        text.innerHTML =  
          "Terima kasih sudah jadi bagian dari hidup aku. Happy 3 months, and many more months to come 🤍";  
        btn.style.display = "none";  
      }  
    }  
  </script>  
  
</body>  
</html>  
