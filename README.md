# vickspares254
the best spare parts shop
<!DOCTYPE html>
<html>
<head>
    <title>Victor Auto & Tech Spares</title>
    <link rel="stylesheet" href="style.css">
    <script defer src="script.js"></script>
</head>
<body>

<header>
    <h1>Victor Auto & Tech Spares</h1>
    <nav>
        <a href="index.html">Home</a>
        <a href="komatsu.html">Komatsu Parts</a>
        <a href="contact.html">Contact</a>
    </nav>
</header>

<section class="hero">
    <h2>Heavy Machinery & Tech Spare Parts</h2>
    <p>Genuine & Aftermarket Parts Available</p>
</section>

<section class="search-section">
    <input type="text" id="searchInput" placeholder="Search parts (e.g. PC200-7)">
</section>

<section id="productList" class="products">

    <div class="product">
        <h3>Komatsu Oil Filter</h3>
        <p>Model: PC200-7</p>
        <p class="genuine">Genuine - KES 4,500</p>
        <p class="stock">In Stock</p>
        <a href="https://wa.me/2547XXXXXXXX?text=I%20want%20Genuine%20Komatsu%20Oil%20Filter%20PC200-7">
            <button>Order</button>
        </a>
    </div>

    <div class="product">
        <h3>Komatsu Oil Filter</h3>
        <p>Model: PC200-7</p>
        <p class="aftermarket">Aftermarket - KES 2,800</p>
        <p class="stock">In Stock</p>
        <a href="https://wa.me/2547XXXXXXXX?text=I%20want%20Aftermarket%20Komatsu%20Oil%20Filter%20PC200-7">
            <button>Order</button>
        </a>
    </div>

    <div class="product">
        <h3>Komatsu Air Cleaner</h3>
        <p>Model: PC300</p>
        <p class="genuine">Genuine - KES 6,800</p>
        <p class="stock">Limited Stock</p>
        <a href="https://wa.me/2547XXXXXXXX?text=I%20want%20Komatsu%20Air%20Cleaner%20PC300">
            <button>Order</button>
        </a>
    </div>

    <div class="product">
        <h3>Komatsu Piston Rings</h3>
        <p>Model: PC200-7</p>
        <p class="aftermarket">Aftermarket - KES 12,000</p>
        <p class="stock">In Stock</p>
        <a href="https://wa.me/2547XXXXXXXX?text=I%20want%20Komatsu%20Piston%20Rings%20PC200-7">
            <button>Order</button>
        </a>
    </div>

</section>

</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    background: #f4f4f4;
}

header {
    background: #111;
    color: white;
    padding: 15px;
    text-align: center;
}

nav a {
    color: white;
    margin: 10px;
    text-decoration: none;
}

nav a:hover {
    color: yellow;
}

.hero {
    text-align: center;
    padding: 30px;
    background: #222;
    color: white;
}

.search-section {
    text-align: center;
    padding: 20px;
}

#searchInput {
    padding: 10px;
    width: 60%;
    max-width: 400px;
}

.products {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

.product {
    background: white;
    margin: 15px;
    padding: 20px;
    width: 250px;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
}

.product button {
    background: green;
    color: white;
    padding: 10px;
    border: none;
    cursor: pointer;
    width: 100%;
}

.product button:hover {
    background: darkgreen;
}

.genuine {
    color: blue;
    font-weight: bold;
}

.aftermarket {
    color: orange;
    font-weight: bold;
}

.stock {
    color: green;
    font-weight: bold;
}
document.getElementById("searchInput").addEventListener("keyup", function() {
    let filter = this.value.toLowerCase();
    let products = document.querySelectorAll(".product");

    products.forEach(function(product) {
        let text = product.textContent.toLowerCase();
        if (text.includes(filter)) {
            product.style.display = "";
        } else {
            product.style.display = "none";
        }
    });
});
<!DOCTYPE html>
<html>
<head>
    <title>Contact - Victor Auto & Tech Spares</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1>Contact Us</h1>
</header>

<section style="text-align:center; padding:20px;">
    <p><b>Location:</b> Nairobi, Kenya</p>
    <p><b>Phone:</b> +254723451982</p>
    <p><b>M-Pesa Till:</b> 123456</p>

    <iframe 
        src="https://www.google.com/maps?q=Nairobi&output=embed"
        width="400" 
        height="300">
    </iframe>
</section>

</body>
</html>
