<!DOCTYPE html>
<html>
<head>
<title>swetha's Online Book Store</title>

<style>
body{
    font-family: Arial;
    text-align: center;
}

.book{
    border:1px solid black;
    padding:10px;
    margin:10px;
    width:200px;
    display:inline-block;
}

button{
    background-color:green;
    color:white;
    padding:5px;
}
</style>

<script>
let cart = 0;

function addBook(book){
    cart++;
    alert(book + " added to cart");
    document.getElementById("cart").innerHTML = cart;
}
</script>

</head>

<body>

<h1>Swetha's Online Book Store</h1>

<h3>Cart Items: <span id="cart">0</span></h3>

<div class="book">
<h3>JavaScript Book</h3>
<p>Price: ₹500</p>
<button onclick="addBook('JavaScript Book')">Add to Cart</button>
</div>

<div class="book">
<h3>HTML Book</h3>
<p>Price: ₹300</p>
<button onclick="addBook('HTML Book')">Add to Cart</button>
</div>

<div class="book">
<h3>CSS Book</h3>
<p>Price: ₹350</p>
<button onclick="addBook('CSS Book')">Add to Cart</button>
</div>

</body>
</html>
