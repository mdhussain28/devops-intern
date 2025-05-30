# DevOps CI/CD Pipeline with GitHub Actions, Docker, Kubernetes, and Argo CD

This project demonstrates a complete CI/CD pipeline setup using **GitHub Actions** for CI and **Argo CD** for CD. It builds a Docker image from the application source code, pushes it to a container registry, and deploys the image to a Kubernetes cluster using Argo CD.

---

## 🚀 Workflow Overview

### Continuous Integration (CI) - GitHub Actions
- Triggers on every push to the `main` branch (or a specific branch).
- Builds the Docker image.
- Pushes the image to Docker Hub (or any specified container registry).
- Updates the Kubernetes manifest (optional).

### Continuous Deployment (CD) - Argo CD
- Watches the Git repository for changes in Kubernetes manifests.
- Automatically syncs the changes and deploys to the Kubernetes cluster.

---

## 🔧 Technologies Used

- **GitHub Actions** - for CI workflows
- **Docker** - to containerize the application
- **Docker Hub** - as a container image registry
- **Kubernetes** - to run the application pods
- **Argo CD** - for GitOps-based continuous delivery

---

# index.html file 
## v1 Blue
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BlueCommerce - Online Shopping</title>
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #e3f2fd; /* Pale blue */
        }

        header {
            background-color: white;
            padding: 20px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #007bff; /* Blue */
            text-decoration: none;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 20px;
            align-items: center;
        }

        .nav-links a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
        }

        .hero {
            background-color: #f8f9fa;
            text-align: center;
            padding: 100px 20px;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            color: #212529;
        }

        .hero p {
            color: #666;
            margin-bottom: 30px;
        }

        .cta-button {
            background-color: #007bff; /* Blue */
            color: white;
            padding: 15px 30px;
            border-radius: 5px;
            text-decoration: none;
            display: inline-block;
        }

        .products {
            max-width: 1200px;
            margin: 50px auto;
            padding: 0 20px;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }

        .product-card {
            background-color: white;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            text-align: center;
        }

        .product-image {
            background-color: #eee;
            height: 200px;
            border-radius: 5px;
            margin-bottom: 15px;
        }

        .product-card button {
            background-color: #007bff; /* Blue */
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 5px;
            cursor: pointer;
        }

        footer {
            background-color: #f8f9fa;
            text-align: center;
            padding: 30px 20px;
            margin-top: 50px;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="/" class="logo">BlueCommerce</a>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#shop">Shop</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <h1>Welcome to BlueCommerce</h1>
            <p>Discover amazing products at great prices</p>
            <a href="#shop" class="cta-button">Shop Now</a>
        </section>

        <section class="products">
            <h2>Featured Products</h2>
            <div class="product-grid">
                <div class="product-card">
                    <div class="product-image"></div>
                    <h3>Product 1</h3>
                    <p>$99.99</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <div class="product-image"></div>
                    <h3>Product 2</h3>
                    <p>$149.99</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <div class="product-image"></div>
                    <h3>Product 3</h3>
                    <p>$79.99</p>
                    <button>Add to Cart</button>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2023 BlueCommerce. All rights reserved.</p>
    </footer>
</body>
</html>

```
## v2 Green
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GreenCommerce - Online Shopping</title>
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #e3f2fd; /* Pale blue */
        }

        header {
            background-color: white;
            padding: 20px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #28a745; /* Green */
            text-decoration: none;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 20px;
            align-items: center;
        }

        .nav-links a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
        }

        .cart-icon {
            font-size: 20px;
            color: #28a745; /* Green */
            cursor: pointer;
        }

        .hero {
            background-color: #f8f9fa;
            text-align: center;
            padding: 100px 20px;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            color: #212529;
        }

        .hero p {
            color: #666;
            margin-bottom: 30px;
        }

        .cta-button {
            background-color: #28a745; /* Green */
            color: white;
            padding: 15px 30px;
            border-radius: 5px;
            text-decoration: none;
            display: inline-block;
        }

        .products {
            max-width: 1200px;
            margin: 50px auto;
            padding: 0 20px;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }

        .product-card {
            background-color: white;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            text-align: center;
        }

        .product-image {
            background-color: #eee;
            height: 200px;
            border-radius: 5px;
            margin-bottom: 15px;
        }

        .product-card button {
            background-color: #28a745; /* Green */
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 5px;
            cursor: pointer;
        }

        footer {
            background-color: #f8f9fa;
            text-align: center;
            padding: 30px 20px;
            margin-top: 50px;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="/" class="logo">GreenCommerce</a>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#shop">Shop</a></li>
                <li><a href="#cart"><i class="fas fa-shopping-cart cart-icon"></i> Cart</a></li> <!-- Cart added here -->
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <h1>Welcome to GreenCommerce</h1>
            <p>Discover amazing products at great prices</p>
            <a href="#shop" class="cta-button">Shop Now</a>
        </section>

        <section class="products">
            <h2>Featured Products</h2>
            <div class="product-grid">
                <div class="product-card">
                    <div class="product-image"></div>
                    <h3>Product 1</h3>
                    <p>$99.99</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <div class="product-image"></div>
                    <h3>Product 2</h3>
                    <p>$149.99</p>
                    <button>Add to Cart</button>
                </div>
                <div class="product-card">
                    <div class="product-image"></div>
                    <h3>Product 3</h3>
                    <p>$79.99</p>
                    <button>Add to Cart</button>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2023 GreenCommerce. All rights reserved.</p>
    </footer>
</body>
</html>
```
