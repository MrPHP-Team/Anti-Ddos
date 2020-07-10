<img src="img/icone.png" >
<h1>AntiDDOS-system</h1>
Простой способ защитить ваше веб-приложение от DDOS-атаки (СВОБОДНО) в * 1 строке *.

## Как это работает?
<img src="img/icon.png" >

При каждом соединении система временно сохраняет IP-адрес клиента и контролирует частоту его соединения, если эта частота соединения ненормальная, то система рассматривает его как черный IP-адрес и отправляет запрос проверки в форме проверки. Капча интегрирована в систему, если он пройдет эту проверку, то это человек, а не робот!

**"Этот проект был протестирован несколькими программами ddos ​​с результатом 77%."**
## Как использовать это?

### Базовое использование
```php
<?php
	include ("anti_ddos/start.php"); //напишите это в верхней части вашего PHP-приложения и все готово !!!
?>
<!DOCTYPE html>
<html>
<head>
	<title>
		Example Web page protected!
	</title>
</head>
	<body>
		...
		<h2>Example Web page protected!</h2>
		...
	</body>
</html>
```

### Продвинутое использование:
```php
<?php
	try{
		if (!file_exists('anti_ddos/start.php'))
			throw new Exception ('anti_ddos/start.php does not exist');
		else
			require_once('anti_ddos/start.php');
	}
	//Ловите исключение, если что-то идет не так.
	catch (Exception $ex) {
		// напечатаем сообщение о том, что произошла ошибка
		echo '<div style="padding:10px;color:white;position:fixed;top:0;left:0;width:100%;background:black;text-align:center;">
		<a href="#" target="_blank">"AntiDDOS System"</a> не удалось правильно загрузить на этом сайте, пожалуйста, оставьте комментарий \'catch Exception\' чтобы увидеть, что происходит!</div>';
		//Печатаем сообщение об ошибке
		//echo $ex->getMessage();
	}
?>
---- THE HTML PAGE CONTENT ----
```
### Скачивание (ZIP):
[ZIP](https://github.com/lkapitman/Anti-ddos/archive/master.zip "Download")
