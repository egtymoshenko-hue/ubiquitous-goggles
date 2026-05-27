<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>VegasGift Mini App</title>
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            background-color: #0b1118;
            color: white;
            margin: 0;
            padding: 20px;
            text-align: center;
            -webkit-user-select: none;
        }
        .header {
            margin-top: 20px;
            padding: 15px;
            background: linear-gradient(135deg, #1e293b, #0f172a);
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);
        }
        h1 {
            color: #f59e0b;
            margin: 0 0 10px 0;
            font-size: 24px;
        }
        .balance-box {
            font-size: 18px;
            margin: 15px 0;
            background: rgba(255,255,255,0.05);
            padding: 10px;
            border-radius: 10px;
        }
        .balance-num {
            font-weight: bold;
            color: #10b981;
            font-size: 22px;
        }
        .btn {
            display: block;
            width: 100%;
            padding: 15px;
            margin: 15px 0;
            background: #2481cc;
            color: white;
            border: none;
            border-radius: 12px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            box-shadow: 0 4px 10px rgba(36,129,204,0.3);
        }
        .btn-crash { background: linear-gradient(135deg, #ef4444, #b91c1c); }
        .btn-cases { background: linear-gradient(135deg, #8b5cf6, #6d28d9); }
    </style>
</head>
<body>

    <div class="header">
        <h1>🎰 VegasGift App</h1>
        <p>Добро пожаловать в игровой стартап Mini App!</p>
        <div class="balance-box">
            Твой баланс: <span class="balance-num">100.00 TON</span>
        </div>
    </div>

    <button class="btn btn-crash" onclick="alert('Игра Краш запускается...')">🚀 Играть в Crash</button>
    <button class="btn btn-cases" onclick="alert('Открытие кейсов...')">🎁 Открыть Кейсы (Xmas Stocking)</button>
    <button class="btn" onclick="tgClose()">❌ Закрыть приложение</button>

    <script>
        // Автоматическое расширение внутри Telegram
        const tg = window.Telegram.WebApp;
        tg.expand();

        function tgClose() {
            tg.close();
        }
    </script>
</body>
</html>
