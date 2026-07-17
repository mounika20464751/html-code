<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bus Booking</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
height:100vh;
display:flex;
justify-content:center;
align-items:center;
background:linear-gradient(135deg,#3b82f6,#06b6d4,#22c55e);
overflow:hidden;
}

body::before{
content:'';
position:absolute;
width:400px;
height:400px;
background:rgba(255,255,255,.15);
border-radius:50%;
top:-120px;
left:-120px;
filter:blur(30px);
}

body::after{
content:'';
position:absolute;
width:350px;
height:350px;
background:rgba(255,255,255,.15);
border-radius:50%;
bottom:-120px;
right:-120px;
filter:blur(30px);
}

.container{
width:900px;
background:rgba(255,255,255,.18);
backdrop-filter:blur(15px);
padding:35px;
border-radius:25px;
box-shadow:0 20px 50px rgba(0,0,0,.2);
z-index:1;
}

.title{
text-align:center;
font-size:34px;
font-weight:700;
color:#fff;
margin-bottom:8px;
}

.subtitle{
text-align:center;
color:#eef;
margin-bottom:30px;
}

.form{
display:grid;
grid-template-columns:repeat(2,1fr);
gap:20px;
}

.input-box{
display:flex;
flex-direction:column;
}

label{
margin-bottom:8px;
font-weight:500;
color:white;
}

input,select{
padding:14px;
border:none;
outline:none;
border-radius:12px;
font-size:15px;
background:white;
transition:.3s;
}

input:focus,
select:focus{
transform:scale(1.02);
box-shadow:0 0 15px rgba(255,255,255,.6);
}

.search-btn{
grid-column:span 2;
padding:16px;
border:none;
border-radius:15px;
background:#ff6b00;
color:white;
font-size:18px;
font-weight:600;
cursor:pointer;
transition:.3s;
}

.search-btn:hover{
background:#ff4500;
transform:translateY(-3px);
box-shadow:0 10px 25px rgba(255,107,0,.4);
}

.features{
display:flex;
justify-content:space-between;
margin-top:35px;
}

.card{
flex:1;
margin:0 10px;
background:white;
border-radius:18px;
padding:22px;
text-align:center;
transition:.3s;
}

.card:hover{
transform:translateY(-8px);
box-shadow:0 15px 30px rgba(0,0,0,.15);
}

.card h2{
font-size:40px;
}

.card h3{
margin-top:10px;
color:#333;
}

.card p{
margin-top:8px;
color:#666;
font-size:14px;
}

@media(max-width:850px){

.container{
width:95%;
}

.form{
grid-template-columns:1fr;
}

.search-btn{
grid-column:span 1;
}

.features{
flex-direction:column;
}

.card{
margin:10px 0;
}

}

</style>

</head>

<body>

<div class="container">

<div class="title">🚌 Bus Booking</div>
<div class="subtitle">Find & Book Your Comfortable Journey</div>

<div class="form">

<div class="input-box">
<label>From</label>
<input type="text" placeholder="Enter Source City">
</div>

<div class="input-box">
<label>To</label>
<input type="text" placeholder="Enter Destination City">
</div>

<div class="input-box">
<label>Journey Date</label>
<input type="date">
</div>

<div class="input-box">
<label>Passengers</label>
<select>
<option>1 Passenger</option>
<option>2 Passengers</option>
<option>3 Passengers</option>
<option>4 Passengers</option>
<option>5+ Passengers</option>
</select>
</div>

<button class="search-btn">
🔍 Search Buses
</button>

</div>

<div class="features">

<div class="card">
<h2>🛡️</h2>
<h3>Safe Travel</h3>
<p>Verified buses with experienced drivers.</p>
</div>

<div class="card">
<h2>💺</h2>
<h3>Seat Selection</h3>
<p>Choose your favorite window or sleeper seat.</p>
</div>

<div class="card">
<h2>💳</h2>
<h3>Secure Payment</h3>
<p>Fast and secure online payment options.</p>
</div>

</div>

</div>

</body>
</html>
