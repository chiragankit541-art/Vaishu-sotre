# Vaishu-sotre
body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    background: #111;
    color: white;
    text-align: center;
}

header {
    padding: 20px;
    background: #222;
    border-bottom: 2px solid #444;
}

h1 {
    font-size: 26px;
}

.product-section {
    margin-top: 25px;
}

.product-img {
    width: 90%;
    max-width: 360px;
    border-radius: 12px;
    box-shadow: 0 0 10px #000;
}

.price {
    font-size: 28px;
    margin-top: 15px;
    font-weight: bold;
}

.buy-btn {
    background: #00ff88;
    padding: 12px 25px;
    font-size: 20px;
    border: none;
    border-radius: 10px;
    margin-top: 15px;
    cursor: pointer;
}

.buy-btn:hover {
    background: #00cc6a;
}

.upi-box {
    background: #222;
    margin: 35px 20px;
    padding: 20px;
    border-radius: 12px;
}

.upi-id {
    background: #333;
    padding: 12px;
    margin-top: 10px;
    border-radius: 8px;
    font-size: 18px;
}

.copy-btn {
    margin-top: 10px;
    padding: 10px 20px;
    background: #ffaa00;
    border: none;
    border-radius: 10px;
    font-size: 18px;
    cursor: pointer;
}

.copy-btn:hover {
    background: #dd8800;
}<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Vaishu Modern Clothing Store</title>
    <link rel="stylesheet" href="style.css" />
</head>

<body>

    <header>
        <h1>Vaishu Modern Clothing Store</h1>
        <p>Trendy • Stylish • Affordable</p>
    </header>

    <section class="product-section">
        <img src="https://ibb.co/RGgTWQRf" alt="Product" class="product-img"/>

        <h2 class="price">₹499 Only</h2>

        <button class="buy-btn" onclick="pay()">Buy Now</button>
    </section>

    <section class="upi-box">
        <h3>Pay Using UPI</h3>

        <div class="upi-id">
            <p>7828131477@ibl</p>
        </div>

        <button class="copy-btn" onclick="copyUPI()">Copy UPI ID</button>
    </section>

    <script>
        function copyUPI() {
            navigator.clipboard.writeText("7828131477@ibl");
            alert("UPI ID Copied!");
        }

        function pay() {
            window.location.href = "upi://pay?pa=7828131477@ibl&pn=VaishuStore&am=499&cu=INR";
        }
    </script>

</body>
</html>https://i.ibb.co/tLWFKtS/vaishu-store-model.jpg
