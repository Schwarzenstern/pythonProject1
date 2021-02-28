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
