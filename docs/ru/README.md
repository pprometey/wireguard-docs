# Бесплатный VPN сервис Wireguard на AWS

## Для чего?

С ростом цензурирования интернета авторитарными режимами, блокируются все большое количество полезных интернет ресурсов и сайтов.
Таким обзразом, становиться невозможно полноценно пользоваться интернетом и нарушается фундаменальное право на свободу слова, закрепленное во [Всеобщей декларации прав человека](https://www.un.org/ru/documents/decl_conv/declarations/declhr.shtml).
::: tip Статья 19
Каждый человек имеет право на свободу убеждений и на свободное выражение их; это право включает свободу беспрепятственно придерживаться своих убеждений и свободу искать, получать и распространять информацию и идеи любыми средствами и независимо от государственных границ
:::

В данном руководстве мы за 6 этапов развернем свой собственный бесплатный* [VPN сервис](https://ru.bmstu.wiki/VPN_(Virtual_Private_Network)) на базе технологии [Wireguard](https://www.wireguard.com/), в облачной инфраструктуре [Amazon Web Services](https://aws.amazon.com/ru/) (AWS), с помощью бесплатного аккаунта (на 12 месяцев), на инстансе (виртуальной машине) под управлением [Ubuntu Server 18.04 LTS](https://www.ubuntu.com/server).
Я старался сделать это пошаговое руководство как можно более дружественным к людям, далеким от ИТ. Единственное что требуется - это усидчивость в повторении описанных ниже шагов.   

::: tip Примечание
* AWS предоставляет [бесплатный уровень использования](https://aws.amazon.com/ru/free/faqs/) сроком на 12 месяцев, с ограничением на 15 гигабайт трафика в месяц.
:::

## Этапы 
1. [Регистрация бесплатного аккаунта AWS](aws-account-registration)
2. [Создание инстанса AWS](create-aws-instance)
3. [Подключение к инстансу AWS](connection-to-instance)
4. [Конфигурирование Wireguard](configure-wireguard)
5. [Конфигурирование VPN клиентов](configure-vpn-clients)
6. [Проверка корректности установки VPN](check-the-installation-of-vpn)

## Полезные ссылки
* [Скрипты автоматической установки Wireguard на AWS](https://github.com/isystem-io/wireguard-aws)