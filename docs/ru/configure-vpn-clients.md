# 5. Конфигурирование VPN клиентов

## 5.1. Настройка мобильного клиента Андроид
Официальный клиент Wireguard для Андроид можно [установить из официального магазина GooglePlay](https://play.google.com/store/apps/details?id=com.wireguard.android)

После чего, необходимо имортировать конфигуацию, считав QR код с конфигурацией клиента (см. пункт [4.2.2](configure-wireguard.html#_4-2-2-qr-код-конфигурации-кnиента)) и дать ему имя:

![Настройка Андроид клиента Wireguard](/images/ru/android1.jpg)

После успешного импорта конфигурации, можно включить VPN тонель. Об успешном подключиении скажет значек ключика в системной панели Андроид

![Работающий Андроид клиент Wireguard](/images/ru/android2.jpg)

## 5.2. Настройка клиента Windows
Первоначально необходимо скачать и установить программу [TunSafe for Windows](https://tunsafe.com/download) - это клиент Wireguard для Windows.

### 5.2.1. Создание файла конфигурации для импорта
Правой кнопкой мышки создаем текстовый файл на рабочем столе. 

![Создание текстового файла](/images/ru/windows1.jpg)

### 5.2.2. Копирование содержимого файла конфигурации с сервера
Дальше возращаемя к терминалу Putty и отображаем содержимое конфигурационного файла нужного пользователя, как это описано на шаге [4.2.1](configure-wireguard.html#_4-2-1-файn-поnьзоватеnьской-конфигурации).   
Далее выделяем правой кнопкой мыши текст конфигурации в терминале Putty, по окончании выделения он автоматически скопируется в буфер обмена. 

![Копирование текста с конфигурацией](/images/ru/windows2.jpg)

### 5.2.3. Копирование конфигурации в локальный файл конфигурации
Поле этого возвращаемся к созданному нами ранее на рабочем столе текстовому файлу, и вставляем в него из буфера обмена текст конфигурации. 

![Копирование текста с конфигурацией](/images/ru/windows3.jpg)

### 5.2.4. Сохранение локального файла конфигурации
Сохраняем файл, с расширением **.conf** (в данном случае с именем `london.conf`)

![Сохранения файла с конфигурацией](/images/ru/windows4.jpg)

### 5.2.5. Импорт локального файла конфигурации
Далее необходимо импортировать файл конфигурации в программу TunSafe.

![Импорт файла конфигурации в TunSafe](/images/ru/windows5.jpg)

### 5.2.6. Установка VPN соединения
Выбрать этот файл конфигурации и подключится, нажав кнопку **Connect**.
![Подключение к серверу VPN через TunSafe](/images/ru/windows6.jpg)