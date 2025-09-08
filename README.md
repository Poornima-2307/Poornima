<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Login | TrendyKart</title>
  <link rel="stylesheet" href="style.css">
</head>
<body class="login-page">
  <div class="login-wrapper">
    <h2>TrendyKart Login</h2>
    <form action="products.html" method="get" class="login-form">
      <input type="text" placeholder="Username" required>
      <input type="password" placeholder="Password" required>
      <button type="submit">Login</button>
      <p>New here? <a href="#">Create Account</a></p>
    </form>
  </div>
</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Products | TrendyKart</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header class="main-header">
    <h1>🛒 TrendyKart</h1>
    <nav>
      <a href="login.html">Logout</a>
    </nav>
  </header>

  <section class="product-list">
    <div class="product-item">
      <img src="https://via.placeholder.com/200x200" alt="Product 1">
      <h3>Stylish Sneakers</h3>
      <p>$49.99</p>
      <button>Add to Cart</button>
    </div>

    <div class="product-item">
      <img src="https://via.placeholder.com/200x200" alt="Product 2">
      <h3>Denim Jacket</h3>
      <p>$59.99</p>
      <button>Add to Cart</button>
    </div>

    <div class="product-item">
      <img src="https://via.placeholder.com/200x200" alt="Product 3">
      <h3>Smart Watch</h3>
      <p>$89.99</p>
      <button>Add to Cart</button>
    </div>

    <div class="product-item">
      <img src="https://via.placeholder.com/200x200" alt="Product 4">
      <h3>Leather Wallet</h3>
      <p>$19.99</p>
      <button>Add to Cart</button>
    </div>
  </section>
</body>
</html>/* Reset and base */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: #f5f5f5;
}

/* === LOGIN PAGE === */
.login-page {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(to right, #4facfe, #00f2fe);
}

.login-wrapper {
  background: #fff;
  padding: 40px;
  border-radius: 10px;
  width: 300px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  text-align: center;
}

.login-wrapper h2 {
  margin-bottom: 20px;
  color: #333;
}

.login-form input {
  width: 100%;
  padding: 12px;
  margin: 10px 0;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.login-form button {
  width: 100%;
  padding: 12px;
  background-color: #1abc9c;
  color: white;
  border: none;
  border-radius: 5px;
  font-weight: bold;
  cursor: pointer;
  margin-top: 10px;
}

.login-form button:hover {
  background-color: #16a085;
}

.login-form p {
  margin-top: 15px;
  font-size: 14px;
}

.login-form a {
  color: #3498db;
  text-decoration: none;
}

/* === PRODUCT PAGE === */
.main-header {
  background-color: #34495e;
  color: white;
  padding: 15px 30px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.main-header nav a {
  color: white;
  text-decoration: none;
  font-weight: bold;
  background: #2c3e50;
  padding: 8px 12px;
  border-radius: 4px;
}

.main-header nav a:hover {
  background: #1abc9c;
}

.product-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
  padding: 30px;
}

.product-item {
  background: white;
  padding: 20px;
  text-align: center;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  transition: transform 0.2s;
}

.product-item:hover {
  transform: translateY(-5px);
}

.product-item img {
  width: 100%;
  border-radius: 8px;
  margin-bottom: 10px;
}

.product-item h3 {
  margin: 10px 0;
  color: #333;
}

.product-item p {
  font-weight: bold;
  color: #27ae60;
}

.product-item button {
  padding: 10px 15px;
  background-color: #e74c3c;
  color: white;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

.product-item button:hover {
  background-color: #c0392b;
}

/* Responsive tweaks */
@media (max-width: 600px) {
  .login-wrapper {
    width: 90%;
  }

  .main-header h1 {
    font-size: 20px;
  }

  .product-list {
    grid-template-columns: 1fr;
  }
}