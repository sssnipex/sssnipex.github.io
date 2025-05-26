<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>mini-adapter sil2nt.t.me</title>
    <meta name="description" content="Адаптер для быстрого доступа к ресурсам">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700&display=swap" rel="stylesheet">
    <style>
        @font-face {
            font-family: 'Coves Bold';
            src: url('https://fonts.cdnfonts.com/css/coves') format('woff2');
            font-weight: bold;
            font-style: normal;
        }
        
        body {
            margin: 0;
            padding: 0;
            font-family: 'Coves Bold', 'Montserrat', sans-serif;
            background: linear-gradient(90deg, #1a1a1a 0%, #2e2e2e 50%, #1a1a1a 100%);
            color: #ffffff;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .container {
            text-align: center;
            padding: 30px;
            max-width: 900px;
            width: 90%;
            animation: fadeIn 0.8s ease-out;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .header {
            margin-bottom: 50px;
        }
        
        .header a {
            color: white;
            text-decoration: none;
            font-size: 3rem;
            letter-spacing: 2px;
            text-shadow: 0 0 8px rgba(100, 180, 255, 0.6), 0 0 16px rgba(100, 180, 255, 0.4);
            transition: all 0.3s ease;
            position: relative;
            font-family: 'Coves Bold', sans-serif;
        }
        
        .header a:hover {
            text-shadow: 0 0 12px rgba(100, 180, 255, 0.8), 0 0 24px rgba(100, 180, 255, 0.6);
        }
        
        .buttons-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 25px;
            width: 100%;
        }
        
        @media (min-width: 768px) {
            .buttons-grid {
                grid-template-columns: 1fr 1fr;
            }
        }
        
        .btn {
            display: flex;
            align-items: center;
            justify-content: flex-start;
            padding: 20px 25px;
            background-color: rgba(40, 40, 40, 0.8);
            color: white;
            text-decoration: none;
            border-radius: 12px;
            font-size: 1.5rem;
            transition: all 0.3s ease;
            border: 1px solid #333;
            cursor: pointer;
            height: 120px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(5px);
            font-family: 'Coves Bold', sans-serif;
        }
        
        .btn:hover {
            background-color: rgba(60, 60, 60, 0.9);
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
            border-color: rgba(100, 180, 255, 0.6);
        }
        
        .btn-icon {
            width: 60px;
            height: 60px;
            margin-right: 20px;
            object-fit: contain;
            border-radius: 10px;
            background-color: rgba(50, 50, 50, 0.5);
            padding: 8px;
            box-sizing: border-box;
            filter: brightness(1.1) contrast(1.1);
        }
        
        footer {
            margin-top: 60px;
            color: #666;
            font-size: 0.9rem;
            letter-spacing: 1px;
            font-family: 'Coves Bold', sans-serif;
        }
        
        #toTop {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: rgba(40, 40, 40, 0.8);
            color: rgba(100, 180, 255, 0.8);
            border: none;
            cursor: pointer;
            display: none;
            font-size: 1.5rem;
            transition: all 0.3s;
            backdrop-filter: blur(5px);
            border: 1px solid #333;
        }
        
        #toTop:hover {
            background-color: rgba(60, 60, 60, 0.9);
            color: rgba(100, 180, 255, 1);
            border-color: rgba(100, 180, 255, 0.6);
        }
        
        #toTop.show {
            display: block;
        }
        
        @media (max-width: 600px) {
            .header a {
                font-size: 2rem;
            }
            
            .btn {
                height: 100px;
                font-size: 1.2rem;
            }
            
            .btn-icon {
                width: 50px;
                height: 50px;
                margin-right: 15px;
                padding: 5px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <a href="https://t.me/sil2nt" target="_blank" rel="noopener noreferrer">mini-adapter sil2nt.t.me</a>
        </div>
        
        <div class="buttons-grid">
            <a href="https://t.me/sxdsg_bot" class="btn" target="_blank" rel="noopener noreferrer">
                <img src="https://www.buildableweb.com/pub/photo/blueshop.png" class="btn-icon" alt="Заказ">
                <span>Сделать заказ в ТГ</span>
            </a>
            
            <a href="https://t.me/SnipDesign" class="btn" target="_blank" rel="noopener noreferrer">
                <img src="https://t22.ru/images/telegram8.png" class="btn-icon" alt="Канал">
                <span>Мой канал в Телеграм</span>
            </a>
            
            <a href="https://t.me/SnipPortfolio" class="btn" target="_blank" rel="noopener noreferrer">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2c/Noto_Emoji_Oreo_1f4bc.svg/1200px-Noto_Emoji_Oreo_1f4bc.svg.png" class="btn-icon" alt="Портфолио">
                <span>Мое портфолио</span>
            </a>
            
            <a href="https://www.tiktok.com/@sssnipex" class="btn" target="_blank" rel="noopener noreferrer">
                <img src="https://i2.wp.com/www.pngplay.com/wp-content/uploads/9/TikTok-Logo-Transparent-Background.png" class="btn-icon" alt="TikTok">
                <span>Я в ТикТок</span>
            </a>
        </div>
        
        <footer>
            © 2023 sil2nt.t.me | Все права защищены
        </footer>
    </div>

    <button id="toTop" onclick="window.scrollTo({top: 0, behavior: 'smooth'})">↑</button>

    <script>
        // Кнопка "Наверх"
        const toTopButton = document.getElementById('toTop');
        
        window.addEventListener('scroll', () => {
            if (window.pageYOffset > 300) {
                toTopButton.classList.add('show');
            } else {
                toTopButton.classList.remove('show');
            }
        });

        // Анимация при загрузке
        document.addEventListener('DOMContentLoaded', () => {
            document.body.style.opacity = 1;
        });
    </script>
</body>
</html>
