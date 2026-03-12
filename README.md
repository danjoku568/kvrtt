<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>kvrtt online shopping</title></title>

<style>
body{
font-family: Arial;
margin:0;
background:#f4f4f4;
}

header{
background:#222;
color:white;
padding:15px;
display:flex;
justify-content:space-between;
}

.products{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
gap:20px;
padding:20px;
}

.product{
background:white;
padding:15px;
border-radius:10px;
text-align:center;
box-shadow:0 2px 5px rgba(0,0,0,0.2);
}

button{
background:#28a745;
color:white;
border:none;
padding:10px 15px;
cursor:pointer;
border-radius:5px;
}

button:hover{
background:#218838;
}

img{
width:100%;
border-radius:8px;
}
</style>
</head>

<body>

<header>
<h2>My Online Shop</h2>
<div>Cart 🛒: <span id="cart">0</span></div>
</header>

<section class="products">

<div class="product">
<img src="https://via.placeholder.com/200">
<h3>Shoes</h3>
<p>$40</p>
<button onclick="addToCart()">Add to Cart</button>
</div>

<div class="product">
<img src="https://via.placeholder.com/200">
<h3>Smart Watch</h3>
<p>$60</p>
<button onclick="addToCart()">Add to Cart</button>
</div>

<div class="product">
<img src="https://via.placeholder.com/200">
<h3>Headphones</h3>
<p>$25</p>
<button onclick="addToCart()">Add to Cart</button>
</div>

<div class="product">
<img src="https://via.placeholder.com/200">
<h3>Backpack</h3>
<p>$35</p>
<button onclick="addToCart()">Add to Cart</button>
</div>

</section>

<script>

let cart = 0;

function addToCart(){
cart++;
document.getElementById("cart").innerText = cart;
}

</script>

</body>
</html>

