<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TechGame Store - Peças & Jogos</title>
    <style>
        :root {
            --primary-color: #6A1B9A;
            --secondary-color: #212121;
            --accent-color: #9C27B0;
            --text-color: #FFFFFF;
        }

        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--secondary-color);
            color: var(--text-color);
        }

        .header {
            background: linear-gradient(to right, var(--primary-color), var(--accent-color));
            padding: 1rem;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0,0,0,0.3);
        }

        .nav {
            display: flex;
            justify-content: center;
            gap: 2rem;
            padding: 1rem;
        }

        .nav a {
            color: var(--text-color);
            text-decoration: none;
            font-weight: 500;
            transition: 0.3s;
        }

        .nav a:hover {
            color: #FFD700;
        }

        .main-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .product-card {
            background: rgba(255,255,255,0.05);
            border-radius: 10px;
            padding: 1rem;
            transition: transform 0.3s;
        }

        .product-card:hover {
            transform: translateY(-5px);
        }

        .promo-section {
            border: 2px solid var(--primary-color);
            border-radius: 10px;
            padding: 1rem;
            margin: 2rem 0;
        }

        .coupon-code {
            background: rgba(255,255,255,0.1);
            padding: 0.5rem;
            border-radius: 5px;
            margin: 0.5rem 0;
        }

        .retailer-logos {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 1rem;
            padding: 2rem 0;
        }

        .retailer-logo {
            width: 120px;
            filter: grayscale(100%);
            transition: 0.3s;
        }

        .retailer-logo:hover {
            filter: grayscale(0%);
        }

        @media (max-width: 768px) {
            .nav {
                flex-direction: column;
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <header class="header">
        <h1>TechGame Store</h1>
        <nav class="nav">
            <a href="#pecas">Peças PC</a>
            <a href="#games">Video Games</a>
            <a href="#promo">Promoções</a>
            <a href="#cupons">Cupons</a>
        </nav>
    </header>

    <main class="main-container">
        <section id="promo">
            <h2>Promoções em Destaque</h2>
            <div class="promo-section">
                <!-- Conteúdo dinâmico de promoções -->
            </div>
        </section>

        <section id="pecas">
            <h2>Peças de Computador</h2>
            <div class="product-grid">
                <!-- Produtos de hardware -->
                <div class="product-card">
                    <h3>Placa de Vídeo RTX 4080</h3>
                    <p>Kabum - R$ 7.999,00</p>
                    <div class="coupon-code">CUPOM: KABUM10</div>
                </div>
                <!-- Mais produtos -->
            </div>
        </section>

        <section id="games">
            <h2>Jogos para PC e Console</h2>
            <div class="product-grid">
                <!-- Produtos de jogos -->
                <div class="product-card">
                    <h3>Cyberpunk 2077</h3>
                    <p>Steam - R$ 199,00</p>
                    <div class="coupon-code">CUPOM: STEAMSUMMER</div>
                </div>
                <!-- Mais jogos -->
            </div>
        </section>

        <div class="retailer-logos">
            <img src="kabum-logo.png" alt="Kabum" class="retailer-logo">
            <img src="terabyte-logo.png" alt="Terabyte" class="retailer-logo">
            <img src="steam-logo.png" alt="Steam" class="retailer-logo">
            <!-- Demais logos -->
        </div>
    </main>

    <footer>
        <!-- Rodapé com informações -->
    </footer>
</body>
</html>
