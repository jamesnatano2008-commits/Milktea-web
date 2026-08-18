
<!DOCTYPE html>
<html>

<head>
    <title>Miltea shop</title>

    <!-- External CSS -->
    <link rel="stylesheet" href="style.css">

    <!-- Internal CSS -->
    <style>



        body {
        background-color: #3B240B;  
        margin: 0;
    }
        p{
            font-size:18px;
            text-align:center;
            color:white;
        }

        h2{
            color:white;
            text-align:center;
        }



         /* ===== NAVIGATION BAR ===== */
        .navbar {
            background-color:blue;
            padding: 15px 30px;
            text-align: center;
        }

        .navbar a {
            color: blue;
            text-decoration: none;
            margin: 0 15px;
            font-size: 17px;
            padding: 8px 12px;
        }

        .navbar a:hover {
            color:blue;
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <nav>
        <a href="index.html">Home</a>
        <a href="products.html">Products</a>
        <a href="Gallery.html">Gallery</a>
        <a href="contacts.html">Contact</a>
        <a href="aboutus.html">About Us</a>
    </nav>

    <!-- Inline CSS -->
    <h1 style="color:White; text-align:center;">
        Enjoy At Lasapin Ang Sarap ng Milk tea
    </h1>

 <div class="slider">

    <div class="slides fade">
        <img src="images/jim.png">
    </div>

    <div class="slides fade">
        <img src="images/etis2.png">
    </div>

    <div class="slides fade">
        <img src="images/etis3.png">
    </div>

    <!-- Previous -->
    <a class="prev" onclick="plusSlides(-1)">&#10094;</a>

    <!-- Next -->
    <a class="next" onclick="plusSlides(1)">&#10095;</a>

</div>

<!-- Dots -->
<div class="dots">

    <span class="dot" onclick="currentSlide(1)"></span>

    <span class="dot" onclick="currentSlide(2)"></span>

    <span class="dot" onclick="currentSlide(3)"></span>

</div>

<script src="script.js"></script>

    <h2>Welcome!</h2>

    <p>
        Welcome to our Milktea Shop! Thank you for visiting  we serve fresh, creamy, and high-quality milktea made with love. Sit back, relax, and enjoy your favorite drink! ✨
    </p>

    <p>
        We are so glad you're here. Come and taste our best-selling milktea  crafted with premium ingredients and served fresh just for you! 💚
    </p>

</body>

</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Milktea Shop</title>
    <link rel="stylesheet" href="style.css">
    <style>
     {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #98FB98;  /* Dark Blue Header */
            color: white;
            padding: 30px;
        }

/* ===== NAVIGATION BAR ===== */
        .navbar {
            background-color: white; /* Dark brown Header */
            padding: 15px 30px;
            text-align: center;
        }

        .navbar a {
            color: #0B1742;
            text-decoration: none;
            margin: 0 15px;
            font-size: 17px;
            padding: 8px 12px;
        }

        .navbar a:hover {
            color: #0B1742;
        }

 

        /* ===== HEADER ===== */
        .header-bar {
            background-color: #0B1742; /* Dark Blue Header */
            text-align: center;
            padding: 18px;
            border-radius: 12px;
            font-size: 28px;
            font-weight: bold;
            margin: 30px;
            letter-spacing: 1px;
        }

        .header-bar {
            background-color: #0B1742; /* Dark Blue Header */
            text-align: center;
            padding: 18px;
            border-radius: 12px;
            font-size: 28px;
            font-weight: bold;
            margin-bottom: 30px;
            letter-spacing: 1px;
        }

        .container {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .product-card {
            background-color: #0B1742; /* Dark Blue Boxes */
            border-radius: 12px;
            padding: 20px;
            text-align: center;
            transition: 0.3s;
        }

        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0,0,0,0.35);
        }

        .product-img {
            width: 100%;
            height: 200px;
            background-color: #1A2C70; /* Lighter Dark Blue for image area */
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            margin-bottom: 18px;
        }

        .product-name {
            font-size: 17px;
            margin-bottom: 8px;
            font-weight: 500;
        }

        .product-price {
            font-size: 16px;
            opacity: 0.9;
            margin-bottom: 15px;
        }

        .add-btn {
            background-color: #1A2C70; /* Slightly lighter blue button */
            color: white;
            border: none;
            padding: 10px 22px;
            border-radius: 20px;
            font-size: 14px;
            cursor: pointer;
            transition: 0.2s;
        }

        .add-btn:hover {
            background-color: #283EA8;
        }

        /* Cart Panel — top right */
        .cart-panel {
            position: absolute;
            top: 30px;
            right: 30px;
            background-color: #0B1742; /* Dark Blue Cart Box */
            color: white;
            padding: 18px;
            border-radius: 10px;
            width: 200px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.35);
        }

        .cart-title {
            font-size: 18px;
            font-weight: bold;
            margin-bottom: 12px;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        .cart-badge {
            background-color: #3B240B; /* Match dark brown theme */
            color: white;
            font-size: 12px;
            border-radius: 50%;
            width: 22px;
            height: 22px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .cart-empty {
            font-size: 14px;
            color: #ddd;
            margin-bottom: 10px;
        }

        .cart-total {
            border-top: 1px solid #4455AA;
            padding-top: 8px;
            margin-bottom: 12px;
            font-weight: 500;
        }

        .purchase-btn {
            width: 100%;
            background-color: #1A2C70;
            color: white;
            border: none;
            padding: 9px;
            border-radius: 6px;
            cursor: pointer;
            font-weight: 500;
        }

        .purchase-btn:hover {
            background-color: #283EA8;
        }

        /* Responsive */
        @media(max-width:992px) {
            .container { grid-template-columns: repeat(2,1fr); }
        }
        @media(max-width:600px) {
            .container { grid-template-columns: 1fr; }
            .cart-panel { position: static; width: 100%; margin-bottom: 20px; }
        } 



        body {
            background-color: #3B240B;
            margin: 0;
            padding: 20px;
            font-family: 'Segoe UI', sans-serif;
        }
        .video-section {
            background-color: #0B1742;
            color: white;
            text-align: center;
            padding: 30px;
            border-radius: 12px;
            max-width: 800px;
            object-fit: cover; /* Keep image nice & cropped evenly */
            margin: 30px auto;

        }
        .video-section h2 {
            margin-bottom: 20px;
            font-size: 24px;
        }
        .video-section video {
            width: 100%;
            border-radius: 10px;
        }
    </style>
</head>

    <body>

   <!-- ✅ NAVIGATION BAR -->
    <div class="navbar">
         <a href="index.html">Home</a>
        <a href="products.html">Products</a>
        <a href="Gallery.html">Gallery</a>
        <a href="contacts.html">Contact</a>
        <a href="aboutus.html">About Us</a>
    </div>


    <!-- Cart Panel -->
    <div class="cart-panel">
        <div class="cart-title">🛒 Cart <span class="cart-badge">0</span></div>
        <p class="cart-empty">Your cart is empty.</p>
        <p class="cart-total">Total: ₱0</p>
        <button class="purchase-btn">Purchase Now</button>
    </div>

    <!-- Header -->
    <div class="header-bar">🧋 Milktea Favorites Menu</div>

    <!-- Products Grid -->
    <div class="container">
        <!-- Product 1 -->
        <div class="product-card">
            <img src="images/1786432199368.png" height="200" width="200"> 
            <h3 class="product-name">Salted Caramel Milk Tea</h3>
            <p class="product-price">₱190</p>
            <button class="add-btn">Add to Cart</button>
        </div>

        <!-- Product 2 -->
        <div class="product-card">
            <img src="images/1786432207374.png" height="200px" width="200px">
            <h3 class="product-name">Taro Milk Tea</h3>
            <p class="product-price">₱180</p>
            <button class="add-btn">Add to Cart</button>
        </div>

        <!-- Product 3 -->
        <div class="product-card">
            <img src="images/1786432212090.png" height="200" width="200">
            <h3 class="product-name">Matcha Green Milk Tea</h3>
            <p class="product-price">₱150</p>
            <button class="add-btn">Add to Cart</button>
        </div>

        <!-- Product 4 -->
        <div class="product-card">
            <img src="images/1786432230623.png" height="200" width="200">
            <h3 class="product-name">Ube Halaya Milk Tea</h3>
            <p class="product-price">₱175</p>
            <button class="add-btn">Add to Cart</button>
        </div>

        <!-- Product 5 -->
        <div class="product-card">
           <img src="images/1786432225675.png" height="200" width="200">
            <h3 class="product-name">Mango Milk Tea</h3>
            <p class="product-price">₱165</p>
            <button class="add-btn">Add to Cart</button>
        </div>

        <!-- Product 6 -->
        <div class="product-card">
            <img src="images/1786432221042.png" height="200" width="200">
            <h3 class="product-name">Oreo Chocolate Milk Tea</h3>
            <p class="product-price">₱200</p>
            <button class="add-btn">Add to Cart</button>
         </div>

        <!-- Product 7 -->
            <div class="product-card">
            <img src="images/1786432234925.png" height="200" width="200">
            <h3 class="product-name">Classic Assam Black Milk Tea</h3>
            <p class="product-price">₱200</p>
            <button class="add-btn">Add to Cart</button>
        </div>

      <!-- Product 8 -->
            <div class="product-card">
            <img src="images/1786432238896.png" height="200" width="200">
            <h3 class="product-name">Lychee Rose Milk Tea</h3>
            <p class="product-price">₱200</p>
            <button class="add-btn">Add to Cart</button>
         </div>


        <!-- Product 9 -->
            <div class="product-card">
            <img src="images/1786432216523.png" height="200" width="200">
            <h3 class="product-name">Strawberry Milk Tea</h3>
            <p class="product-price">₱200</p>
            <button class="add-btn">Add to Cart</button>
        </div>
    </div>

</body>

</html>




<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Products - Milktea Shop</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Times New Roman', serif;
        }

        body {
            background-color: #442A16; /* Dark brown background */
            padding: 0;
            margin: 0;
        }

        /* ========== WHITE NAVIGATION BAR ========== */
        .navbar {
            background-color: #FFFFFF;
            text-align: center;
            padding: 12px 0;
            margin: 0;
        }

        .navbar a {
            color: #442A16;
            text-decoration: none;
            font-size: 17px;
            margin: 0 22px;
            padding: 8px 12px;
        }

        .navbar a:hover {
            text-decoration: underline;
        }

        /* ========== PAGE HEADER ========== */
        .page-header {
            background-color: #0A1A47; /* Dark navy blue */
            color: #FFFFFF;
            font-size: 26px;
            font-weight: bold;
            text-align: center;
            padding: 15px;
            margin: 20px auto;
            width: 80%;
            border-radius: 10px;
        }

        /* ========== PRODUCTS GRID ========== */
        .products-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
            max-width: 1200px;
            margin: 30px auto;
            padding: 0 20px;
        }

        /* ========== PRODUCT CARD — ONLY IMAGE + NAME ========== */
        .product-card {
            background-color: #0A1A47;
            border-radius: 12px;
            padding: 25px 20px;
            text-align: center;
            color: #FFFFFF;
        }

        .product-img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 15px;
        }

        .product-name {
            font-size: 17px;
            color: #FFFFFF;
            line-height: 1.5;
        }

        /* ========== RESPONSIVE ========== */
        @media (max-width: 900px) {
            .products-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }
        @media (max-width: 550px) {
            .products-grid {
                grid-template-columns: 1fr;
            }
            .page-header { width: 90%; }
        }
    </style>
</head>
<body>

    <!-- ========== WHITE NAVIGATION BAR ========== -->
    <div class="navbar">
        <a href="index.html">Home</a>
        <a href="products.html">Products</a>
        <a href="Gallery.html">Gallery</a>
        <a href="contacts.html">Contact</a>
        <a href="aboutus.html">About Us</a>
    </div>

    <!-- PAGE HEADER -->
    <div class="page-header">
        🥤 Milktea Favorites Menu
    </div>

    <!-- PRODUCTS — ONLY PICTURE + NAME -->
    <div class="products-grid">

        <!-- PRODUCT 1 -->
        <div class="product-card">
            <img src="images/1.jpg"  class="product-img">
            <h3 class="product-name">Freshly made with love every drink prepared carefully just for you</h3>
        </div>

        <!-- PRODUCT 2 -->
        <div class="product-card">
            <img src="images/images2.jpg"  class="product-img">
            <h3 class="product-name">Meet our friendly team  always happy to serve you with a smile!</h3>
        </div>

        <!-- PRODUCT 3 -->
        <div class="product-card">
            <img src="images/image3.jpg"  class="product-img">
            <h3 class="product-name">Handcrafted step-by-step  making your milktea perfect, one sip at a time!</h3>
        </div>

        <!-- PRODUCT 4 -->
        <div class="product-card">
            <img src="images/images4.jpg"  class="product-img">
            <h3 class="product-name"> Our kitchen  clean, organized, and ready to brew your favorites!</h3>
        </div>

        <!-- PRODUCT 5 -->
        <div class="product-card">
            <img src="images/images5.jpg"  class="product-img">
            <h3 class="product-name">Proudly serving happiness in every cup! </h3>
        </div>

        <!-- PRODUCT 6 -->
        <div class="product-card">
            <img src="images/images6.jpg"  class="product-img">
            <h3 class="product-name"> Welcome to our shop  where great taste meets warm vibes!</h3>
        </div> 


        <!-- PRODUCT 7 -->
        <div class="product-card">
            <img src="images/images7.jpg"  class="product-img">
            <h3 class="product-name"> Only the freshest and finest ingredients go into every drink!</h3>
        </div>


        <!-- PRODUCT 8 -->
        <div class="product-card">
            <img src="images/images8.jpg"  class="product-img">
            <h3 class="product-name"> Care, passion, and quality in every single cup!</h3>
        </div>

        <!-- PRODUCT 9 -->
        <div class="product-card">
            <img src="images/images.jpg" alt="Oreo Chocolate Milk Tea" class="product-img">
            <h3 class="product-name">Oreo Chocolate Milk Tea</h3>
        </div>



        
    </div>
    <style>
        body {
            background-color: #3B240B;
            margin: 0;
            padding: 20px;
            font-family: 'Segoe UI', sans-serif;
        }
        .video-section {
            background-color: #0B1742;
            color: white;
            text-align: center;
            padding: 30px;
            border-radius: 12px;
            max-width: 800px;
            object-fit: cover; /* Keep image nice & cropped evenly */
            margin: 30px auto;

        }
        .video-section h2 {
            margin-bottom: 20px;
            font-size: 24px;
        }
        .video-section video {
            width: 100%;
            border-radius: 10px;
        }
    </style>


    <div class="video-section">
        <h2>🎥 Watch Our Video</h2>

        <!-- 👇 Ito ang PINAKAMAHALAGANG BAHAGI -->
        <video src="video/Download.mp4"  controls width="420" height="420">
                    </video>
    </div>

</body>
</html>


