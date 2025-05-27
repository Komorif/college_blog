<mark style="background: #FF5582A6;">1. Установка SQL Server и SSMS</mark>
(1) Переходим на сайт: [https://www.microsoft.com/en-us/sql-server/sql-server-downloads], затем выбираем SQL Server 2022 Developer и устанавливаем

![[Pasted image 20250527210602.png]]

(2) Открываем скачанный .exe файл, затем в Developer Edition выбираем Базовая (Basic)

![[Pasted image 20250527210843.png]]

(3) Выбираем язык (по умолчанию русский), затем жмем кнопку принять

![[Pasted image 20250527211024.png]]

(4) Оставляем место установки по умолчанию и жмем установить

![[Pasted image 20250527211107.png]]

(5)
1 вариант: После успешной установки переходим по этой ссылке [https://learn.microsoft.com/ru-ru/ssms/release-history] и скачиваем последнюю версию SSMS.

![[Pasted image 20250527212012.png]]

2 вариант: После успешной установки нажимаем на кнопку установить SSMS затем ищем последнюю версию и скачиваем, после чего можем нажать кнопку закрыть

![[Pasted image 20250527211454.png]]

(5) После скачивания SSMS открываем .exe файл. Путь оставляем по умолчанию затем жмем install

![[Pasted image 20250527212350.png]]

(6) После успешной установки жмем close

![[Pasted image 20250527212558.png]]

(7) Пишем в поиске sql server, затем открываем его

![[Pasted image 20250527212644.png]]

(8)
В Server name ставим DESKTOP-.. (наш пк)
В Authentication ставим Windows Authentication
В Encryption выбираем Mandatory и ставим галочку (Trust server certificate)
После этого нажимаем connect

![[Pasted image 20250527213136.png]]

<mark style="background: #FF5582A6;">2. Настройка сервера</mark>

<mark style="background: #3B83BD;">1. Включение доступа по логину и паролю</mark>

(1) Нажимаем правой кнопкой мыши по DESKTOP-.. и properties

![[Pasted image 20250527213709.png]]

(2) Security затем жмем SQL Server and Windows Authentication mode

![[Pasted image 20250527213750.png]]

(3) Соглашаемся на перезапуск SSMS, после перезагружаем локальный сервер

![[Pasted image 20250527214303.png]]

(4) раскрываем папку Security затем Logins после чего нажимаем правой кнопкой мыши по "sa" затем properties

![[Pasted image 20250527215234.png]]

(5)
1 - Свой пароль с буквами и цифрами
2- Политики безопасности

![[Pasted image 20250527215915.png]]

3 - Нажимаем Status слева
4 - проставляем галочки как на фото
После всего жмем ОК

![[Pasted image 20250527220215.png]]

(6) 
1 - Жмем "вилку"
2 - В Authentication выбираем SQL Server Authentication
3 - Пишем Login: sa Password: "ваш пароль"

![[Pasted image 20250527220623.png]]