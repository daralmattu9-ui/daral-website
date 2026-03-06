daral-website
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>DARAL Luxury Clothing</title>
<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@600&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

<style>

body{margin:0;background:black;color:white;font-family:'Poppins',sans-serif;}

header{background:black;border-bottom:1px solid gold;padding:15px 20px;position:sticky;top:0;z-index:1000}

nav{display:flex;justify-content:space-between;align-items:center}

.logo{font-family:'Cinzel',serif;font-size:30px;color:gold;letter-spacing:3px;animation:shine 3s infinite}

@keyframes shine{
0%{text-shadow:0 0 5px gold}
50%{text-shadow:0 0 20px silver,0 0 30px gold}
100%{text-shadow:0 0 5px gold}
}

.menu a{color:white;text-decoration:none;margin:0 10px;font-size:14px}
.menu a:hover{color:gold}

.search{padding:6px;border-radius:4px;border:none}

.hero{text-align:center;padding:80px 20px;background:linear-gradient(black,#111)}
.hero h1{font-family:'Cinzel',serif;font-size:48px;color:gold}
.hero p{color:silver}

.section{padding:50px 20px;text-align:center}
.section h2{font-family:'Cinzel',serif;color:gold;margin-bottom:30px}

.products{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:25px;max-width:1100px;margin:auto}

.product{background:#111;padding:15px;border:1px solid #333;border-radius:8px}
.product img{width:100%;border-radius:6px}
.product h3{margin:10px 0}
.price{color:gold;margin-bottom:10px}

.btn{display:inline-block;padding:10px 18px;background:gold;color:black;text-decoration:none;font-weight:600;border-radius:4px;margin:5px}
.btn:hover{background:silver}

.category{margin-bottom:40px}

.reviews{max-width:800px;margin:auto;text-align:left}
.review{background:#111;padding:15px;margin-bottom:15px;border-radius:6px;border:1px solid #333}

footer{margin-top:40px;padding:30px;text-align:center;border-top:1px solid #333;color:silver}

</style>

<script>
function searchProducts(){
let input=document.getElementById('search').value.toLowerCase();
let items=document.getElementsByClassName('product');
for(let i=0;i<items.length;i++){
let text=items[i].innerText.toLowerCase();
items[i].style.display=text.includes(input)?'block':'none';
}
}
</script>

</head>
<body>

<header>
<nav>
<div class="logo">DARAL</div>
<div class="menu">
<a href="#home">Home</a>
<a href="#men">Men</a>
<a href="#women">Women</a>
<a href="#premium">Premium</a>
<a href="#order">Order</a>
</div>
<input id="search" class="search" placeholder="Search" onkeyup="searchProducts()">
</nav>
</header>

<section class="hero" id="home">
<h1>DARAL Luxury Fashion</h1>
<p>Black • Gold • Silver Streetwear</p>
<a class="btn" href="#premium">Premium Clothes</a>
</section>

<section class="section category" id="men">
<h2>Men Collection</h2>
<div class="products">

<div class="product">
<select style="margin-top:10px;padding:6px;border-radius:4px;border:none;background:#222;color:white">
<option>Select Size</option>
<option>S</option>
<option>M</option>
<option>L</option>
<option>XL</option>
</select>
<img src="https://images.unsplash.com/photo-1521572163474-6864f9cf17ab">
<h3>Classic T-Shirt</h3>
<div class="price">₹499</div>
<a class="btn" href="https://wa.me/917527998135">Order</a>
</div>

<div class="product">
<select style="margin-top:10px;padding:6px;border-radius:4px;border:none;background:#222;color:white">
<option>Select Size</option>
<option>S</option>
<option>M</option>
<option>L</option>
<option>XL</option>
</select>
<img src="https://images.unsplash.com/photo-1556906781-9a412961c28c">
<h3>Street Hoodie</h3>
<div class="price">₹999</div>
<a class="btn" href="https://wa.me/917527998135">Order</a>
</div>

</div>
</section>

<section class="section category" id="women">
<h2>Women Collection</h2>
<div class="products">

<div class="product">
<select style="margin-top:10px;padding:6px;border-radius:4px;border:none;background:#222;color:white">
<option>Select Size</option>
<option>S</option>
<option>M</option>
<option>L</option>
<option>XL</option>
</select>
<img src="https://images.unsplash.com/photo-1495121605193-b116b5b09a14">
<h3>Stylish Jacket</h3>
<div class="price">₹1499</div>
<a class="btn" href="https://wa.me/917527998135">Order</a>
</div>

<div class="product">
<select style="margin-top:10px;padding:6px;border-radius:4px;border:none;background:#222;color:white">
<option>Select Size</option>
<option>S</option>
<option>M</option>
<option>L</option>
<option>XL</option>
</select>
<img src="https://images.unsplash.com/photo-1523381294911-8d3cead13475">
<h3>Designer Hoodie</h3>
<div class="price">₹1299</div>
<a class="btn" href="https://wa.me/917527998135">Order</a>
</div>

</div>
</section>

<section class="section" id="premium">
<h2>Premium Collection</h2>
<div class="products">

<div class="product">
<select style="margin-top:10px;padding:6px;border-radius:4px;border:none;background:#222;color:white">
<option>Select Size</option>
<option>S</option>
<option>M</option>
<option>L</option>
<option>XL</option>
</select>
<img src="https://images.unsplash.com/photo-1503342217505-b0a15ec3261c">
<h3>Premium Streetwear</h3>
<div class="price">₹2499</div>
<a class="btn" href="https://wa.me/917527998135">Order</a>
</div>

</div>
</section>

<section class="section" id="order">
<h2>Order & Payment</h2>
<p>Order on WhatsApp or pay using UPI.</p>
<a class="btn" href="https://wa.me/917527998135">Order on WhatsApp</a>
<p style="margin-top:20px;color:silver">UPI Payment Example: yourupi@bank</p>
</section>

<section class="section">
<h2>Customer Reviews</h2>
<div class="reviews">

<div class="review">
⭐️⭐️⭐️⭐️⭐️<br>
Amazing quality hoodie. Very stylish.
</div>

<div class="review">
⭐️⭐️⭐️⭐️⭐️<br>
Best streetwear brand. Fast delivery.
</div>

</div>
</section>

<section class="section" id="orderform">
<h2>Order Form</h2>
<p>Fill the form and send order on WhatsApp.</p>
<form onsubmit="sendOrder();return false;" style="max-width:500px;margin:auto;text-align:left">
<input id="name" placeholder="Your Name" required style="width:100%;padding:10px;margin:6px 0;border:none;border-radius:4px">
<input id="phone" placeholder="Phone Number" required style="width:100%;padding:10px;margin:6px 0;border:none;border-radius:4px">
<input id="address" placeholder="Delivery Address" required style="width:100%;padding:10px;margin:6px 0;border:none;border-radius:4px">
<select id="size" style="width:100%;padding:10px;margin:6px 0;border:none;border-radius:4px">
<option>S</option><option>M</option><option>L</option><option>XL</option>
</select>
<button class="btn" type="submit">Send Order</button>
</form>
</section>

<section class="section" id="tracking">
<h2>Delivery Tracking</h2>
<p style="color:silver">Enter your order phone number to check delivery status.</p>
<input placeholder="Phone Number" style="padding:10px;border:none;border-radius:4px">
<p style="margin-top:15px;color:silver">Status: Processing / Shipped / Delivered</p>
</section>

<script>
function sendOrder(){
let name=document.getElementById('name').value;
let phone=document.getElementById('phone').value;
let address=document.getElementById('address').value;
let size=document.getElementById('size').value;
let msg=`Order from DARAL:%0AName: ${name}%0APhone: ${phone}%0AAddress: ${address}%0ASize: ${size}`;
window.open(`https://wa.me/917527998135?text=${msg}`,'_blank');
}
</script>

<footer>
© 2026 DARAL Clothing Brand
</footer>

</body>
</html>
