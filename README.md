<!DOCTYPE html>
<html>
<head>
    <title>Vostok357 Minecraft</title>
    <style>
        :root {
            --primary: #2563eb;
            --dark: #0f172a;
            --light: #f8fafc;
            --success: #10b981;
        }
        body {
            background: linear-gradient(135deg, var(--dark) 0%, #1e293b 100%);
            color: var(--light);
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            min-height: 100vh;
            margin: 0;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 40px 20px;
        }
        .header {
            text-align: center;
            margin-bottom: 60px;
        }
        .logo {
            font-size: 3em;
            font-weight: 900;
            background: linear-gradient(45deg, var(--primary), #7c3aed);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 10px;
        }
        .card {
            background: rgba(30, 41, 59, 0.7);
            backdrop-filter: blur(10px);
            border-radius: 16px;
            padding: 30px;
            margin: 30px 0;
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }
        .step {
            display: flex;
            align-items: center;
            margin: 25px 0;
            gap: 20px;
        }
        .step-number {
            background: var(--primary);
            color: white;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            flex-shrink: 0;
        }
        .download-btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: var(--primary);
            color: white;
            padding: 15px 25px;
            border-radius: 10px;
            text-decoration: none;
            font-weight: 600;
            margin: 10px 5px;
            transition: transform 0.2s, box-shadow 0.2s;
        }
        .download-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(37, 99, 235, 0.3);
        }
        .server-info {
            background: rgba(16, 185, 129, 0.1);
            border-left: 4px solid var(--success);
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
        }
        .copy-box {
            background: rgba(0,0,0,0.3);
            padding: 15px;
            border-radius: 8px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 15px 0;
        }
        .qr-code {
            text-align: center;
            margin: 30px 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="logo">VOSTOK357</div>
            <p style="opacity: 0.8;">Minecraft Survival Server</p>
        </div>

        <div class="card">
            <h2>🎮 Быстрый старт</h2>
            
            <div class="step">
                <div class="step-number">1</div>
                <div>
                    <h3>Скачайте лаунчер</h3>
                    <p>Выберите удобный лаунчер:</p>
                    <div>
                        <a href="https://tlauncher.org/" class="download-btn">⬇️ TLaucher</a>
                        <a href="https://www.minecraft.net" class="download-btn">⬇️ Official</a>
                    </div>
                </div>
            </div>

            <div class="step">
                <div class="step-number">2</div>
                <div>
                    <h3>Установите сборку</h3>
                    <p>Скачайте и установите наш модпак:</p>
                    <a href="YOUR_GOOGLE_DRIVE_LINK" class="download-btn">
                        📦 Скачать сборку (4.2 GB)
                    </a>
                    <p style="font-size: 0.9em; opacity: 0.7; margin-top: 10px;">
                        Архив → Распаковать в папку .minecraft → Выбрать профиль "Vostok357"
                    </p>
                </div>
            </div>

            <div class="step">
                <div class="step-number">3</div>
                <div>
                    <h3>Подключитесь к серверу</h3>
                    <div class="server-info">
                        <p><strong>Сервер готов к подключению!</strong></p>
                        <div class="copy-box">
                            <code style="font-size: 1.2em;">vostok357.ddns.net:24</code>
                            <button onclick="copyIP()" style="background: var(--primary); color: white; border: none; padding: 8px 15px; border-radius: 6px; cursor: pointer;">Копировать</button>
                        </div>
                        <a href="minecraft://vostok357.ddns.net:24" class="download-btn" style="background: var(--success);">
                            🎯 Автоподключение
                        </a>
                    </div>
                </div>
            </div>
        </div>

        <div class="card">
            <h2>📋 Инструкция подробно</h2>
            <details>
                <summary>Для новичков (развернуть)</summary>
                <div style="padding: 20px;">
                    <h4>Установка TLaucher:</h4>
                    <p>1. Скачайте с официального сайта</p>
                    <p>2. Запустите установщик</p>
                    <p>3. В настройках поставьте русский язык</p>
                    
                    <h4>Установка сборки:</h4>
                    <p>1. Скачайте архив с модами</p>
                    <p>2. Нажмите Win+R, введите %appdata%</p>
                    <p>3. Найдите папку .minecraft</p>
                    <p>4. Распакуйте архив туда (с заменой файлов)</p>
                    
                    <h4>Подключение:</h4>
                    <p>1. Запустите TLaucher</p>
                    <p>2. Выберите версию "1.20.4 Forge"</p>
                    <p>3. Нажмите "Играть"</p>
                    <p>4. Мультиплеер → Добавить сервер → Вставьте адрес</p>
                </div>
            </details>
        </div>

        <div class="card">
            <h2>📱 Быстрая связь</h2>
            <p style="margin-bottom: 20px;">Есть вопросы или проблемы с подключением?</p>
            <div style="display: flex; gap: 15px; flex-wrap: wrap;">
                <a href="https://t.me/YOUR_TG" class="download-btn" style="background: #0088cc;">💬 Telegram</a>
                <a href="https://discord.gg/YOUR_DISCORD" class="download-btn" style="background: #5865f2;">🎮 Discord</a>
                <a href="mailto:your@email.com" class="download-btn" style="background: #ea4335;">📧 Email</a>
            </div>
            
            <div class="qr-code">
                <p>Или отсканируйте QR-код для быстрого доступа:</p>
                <img src="https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=vostok357.ddns.net:24" alt="QR Code">
                <p style="font-size: 0.9em; opacity: 0.7;">vostok357.ddns.net:24</p>
            </div>
        </div>
    </div>

    <script>
        function copyIP() {
            navigator.clipboard.writeText('vostok357.ddns.net:24');
            alert('Адрес скопирован в буфер!');
        }
        
        // Слушаем клик по автоподключению
        document.querySelector('[href^="minecraft://"]').addEventListener('click', function(e) {
            if(!confirm('Открыть Minecraft с автоматическим подключением?')) {
                e.preventDefault();
            }
        });
    </script>
</body>
</html>
