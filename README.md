# Основные META-теги, влияющие на отображение страницы

## Кодировка страницы

```html
<!-- Старый формат -->
<meta http-equiv="Content-type" content="text/html;charset=UTF-8" />

<!-- HTML5 -->
<meta charset="UTF-8" />
```

## Настройки адаптивности страницы

### Фиксированная ширина

```html
<meta name="viewport" content="width=1170" />
```

### Адаптивная ширина

```html
<meta name="viewport" content="width=device-width" />
```

### Отключение автоссылки на телефон для iOS

```html
<meta name="format-detection" content="telephone=no" />
```

---

## SEO

### Краткое описание страницы (до 140 символов)

```html
<meta name="description" content=" " />
```

### Ключевые слова (до 20 слов, через запятую)

```html
<meta name="keywords" content=" " />
```

### Управление доступом поисковых роботов к странице

```html
<meta name="robots" content="" />
```

**Примеры:**

- Полный запрет индексации:

  ```html
  <meta name="robots" content="noindex, nofollow" />
  <!-- или -->
  <meta name="robots" content="none" />
  ```

- Запрет индексации ссылок и изображений:
  ```html
  <meta name="robots" content="noimageindex, nofollow" />
  ```

---

## Технические теги

```html
<!-- Автор -->
<meta name="Author" content="Пупкин Василий Петрович" />

<!-- Авторские права -->
<meta name="Copyright" content="Зимина Татьяна Юрьевна" />

<!-- Адрес автора -->
<meta name="Address" content="Луна, кратер №97" />

<!-- Редирект -->
<meta http-equiv="refresh" content="S; url=URL" />
```

- `S` — задержка в секундах
- `URL` — адрес для перенаправления

---

## Для социальных сетей

### Facebook (Open Graph)

```html
<meta property="og:locale" content="ru_RU" />
<meta property="og:type" content="article" />
<meta property="og:title" content="META теги" />
<meta property="og:description" content="Описание страницы про META теги" />
<meta property="og:image" content="http://fls.guru/meta/img/bg.jpg" />
<meta property="og:url" content="http://fls.guru/meta/" />
<meta property="og:site_name" content="Фрилансер по жизни" />
```

✅ Проверка разметки:  
[Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/sharing/)  
📘 Подробнее: [Open Graph Protocol](https://ruogp.me/)

---

### Twitter Cards

```html
<meta name="twitter:card" content="summary" />
<meta name="twitter:site" content="Жека" />
<meta name="twitter:title" content="META теги" />
<meta name="twitter:description" content="про META теги" />
<meta name="twitter:image" content="http://fls.guru/meta/img/bg.jpg" />
```

✅ Проверка:  
[Twitter Card Validator](https://cards-dev.twitter.com/validator)  
📘 Документация:  
[Twitter Cards Guide](https://developer.twitter.com/en/docs/tweets/optimize-with-cards/guides/getting-started)
