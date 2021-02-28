<!doctype html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>{% block title %}{% endblock %}</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>
<body>
  <header class="d-flex flex-column flex-md-row align-items-center p-3 px-md-4 mb-3 bg-body border-bottom shadow-sm">
  <p class="h5 my-0 me-md-auto fw-normal">Цифровой методист</p>
  <nav class="my-2 my-md-0 me-md-3">
    <a class="p-2 text-dark" href="{% url 'home' %}">Главная</a>
    <a class="p-2 text-dark" href="{% url 'about' %}">Про нас</a>
      <a class="p-2 text-dark" href="{% url 'test' %}">Тест</a>
  </nav>
</header>

  <div class="container">
    
    <h1>Тест</h1>
  <p>Название раздела</p>
<html>
 <head>
  <meta charset="utf-8">
  <title>Прототип</title>
 </head>
 <body>
  <form>
   <!-- В форме должен быть action, вызывающий отправку запроса на бэкенд -->
   <p><b>Вопрос</b></p>
    <p><input name="choice" type="radio" value="1">1</p>
    <p><input name="choice" type="radio" value="2">2</p>
    <p><input name="choice" type="radio" value="3" onclick="alert('Выбран ответ №3')">3</p>
    <p><input name="choice" type="radio" value="4">4</p>
    <p><input type="submit" value="Дать ответ"></p>
   <!-- При нажатии на "Дать ответ" должен отправляться на бэкенд запрос, содержащий номер вопроса и номер ответа,
    бэкенд проверяет верность ответа по БД, и возвращает ответ с информацией о том, был ответ пользователя на
    тест верен или нет. Фронтенд получает ответ и отображает информацию из него -->
  </form>
 </body>
</html>
  </div>
</body>
</html>
