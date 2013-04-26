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

    var c = document.createElement('script'); c.type = 'text/javascript'; c.async = true; c.src = 'http://ro.plus1.wapstart.ru/?area=getJsCode&id=' + plus1SiteId + '&encoding=1'; var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(c, s);
    })();
    </script>
```
