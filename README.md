<img src="img/icone.png" >
<h1>AntiDDOS</h1>
Простой способ защитить ваше веб-приложение от DDOS-атаки (СВОБОДНО) в * 1 строке *.

## Лицензия:
[LICENSE](https://github.com/MrPHP-Team/module-anti-ddos/blob/master/LICENSE "LICENSE")

## Как это работает?
<img src="img/icon.png" >

При каждом соединении система временно сохраняет IP-адрес клиента и контролирует частоту его соединения, если эта частота соединения ненормальная, то система рассматривает его как черный IP-адрес и отправляет запрос проверки в форме проверки. Капча интегрирована в систему, если он пройдет эту проверку, то это человек, а не робот!

**"Этот проект был протестирован несколькими программами ddos ​​с результатом 77%."**
## Как использовать это?

### Базовое использование
```php
<?php
	include ("anti_ddos/start.php"); //напишите это в верхней части вашего index.php и все готово !!!
?>
```
