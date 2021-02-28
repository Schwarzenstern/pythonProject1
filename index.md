## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/Schwarzenstern/pythonProject1/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Schwarzenstern/pythonProject1/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

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
      {% block content %}{% endblock %}
  </div>
</body>
</html>

{% extends 'main/base.html' %}

{% block title %}
Прототип страницы тесте
{% endblock %}

{% block content %}
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
{% endblock %}
