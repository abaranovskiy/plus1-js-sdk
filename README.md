plus1-js-sdk
============


Код для установки на площадке

Инструкция по установке кода:
 * Узнайте Ваш идентификатор площадки в интерфейсах plus1.wapstart.ru на странице получения кода или в службе клиентской поддержке.
 * Разместите код из блока 1 в теле страниц в тех местах, на которых планируется показ рекламных объявлений.

   * блок 1

```html
    <div class="wapstart-plus1-ad"></div>
```

 * Разместите код из блока 2 в конце каждой из страниц, на которых планируется показ рекламных объявлений.
   * блок 2

```html
    <script type="text/javascript">
    (function() {
    var plus1SiteId = _ВАШ_ИДЕНТИФИКАТОР_В_СИСТЕМЕ_PLUS1_;
    
    // Возраст (age): мы принимаем информацию о возрасте пользователя в виде целого числа (число полных лет).
    var age = _ВОЗРАСТ_ПОЛЬЗОВАТЕЛЯ_;
    
    // Пол (sex): мы принимаем информацию о поле пользователя в виде строки „man“ или „woman“. 
    // Другие значения недопустимы.
    var sex = _ПОЛ_ПОЛЬЗОВАТЕЛЯ_; 
    
    // Логин (login): допустима передача строки. Мы рекомендуем передавать не сам логин, а его хеш. Например sha1($login).
    var login = _ЛОГИН_ПОЛЬЗОВАТЕЛЯ_; 
    
    // Пожалуйста, согласуйте формат данных geoData с WapStart
    var geoData = _ДАННЫЕ_О_МЕСТОПОЛОЖЕНИИ_;
    
    
    var c = document.createElement('script'); c.type = 'text/javascript'; c.async = true; c.src = 'http://ro.plus1.wapstart.ru/?area=getJsCode&id=' + plus1SiteId + '&age=' + age + '&sex=' + sex + '&login=' + login + '&location=' + geoData + '&encoding=1'; var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(c, s);
    })();
    </script>
```
