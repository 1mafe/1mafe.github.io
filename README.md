<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vostok357 | Minecraft Server</title>
    <style>
        :root {
            --primary: #2563eb;
            --dark: #0f172a;
            --light: #f8fafc;
            --success: #10b981;
            --accent: #7c3aed;
        }
        body {
            background: linear-gradient(145deg, var(--dark) 0%, #1e293b 100%);
            color: var(--light);
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            min-height: 100vh;
            margin: 0;
            line-height: 1.6;
        }
        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
        }
        .header {
            text-align: center;
            margin-bottom: 60px;
        }
        .logo {
            font-size: 3.5em;
            font-weight: 900;
            background: linear-gradient(45deg, var(--primary), var(--accent));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 5px;
            letter-spacing: 2px;
        }
        .sub {
            font-size: 1.2em;
            opacity: 0.8;
            border-bottom: 1px solid rgba(255,255,255,0.1);
            padding-bottom: 20px;
        }
        .card {
            background: rgba(30, 41, 59, 0.6);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border-radius: 24px;
            padding: 35px;
            margin: 35px 0;
            border: 1px solid rgba(255,255,255,0.05);
            box-shadow: 0 20px 35px -8px rgba(0,0,0,0.5);
        }
        .step {
            display: flex;
            align-items: flex-start;
            margin: 30px 0;
            gap: 20px;
        }
        .step-number {
            background: var(--primary);
            color: white;
            width: 44px;
            height: 44px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 1.3em;
            flex-shrink: 0;
            box-shadow: 0 6px 12px rgba(37,99,235,0.25);
        }
        .download-btn {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            background: var(--primary);
            color: white;
            padding: 16px 28px;
            border-radius: 14px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1em;
            margin: 8px 0;
            transition: all 0.2s ease;
            border: none;
            cursor: pointer;
            box-shadow: 0 8px 16px rgba(0,0,0,0.2);
        }
        .download-btn:hover {
            background: #1d4ed8;
            transform: translateY(-3px);
            box-shadow: 0 12px 24px rgba(37,99,235,0.35);
        }
        .server-card {
            background: linear-gradient(145deg, rgba(16,185,129,0.1) 0%, rgba(5,150,105,0.05) 100%);
            border-left: 6px solid var(--success);
            border-radius: 20px;
            padding: 25px;
            margin: 30px 0;
        }
        .copy-box {
            background: rgba(0,0,0,0.35);
            padding: 18px 20px;
            border-radius: 16px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 20px 0;
            border: 1px solid rgba(255,255,255,0.08);
            backdrop-filter: blur(4px);
        }
        .server-address {
            font-size: 1.5em;
            font-weight: 600;
            font-family: 'Courier New', monospace;
            letter-spacing: 1px;
            color: var(--success);
        }
        .copy-btn {
            background: rgba(255,255,255,0.1);
            color: white;
            border: 1px solid rgba(255,255,255,0.15);
            padding: 10px 20px;
            border-radius: 12px;
            font-size: 1em;
            font-weight: 500;
            cursor: pointer;
            transition: 0.15s;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        .copy-btn:hover {
            background: rgba(255,255,255,0.2);
            border-color: rgba(255,255,255,0.3);
        }
        .status {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: rgba(0,0,0,0.3);
            padding: 10px 18px;
            border-radius: 40px;
            font-size: 0.95em;
            margin-top: 10px;
        }
        .online { color: #4ade80; }
        .offline { color: #f87171; }
        .instruction-block {
            background: rgba(0,0,0,0.2);
            border-radius: 18px;
            padding: 20px 25px;
            margin-top: 15px;
            border: 1px solid rgba(255,255,255,0.03);
        }
        .instruction-block h4 {
            margin-top: 0;
            margin-bottom: 15px;
            color: #94a3b8;
            font-size: 1.1em;
        }
        .instruction-block ol, .instruction-block ul {
            margin: 0;
            padding-left: 20px;
        }
        .instruction-block li {
            margin: 8px 0;
            color: #cbd5e1;
        }
        .modrinth-badge {
            background: #1bd96a;
            color: black;
            font-weight: 600;
            padding: 4px 10px;
            border-radius: 20px;
            font-size: 0.8em;
            display: inline-block;
            margin-left: 10px;
        }
        hr {
            border: none;
            border-top: 1px solid rgba(255,255,255,0.08);
            margin: 40px 0 20px;
        }
        .footer {
            text-align: center;
            color: #64748b;
            font-size: 0.9em;
            margin-top: 50px;
        }
        a {
            color: var(--primary);
            text-decoration: none;
        }
        .note {
            background: rgba(245,158,11,0.1);
            border-left: 4px solid #f59e0b;
            padding: 15px 20px;
            border-radius: 12px;
            margin: 25px 0;
            color: #fcd34d;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="logo">VOSTOK357</div>
            <div class="sub">Minecraft — ванильный сервер с Homestead</div>
        </div>

        <!-- ШАГ 1: Prism Launcher -->
        <div class="card">
            <div class="step">
                <div class="step-number">1</div>
                <div style="flex: 1;">
                    <h2 style="margin-top: 0; margin-bottom: 8px;">Установите Prism Launcher</h2>
                    <p style="opacity: 0.8; margin-bottom: 20px;">
                        Кроссплатформенный лаунчер с поддержкой Modrinth, CurseForge и автоматической установкой модов.
                    </p>
                    <a href="https://github.com/Diegiwg/PrismLauncher-Cracked/releases/download/10.0.2/PrismLauncher-Windows-MSVC-Setup-10.0.2.exe" 
                       class="download-btn">
                        ⬇️ Скачать Prism Launcher (Windows)
                    </a>
                    <p style="font-size: 0.9em; opacity: 0.6; margin-top: 12px;">
                        Версия 10.0.2 (cracked) · Поддерживает Modrinth
                    </p>
                </div>
            </div>
        </div>

        <!-- ШАГ 2: Установка Homestead -->
        <div class="card">
            <div class="step">
                <div class="step-number">2</div>
                <div style="flex: 1;">
                    <h2 style="margin-top: 0; margin-bottom: 8px;">Установите сборку Homestead</h2>
                    <p style="opacity: 0.8;">
                        Чистый ванильный+ опыт с улучшенным выживанием.
                    </p>
                    
                    <div class="instruction-block">
                        <h4>📦 Пошаговая инструкция</h4>
                        <ol style="margin-bottom: 0;">
                            <li><strong>Запустите Prism Launcher</strong> и войдите в аккаунт</li>
                            <li>Нажмите кнопку <code style="background: #0f172a; padding: 3px 8px; border-radius: 6px;">«Добавить экземпляр»</code> (Add Instance)</li>
                            <li>Выберите вкладку <strong>Modrinth</strong></li>
                            <li>В поиске введите: <code style="background: #0f172a; padding: 3px 8px; border-radius: 6px;">Homestead</code></li>
                            <li>Выберите версию <strong>1.2.9.4</strong> <span class="modrinth-badge">Modrinth</span></li>
                            <li>Нажмите «OK» — сборка скачается и установится автоматически</li>
                            <li>Версия Minecraft: <strong>1.20.1</strong>, Forge</li>
                        </ol>
                    </div>
                    
                    <details style="margin-top: 20px; background: rgba(0,0,0,0.15); padding: 15px; border-radius: 12px;">
                        <summary style="cursor: pointer; color: #94a3b8; font-weight: 500;">
                            🔍 Что такое Homestead?
                        </summary>
                        <p style="margin-top: 15px; margin-bottom: 0; color: #cbd5e1;">
                            Homestead — это ванильная сборка, которая улучшает выживание, не ломая оригинальный дух Minecraft. 
                            Добавляет улучшенные деревни, структуры, мобов и рецепты, сохраняя ванильный баланс.
                        </p>
                    </details>
                </div>
            </div>
        </div>

        <!-- ШАГ 3: Подключение к серверу -->
        <div class="card">
            <div class="step">
                <div class="step-number">3</div>
                <div style="flex: 1;">
                    <h2 style="margin-top: 0; margin-bottom: 8px;">Подключитесь к серверу</h2>
                    <p style="opacity: 0.8; margin-bottom: 20px;">
                        Сервер работает круглосуточно. Просто скопируйте адрес и добавьте его в мультиплеер.
                    </p>
                    
                    <div class="server-card">
                        <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 20px;">
                            <span style="background: var(--success); width: 12px; height: 12px; border-radius: 50%; display: inline-block;"></span>
                            <span class="status" id="status-text">
                                🟢 Статус: <span id="status-online">загрузка...</span> · 
                                Игроков: <span id="player-count">?</span>/20
                            </span>
                        </div>
                        
                        <div class="copy-box">
                            <div>
                                <div style="font-size: 0.8em; opacity: 0.6; margin-bottom: 4px;">АДРЕС СЕРВЕРА</div>
                                <span class="server-address">vostok357.ddns.net:24</span>
                            </div>
                            <button class="copy-btn" onclick="copyAddress()">
                                📋 Копировать
                            </button>
                        </div>

                        <div style="background: rgba(0,0,0,0.2); padding: 16px; border-radius: 14px;">
                            <p style="margin: 0; display: flex; gap: 8px; align-items: baseline;">
                                <span style="opacity: 0.7;">➡️ В игре:</span> 
                                <strong>Мультиплеер → Добавить сервер → Вставить адрес → Готово</strong>
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Частые вопросы / решение проблем -->
        <div class="card" style="background: rgba(23, 25, 35, 0.6);">
            <h3 style="margin-top: 0; margin-bottom: 25px; display: flex; align-items: center; gap: 10px;">
                <span style="font-size: 1.5em;">⚠️</span> Если что-то пошло не так
            </h3>
            
            <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 25px; max-width: 100%;">
                <div>
                    <h4 style="margin-bottom: 15px; color: #fca5a5;">❌ Не подключается к серверу</h4>
                    <ul style="margin: 0; padding-left: 20px; color: #cbd5e1;">
                        <li>Проверьте версию — нужна <strong>1.20.1</strong> (Forge)</li>
                        <li>Убедитесь, что Homestead версии 1.2.9.4</li>
                        <li>Отключите брандмауэр/антивирус на 5 минут</li>
                        <li>Попробуйте перезапустить Prism</li>
                    </ul>
                </div>
                <div>
                    <h4 style="margin-bottom: 15px; color: #fca5a5;">🐢 Тормозит / вылетает</h4>
                    <ul style="margin: 0; padding-left: 20px; color: #cbd5e1;">
                        <li>Выделите больше ОЗУ в настройках Prism</li>
                        <li>Минимум <strong>4GB</strong>, рекомендуется 6GB</li>
                        <li>Обновите драйверы видеокарты</li>
                        <li>Установите Java 17</li>
                    </ul>
                </div>
            </div>
            
            <div class="note" style="margin-top: 25px; margin-bottom: 0;">
                <strong>📌 Не нашли ответ?</strong> Проверьте версию сборки: Modrinth → Homestead → версия должна быть строго 1.2.9.4 (более новые могут не подходить).
            </div>
        </div>

        <div class="footer">
            Vostok357 Network · Сервер работает на 1.20.1 · Homestead 1.2.9.4
        </div>
    </div>

    <script>
        // Копирование адреса в буфер
        function copyAddress() {
            navigator.clipboard.writeText('vostok357.ddns.net:24');
            
            const btn = event.currentTarget;
            const originalText = btn.innerHTML;
            btn.innerHTML = '✅ Скопировано!';
            btn.style.background = 'rgba(16, 185, 129, 0.3)';
            
            setTimeout(() => {
                btn.innerHTML = '📋 Копировать';
                btn.style.background = 'rgba(255,255,255,0.1)';
            }, 2000);
        }

        // Авто-обновление статуса сервера
        async function updateServerStatus() {
            try {
                const response = await fetch('https://api.mcsrvstat.us/2/vostok357.ddns.net:24');
                const data = await response.json();
                
                const statusEl = document.getElementById('status-online');
                const playersEl = document.getElementById('player-count');
                
                if (data.online) {
                    statusEl.innerHTML = '🟢 ONLINE';
                    statusEl.style.color = '#4ade80';
                    playersEl.innerHTML = data.players.online || '0';
                } else {
                    statusEl.innerHTML = '🔴 OFFLINE';
                    statusEl.style.color = '#f87171';
                    playersEl.innerHTML = '0';
                }
            } catch (e) {
                document.getElementById('status-online').innerHTML = '⚪ Нет данных';
                document.getElementById('player-count').innerHTML = '?';
            }
        }

        updateServerStatus();
        setInterval(updateServerStatus, 45000);
    </script>
</body>
</html>
