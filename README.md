<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>POINT STORE - Top Up FF</title>

<style>
body{
    font-family:Arial,sans-serif;
    background:#111827;
    color:white;
    margin:0;
}

header{
    background:linear-gradient(45deg,#0099ff,#003cff);
    text-align:center;
    padding:20px;
}

.logo{
    width:120px;
    height:120px;
    border-radius:50%;
    object-fit:cover;
    border:3px solid white;
}

.container{
    max-width:800px;
    margin:auto;
    padding:20px;
}

.card{
    background:#1f2937;
    padding:20px;
    border-radius:12px;
    margin-bottom:20px;
}

input,select{
    width:100%;
    padding:12px;
    margin-top:10px;
    border:none;
    border-radius:8px;
}

.btn{
    display:block;
    width:100%;
    padding:15px;
    margin-top:15px;
    background:#25D366;
    color:white;
    text-decoration:none;
    border:none;
    border-radius:10px;
    font-size:18px;
    font-weight:bold;
    cursor:pointer;
}

.price{
    background:#374151;
    padding:12px;
    border-radius:8px;
    margin-top:10px;
    text-align:center;
}
</style>
</head>
<body>

<header>
    <h1>💎 POINT STORE</h1>
    <p>Top Up Diamond Free Fire Murah & Aman</p>
</header>

<div class="container">

<div class="card">
<h2>Form Order</h2>

<input type="text" id="idff" placeholder="Masukkan ID Free Fire">

<select id="diamond">
<option>5 Diamond - Rp1.000</option>
<option>70 Diamond - Rp10.000</option>
<option>140 Diamond - Rp20.000</option>
<option>355 Diamond - Rp50.000</option>
<option>720 Diamond - Rp100.000</option>
</select>

<button class="btn" onclick="pesanWA()">
Pesan Via WhatsApp
</button>

</div>

<div class="card">
<h2>Daftar Harga</h2>

<div class="price">5 Diamond - Rp1.000</div>
<div class="price">70 Diamond - Rp10.000</div>
<div class="price">140 Diamond - Rp20.000</div>
<div class="price">355 Diamond - Rp50.000</div>
<div class="price">720 Diamond - Rp100.000</div>

</div>

</div>

<script>
function pesanWA(){

var id = document.getElementById("idff").value;
var dm = document.getElementById("diamond").value;

var nomor = "6282374179856";

var pesan =
"Halo POINT STORE\n\n" +
"Saya ingin top up FF\n\n" +
"ID FF : " + id + "\n" +
"Paket : " + dm;

window.location.href =
"https://api.whatsapp.com/send?phone=" +
nomor +
"&text=" +
encodeURIComponent(pesan);

}
</script>
<div class="card">
<h2>📞 Contact Admin</h2>

<p><b>WhatsApp:</b> 082374179856</p>
<p><b>Email:</b> alnopurba10@gmail.com</p>

<a href="https://wa.me/6282374179856" class="btn">
Chat Admin WhatsApp
</a>

</div>

</body>
</html>
</body>
</html>
