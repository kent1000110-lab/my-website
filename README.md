<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>我的個人作品集與線上商店</title>
    <style>
        /* ==========================================================================
           1. 全域樣式設定 (手機與電腦皆能完美適應)
           ========================================================================== */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: "Helvetica Neue", Arial, "Noto Sans TC", sans-serif;
        }
        body {
            background-color: #f4f6f9;
            color: #333;
            line-height: 1.6;
        }
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 60px 20px;
        }

        /* 區塊共同大標題 */
        .section-title {
            text-align: center;
            font-size: 2.2rem;
            margin-bottom: 40px;
            color: #222;
        }
        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background-color: #4a90e2;
            margin: 12px auto 0;
            border-radius: 2px;
        }

        /* ==========================================================================
           2. 各區塊專屬樣式
           ========================================================================== */
        
        /* 首頁大招牌 */
        .hero-banner {
            background: linear-gradient(135deg, #1f4068 0%, #162447 100%);
            color: #ffffff;
            text-align: center;
            padding: 120px 20px;
        }
        .hero-banner h1 {
            font-size: 3.5rem;
            margin-bottom: 15px;
            letter-spacing: 2px;
        }
        .hero-banner p {
            font-size: 1.3rem;
            opacity: 0.85;
        }

        /* 作品集格線排版 */
        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        .portfolio-card {
            background: #ffffff;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }
        .portfolio-card:hover {
            transform: translateY(-8px);
        }
        .portfolio-placeholder-img {
            width: 100%;
            height: 220px;
            background-color: #e2e8f0;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #718096;
            font-weight: 500;
        }
        .portfolio-content {
            padding: 25px;
        }
        .portfolio-content h3 {
            font-size: 1.4rem;
            margin-bottom: 10px;
            color: #1a1a1a;
        }
        .portfolio-content p {
            color: #666;
            font-size: 0.95rem;
        }

        /* 商品區塊 */
        .shop-box {
            background: #ffffff;
            border-radius: 12px;
            padding: 40px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.05);
            display: flex;
            flex-wrap: wrap;
            gap: 40px;
            align-items: center;
            margin-top: 20px;
        }
        .product-placeholder-img {
            flex: 1;
            min-width: 300px;
            height: 380px;
            background-color: #edf2f7;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #718096;
            font-size: 1.1rem;
            border-radius: 8px;
        }
        .product-details {
            flex: 1;
            min-width: 300px;
        }
        .product-title {
            font-size: 1.8rem;
            color: #111;
            margin-bottom: 10px;
        }
        .product-price {
            font-size: 2rem;
            color: #e53e3e;
            font-weight: 800;
            margin: 20px 0;
        }
        .product-description {
            color: #4a5568;
            font-size: 1.05rem;
            margin-bottom: 30px;
        }

        /* 台灣綠界金流專用按鈕 */
        .ecpay-button {
            display: inline-block;
            background-color: #38a169;
            color: #ffffff;
            text-decoration: none;
            padding: 16px 40px;
            font-size: 1.25rem;
            border-radius: 50px;
            font-weight: bold;
            box-shadow: 0 4px 12px rgba(56, 161, 105, 0.3);
            transition: all 0.2s ease;
            text-align: center;
        }
        .ecpay-button:hover {
            background-color: #2f855a;
            box-shadow: 0 6px 16px rgba(56, 161, 105, 0.4);
            transform: scale(1.02);
        }

        /* 頁尾版權 */
        footer {
            background-color: #1a202c;
            color: #a0aec0;
            text-align: center;
            padding: 30px 20px;
            margin-top: 60px;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <header class="hero-banner">
        <h1>我的個人作品集</h1>
        <p>歡迎來到我的專屬空間，這裡記錄了我的創作與精選商品</p>
    </header>

    <div class="container">
        
        <section id="portfolio" style="margin-bottom: 80px;">
            <h2 class="section-title">精選作品展示</h2>
            
            <div class="portfolio-grid">
                <div class="portfolio-card">
                    <div class="portfolio-placeholder-img">【作品主要照片預留處】</div>
                    <div class="portfolio-content">
                        <h3>作品名稱 01</h3>
                        <p>在這裡點擊編輯，可以寫下這個作品的背景故事、使用的技術（例如 3D 列印或設計理念）。</p>
                    </div>
                </div>

                <div class="portfolio-card">
                    <div class="portfolio-placeholder-img">【作品主要照片預留處】</div>
                    <div class="portfolio-content">
                        <h3>作品名稱 02</h3>
                        <p>在這裡點擊編輯，可以寫下這個作品的背景故事、使用的技術（例如 3D 列印或設計理念）。</p>
                    </div>
                </div>

                <div class="portfolio-card">
                    <div class="portfolio-placeholder-img">【作品主要照片預留處】</div>
                    <div class="portfolio-content">
                        <h3>作品名稱 03</h3>
                        <p>在這裡點擊編輯，可以寫下這個作品的背景故事、使用的技術（例如 3D 列印或設計理念）。</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="shop">
            <h2 class="section-title">線上商店</h2>
            
            <div class="shop-box">
                <div class="product-placeholder-img">【150元 商品照片預留處】</div>
                
                <div class="product-details">
                    <h3 class="product-title">【原創設計】精選個人特色商品</h3>
                    <p class="product-price">NT$ 150</p>
                    <p class="product-description">
                        這是一段吸引人的商品描述。你可以寫下商品的規格、材質、寄送方式或購買須知。好的文案能讓客人看了更想購買喔！
                    </p>
                    
                    <a href="https://www.ecpay.com.tw" target="_blank" class="ecpay-button">立即安全購買</a>
                </div>
            </div>
        </section>

    </div>

    <footer>
        <p>© 2026 我的個人品牌 版權所有. 歡迎透過 Email 或社群與我聯絡</p>
    </footer>

</body>
</html>
