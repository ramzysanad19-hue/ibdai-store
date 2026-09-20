<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>إبداعى | هدايا ومنتجات مميزة</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Tahoma, Arial, sans-serif;
      background: #faf7f2;
      color: #302821;
      line-height: 1.7;
    }

    header {
      background: white;
      padding: 18px 7%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 10;
      box-shadow: 0 2px 15px rgba(0,0,0,.08);
    }

    .logo {
      font-size: 30px;
      font-weight: bold;
      text-decoration: none;
      color: #302821;
    }

    nav {
      display: flex;
      gap: 20px;
      align-items: center;
    }

    nav a {
      text-decoration: none;
      color: #302821;
    }

    .cart {
      background: #302821;
      color: white;
      padding: 9px 16px;
      border-radius: 10px;
    }

    .hero {
      min-height: 520px;
      padding: 80px 10%;
      display: flex;
      align-items: center;
      background: linear-gradient(120deg, #eee0ce, #fffaf3);
    }

    .hero h1 {
      font-size: 58px;
      line-height: 1.15;
      margin: 15px 0;
    }

    .hero p {
      font-size: 20px;
      max-width: 600px;
      margin-bottom: 25px;
    }

    .btn {
      display: inline-block;
      background: #302821;
      color: white;
      border: none;
      padding: 13px 25px;
      border-radius: 10px;
      cursor: pointer;
      text-decoration: none;
      font-size: 16px;
    }

    section {
      padding: 65px 7%;
    }

    section h2 {
      text-align: center;
      font-size: 32px;
      margin-bottom: 35px;
    }

    .categories {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }

    .category {
      background: white;
      padding: 35px 15px;
      text-align: center;
      border-radius: 16px;
      box-shadow: 0 5px 20px rgba(0,0,0,.06);
      font-size: 24px;
    }

    .category span {
      display: block;
      font-size: 45px;
      margin-bottom: 10px;
    }

    .products {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 22px;
    }

    .product {
      background: white;
      padding: 16px;
      border-radius: 16px;
      box-shadow: 0 5px 20px rgba(0,0,0,.06);
    }

    .product-image {
      height: 210px;
      border-radius: 12px;
      background: #eee4d7;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 65px;
      margin-bottom: 15px;
    }

    .product h3 {
      min-height: 55px;
      font-size: 18px;
    }

    .price {
      font-weight: bold;
      font-size: 19px;
      margin: 10px 0;
    }

    .product button {
      width: 100%;
    }

    .about {
      text-align: center;
      background: white;
    }

    .about p {
      max-width: 750px;
      margin: auto;
    }

    footer {
      background: #302821;
      color: white;
      text-align: center;
      padding: 30px;
    }

    @media(max-width:900px) {
      .products,
      .categories {
        grid-template-columns: repeat(2, 1fr);
      }

      .hero h1 {
        font-size: 45px;
      }
    }

    @media(max-width:550px) {
      nav a:not(.cart) {
        display: none;
      }

      .products,
      .categories {
        grid-template-columns: 1fr;
      }

      .hero {
        padding: 60px 7%;
      }

      .hero h1 {
        font-size: 40px;
      }
    }
  </style>
</head>

<body>

<header>
  <a href="#" class="logo">إبداعى</a>

  <nav>
    <a href="#">الرئيسية</a>
    <a href="#categories">الأقسام</a>
    <a href="#products">المنتجات</a>
    <a href="#about">من نحن</a>
    <a href="#contact">تواصل معنا</a>
    <a href="#cart" class="cart">
      🛒 السلة <span id="cartCount">0</span>
    </a>
  </nav>
</header>

<section class="hero">
  <div>
    <strong>هدايا صنعت بحب ❤️</strong>

    <h1>
      لمسة إبداعية<br>
      لكل مناسبة
    </h1>

    <p>
      اكتشف أجمل صناديق الزان والخزف والصدف
      والمنتجات اليدوية المميزة من إبداعى.
    </p>

    <a href="#products" class="btn">
      تسوق الآن
    </a>
  </div>
</section>

<section id="categories">
  <h2>تسوق حسب القسم</h2>

  <div class="categories">

    <div class="category">
      <span>🎁</span>
      الهدايا
    </div>

    <div class="category">
      <span>🪵</span>
      المنتجات الخشبية
    </div>

    <div class="category">
      <span>🏺</span>
      الخزف والصدف
    </div>

    <div class="category">
      <span>🏠</span>
      الديكور والمنزل
    </div>

  </div>
</section>

<section id="products">

  <h2>منتجات مميزة</h2>

  <div class="products">

    <div class="product">
      <div class="product-image">🪵✨</div>

      <h3>
        صندوق زان مزين بالخزف والصدف
      </h3>

      <div class="price">
        4,250 ج.م
      </div>

      <button class="btn" onclick="addToCart()">
        أضف للسلة
      </button>
    </div>


    <div class="product">
      <div class="product-image">💍</div>

      <h3>
        علبة مجوهرات خشبية فاخرة
      </h3>

      <div class="price">
        3,250 ج.م
      </div>

      <button class="btn" onclick="addToCart()">
        أضف للسلة
      </button>
    </div>


    <div class="product">
      <div class="product-image">🎁</div>

      <h3>
        صندوق هدايا زان — إصدار محدود
      </h3>

      <div class="price">
        5,500 ج.م
      </div>

      <button class="btn" onclick="addToCart()">
        أضف للسلة
      </button>
    </div>


    <div class="product">
      <div class="product-image">🏺</div>

      <h3>
        قطعة ديكور خزف وصدف
      </h3>

      <div class="price">
        2,750 ج.م
      </div>

      <button class="btn" onclick="addToCart()">
        أضف للسلة
      </button>
    </div>

  </div>
</section>

<section class="about" id="about">

  <h2>عن إبداعى</h2>

  <p>
    إبداعى متجر متخصص في الهدايا والمنتجات اليدوية
    ذات الطابع المميز، ونقدم قطعًا تجمع بين الخشب
    والخزف والصدف والتصميم الأنيق.
  </p>

</section>

<footer id="contact">

  <p>© 2026 إبداعى — جميع الحقوق محفوظة</p>

  <p>📞 تواصل معنا قريبًا</p>

</footer>

<script>

let cartCount = 0;

function addToCart() {

  cartCount++;

  document.getElementById("cartCount").innerText = cartCount;

  alert("تمت إضافة المنتج إلى السلة 🛒");

}

</script>

</body>
</html>
