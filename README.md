<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
    <title>Vostok357 | Minecraft Server</title>
    <style>
        :root {
            --primary: #2563eb;
            --dark: #0f172a;
            --light: #f8fafc;
            --success: #10b981;
            --accent: #7c3aed;
        }

        * {
            box-sizing: border-box;
        }

        body {
            background: linear-gradient(145deg, var(--dark) 0%, #1e293b 100%);
            color: var(--light);
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            min-height: 100vh;
            margin: 0;
            line-height: 1.5;
            -webkit-font-smoothing: antialiased;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        .header {
            text-align: center;
            margin-bottom: 50px;
        }

        .logo {
            font-size: 3.2em;
            font-weight: 900;
            background: linear-gradient(45deg, var(--primary), var(--accent));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 10px;
            letter-spacing: 2px;
            line-height: 1.2;
        }

        .sub {
            font-size: 1.2em;
            opacity: 0.85;
            border-bottom: 1px solid rgba(255,255,255,0.1);
            padding-bottom: 20px;
        }

        .card {
            background: rgba(30, 41, 59, 0.7);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border-radius: 28px;
            padding: 30px;
            margin: 35px 0;
            border: 1px solid rgba(255,255,255,0.05);
            box-shadow: 0 20px 35px -8px rgba(0,0,0,0.5);
            transition: transform 0.2s ease;
        }

        .card:hover {
            transform: translateY(-2px);
        }

        .step {
            display: flex;
            align-items: flex-start;
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
            font-weight: 700;
            font-size: 1.3em;
            flex-shrink: 0;
            box-shadow: 0 6px 12px rgba(37,99,235,0.3);
        }

        .download-btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            background: var(--primary);
            color: white;
            padding: 14px 28px;
            border-radius: 40px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1em;
            margin: 10px 0 5px;
            transition: all 0.25s ease;
            border: none;
            cursor: pointer;
            box-shadow: 0 8px 16px rgba(0,0,0,0.2);
            border: 1px solid rgba(255,255,255,0.1);
        }

        .download-btn:hover {
            background: #1d4ed8;
            transform: translateY(-3px);
            box-shadow: 0 12px 24px rgba(37,99,235,0.4);
        }

        .server-card {
            background: linear-gradient(145deg, rgba(16,185,129,0.08) 0%, rgba(5,150,105,0.03) 100%);
            border-left: 6px solid var(--success);
            border-radius: 20px;
            padding: 25px;
            margin-top: 20px;
        }

        .copy-box {
            background: rgba(0,0,0,0.4);
            padding: 16px 20px;
            border-radius: 18px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 15px;
            border: 1px solid rgba(255,255,255,0.08);
            backdrop-filter: blur(4px);
        }

        .server-address {
            font-size: 1.5em;
            font-weight: 600;
            font-family: 'Courier New', monospace;
            letter-spacing: 1px;
            color: var(--success);
            word-break: break-word;
            cursor: pointer;
        }

        .copy-btn {
            background: rgba(255,255,255,0.1);
            color: white;
            border: 1px solid rgba(255,255,255,0.15);
            padding: 10px 22px;
            border-radius: 30px;
            font-size: 1em;
            font-weight: 500;
            cursor: pointer;
            transition: 0.2s;
            display: flex;
            align-items: center;
            gap: 8px;
            backdrop-filter: blur(4px);
        }

        .copy-btn:hover {
            background: rgba(255,255,255,0.2);
            border-color: rgba(255,255,255,0.3);
            transform: scale(1.02);
        }

        .instruction-block {
            background: rgba(0,0,0,0.2);
            border-radius: 20px;
            padding: 20px 25px;
            margin-top: 20px;
            border: 1px solid rgba(255,255,255,0.03);
        }

        .instruction-block h4 {
            margin-top: 0;
            margin-bottom: 15px;
            color: #94a3b8;
            font-size: 1.1em;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .instruction-block ol,
        .instruction-block ul {
            margin: 0;
            padding-left: 20px;
        }

        .instruction-block li {
            margin: 10px 0;
            color: #cbd5e1;
        }

        .modrinth-badge {
            background: #1bd96a;
            color: #000;
            font-weight: 600;
            padding: 4px 12px;
            border-radius: 30px;
            font-size: 0.8em;
            display: inline-block;
            margin-left: 10px;
            letter-spacing: 0.3px;
        }

        code {
            background: #0f172a;
            padding: 4px 10px;
            border-radius: 30px;
            font-size: 0.9em;
            color: #e2e8f0;
            border: 1px solid rgba(255,255,255,0.1);
        }

        details {
            margin-top: 20px;
            background: rgba(0,0,0,0.2);
            padding: 18px 22px;
            border-radius: 18px;
            border: 1px solid rgba(255,255,255,0.03);
        }

        summary {
            cursor: pointer;
            color: #94a3b8;
            font-weight: 500;
            list-style: none;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        summary::-webkit-details-marker {
            display: none;
        }

        .footer {
            text-align: center;
            color: #64748b;
            font-size: 0.9em;
            margin-top: 60px;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.05);
        }

        a {
            color: var(--primary);
            text-decoration: none;
        }

        .note {
            background: rgba(245,158,11,0.08);
            border-left: 4px solid #f59e0b;
            padding: 16px 22px;
            border-radius: 16px;
            margin-top: 25px;
            color: #fde047;
            font-weight: 450;
        }

        /* Адаптация под мобильные устройства */
        @media (max-width: 640px) {
            .container {
                padding: 20px 16px;
            }

            .logo {
                font-size: 2.4em;
            }

            .sub {
                font-size: 1em;
            }

            .card {
                padding: 25px 18px;
                margin: 25px 0;
            }

            .step {
                flex-direction: column;
                align-items: flex-start;
                gap: 12px;
            }

            .step-number {
                width: 40px;
                height: 40px;
                font-size: 1.2em;
            }

            .download-btn {
                width: 100%;
                justify-content: center;
                padding: 14px 20px;
                font-size: 1em;
            }

            .copy-box {
                flex-direction: column;
                align-items: flex-start;
            }

            .copy-btn {
                width: 100%;
                justify-content: center;
            }

            .server-address {
                font-size: 1.2em;
                word-break: break-all;
            }

            .instruction-block ol,
            .instruction-block ul {
                padding-left: 18px;
            }

            .card > div[style*="grid-template-columns"] {
                grid-template-columns: 1fr !important;
                gap: 20px !important;
            }
        }

        @media (max-width: 380px) {
            .logo {
                font-size: 2em;
            }

            .server-address {
                font-size: 1.1em;
            }

            .card {
                padding: 20px 14px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="logo">VOSTOK357</div>
            <div class="sub">Vanilla+ сервер Minecraft на базе Homestead</div>
        </div>

        <!-- ШАГ 1: Prism Launcher -->
        <div class="card">
            <div class="step">
                <div class="step-number">1</div>
                <div style="flex: 1;">
                    <h2 style="margin-top: 0; margin-bottom: 8px;">Установите Prism Launcher и дополнительные моды (обязательный шаг)</h2>
                    <p style="opacity: 0.85; margin-bottom: 16px;">
                        Кроссплатформенный лаунчер с Modrinth, CurseForge и автоматической установкой модов.
                    </p>
                    <a href="https://github.com/Diegiwg/PrismLauncher-Cracked/releases/download/10.0.2/PrismLauncher-Windows-MSVC-Setup-10.0.2.exe" 
                       class="download-btn">
                        ⬇️ Скачать Prism Launcher (Windows)
                    </a>
                    <a href="mods.7z" download class="download-btn">
    📦 Скачать дополнительные моды (7z, 2,4 МБ)
                    </a>
                    <p style="font-size: 0.85em; opacity: 0.6; margin-top: 12px;">
                        Версия 10.0.2 (cracked) · Modrinth
                    </p>
                </div>
            </div>
        </div>

        <!-- ШАГ 2: Установка Homestead -->
        <div class="card">
            <div class="step">
                <div class="step-number">2</div>
                <div style="flex: 1;">
                    <h2 style="margin-top: 0; margin-bottom: 12px;">Установите Homestead</h2>

                    <div class="instruction-block">
                        <h4>📦 Пошаговая инструкция</h4>
                        <ol style="margin-bottom: 0;">
                            <li><strong>Запустите Prism Launcher</strong> и войдите в аккаунт, либо создайте автономный (пиратский)</li>
                            <li>Нажмите <code>«Добавить экземпляр»</code> (Add Instance)</li>
                            <li>Выберите вкладку <strong>Modrinth</strong></li>
                            <li>В поиске введите: <code>Homestead</code></li>
                            <li>Выберите версию <strong>1.2.9.4</strong> <span class="modrinth-badge">Modrinth</span></li>
                            <li>Нажмите «OK» — сборка скачается автоматически</li>
                            <li style="margin-top: 12px;"><strong>Выберите пункт «Изменить...»</strong> в меню сборки</li>
                            <li>В левом меню выберите <strong>«Параметры»</strong></li>
                            <li>Сверху переключитесь на вкладку <strong>«Java»</strong></li>
                            <li><strong>Включите галочку «Память»</strong> и установите <strong>5120 MiB</strong> для обоих полей (минимум и максимум)</li>
                            <li><strong>Докиньте</strong> дополнительные моды из архива в папку mods/</li>
                        </ol>
                    </div>

                    <details>
                        <summary>🔍 Что такое Homestead?</summary>
                        <p style="margin-top: 15px; margin-bottom: 0; color: #cbd5e1;">
                            🌿 Homestead — модпак Vanilla+ для исследователей, строителей и любителей приключений. 
                            Квесты, новые постройки, мобы, предметы — всё это сохраняет дух ванильного Minecraft, 
                            но позволяет играть гораздо дольше.
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
                    <p style="opacity: 0.85; margin-bottom: 16px;">
                        Сервер работает 24/7. Скопируйте адрес и добавьте в мультиплеер.
                    </p>

                    <div class="server-card">
                        <div class="copy-box">
                            <div>
                                <div style="font-size: 0.75em; opacity: 0.6; margin-bottom: 5px;">АДРЕС СЕРВЕРА</div>
                                <span class="server-address" onclick="copyAddress(event)">vostok357.ddns.net:24</span>
                            </div>
                            <button class="copy-btn" onclick="copyAddress(event)">📋 Копировать</button>
                        </div>

                        <div style="background: rgba(0,0,0,0.2); padding: 16px; border-radius: 16px; margin-top: 16px;">
                            <p style="margin: 0; display: flex; gap: 8px; align-items: baseline; flex-wrap: wrap;">
                                <span style="opacity: 0.7;">➡️ В игре:</span>
                                <strong>Мультиплеер → Добавить сервер → Вставить адрес → Готово</strong>
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Частые вопросы / решение проблем -->
        <div class="card" style="background: rgba(23, 25, 35, 0.7);">
            <h3 style="margin-top: 0; margin-bottom: 25px; display: flex; align-items: center; gap: 10px;">
                <span style="font-size: 1.6em;">⚠️</span> Если что-то пошло не так
            </h3>

            <div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 25px; max-width: 100%;">
                <div>
                    <h4 style="margin-bottom: 12px; color: #fca5a5;">❌ Не подключается</h4>
                    <ul style="margin: 0; padding-left: 20px; color: #cbd5e1;">
                        <li style="margin-bottom: 8px;">Версия — <strong>1.20.1 (Fabric)</strong></li>
                        <li style="margin-bottom: 8px;">Homestead строго <strong>1.2.9.4</strong></li>
                        <li style="margin-bottom: 8px;">Отключите брандмауэр / антивирус</li>
                        <li style="margin-bottom: 8px;">Перезапустите Prism</li>
                    </ul>
                </div>
                <div>
                    <h4 style="margin-bottom: 12px; color: #fca5a5;">🐢 Тормозит / вылетает</h4>
                    <ul style="margin: 0; padding-left: 20px; color: #cbd5e1;">
                        <li style="margin-bottom: 8px;">Выделите рекомендованную ОЗУ: <strong>5–10 GB</strong></li>
                        <li style="margin-bottom: 8px;">Обновите драйверы</li>
                        <li style="margin-bottom: 8px;">Отключите шейдеры</li>
                        <li style="margin-bottom: 8px;">Увеличьте выделенную память</li>
                    </ul>
                </div>
            </div>

            <div class="note">
                <strong>📌 Не нашли ответ?</strong> Пишите администратору.
            </div>
        </div>

        <div class="footer">
            Vostok357 Network · 1.20.1 · Homestead 1.2.9.4
        </div>
    </div>

    <script>
        function copyAddress(event) {
            const text = 'vostok357.ddns.net:24';
            navigator.clipboard.writeText(text);

            const btn = event.currentTarget;
            const originalText = btn.innerHTML;
            const isButton = btn.classList.contains('copy-btn');

            if (isButton) {
                btn.innerHTML = '✅ Скопировано!';
                btn.style.background = 'rgba(16, 185, 129, 0.25)';
                btn.style.borderColor = 'rgba(16, 185, 129, 0.4)';
            } else {
                // Если кликнули по адресу — показываем уведомление
                const originalBg = btn.style.background;
                btn.style.background = 'rgba(16, 185, 129, 0.15)';
                btn.style.borderRadius = '12px';
                btn.style.padding = '2px 6px';
                
                setTimeout(() => {
                    btn.style.background = 'transparent';
                    btn.style.borderRadius = '0';
                    btn.style.padding = '0';
                }, 200);
                return;
            }

            setTimeout(() => {
                btn.innerHTML = '📋 Копировать';
                btn.style.background = 'rgba(255,255,255,0.1)';
                btn.style.borderColor = 'rgba(255,255,255,0.15)';
            }, 2000);
        }
    </script>
</body>
</html>
