---
title: "Модификация vWii" #
lang: ru
permalink: /vwii-modding.html
author_profile: true
---

{% include toc title="Разделы" %}

Мы установим Homebrew Channel и другие модификации для встроенного в Wii U эмулятора Wii (vWii - virtual Wii).

Помните, что без оригинального контроллера Wii, вы не сможете зайти в vWii
{: .notice--warning}

Если вы хотите изменить регион вашей vWii на европейский, перейдите [сюда](wiiu-region-change). После выполнения этой инструкции прошивать vWii уже не нужно будет. Вы можете выполнить смену региона вместо прошивки vWii. Результат будет идентичен
{: .notice--info}

## Инструкция

### Часть I - Подготовительные работы

1. Выключите консоль
1. Вставьте SD-карту в компьютер
1. Скопируйте _содержимое_ `.zip-архива` {% include inc/sdfiles.md %} в корень вашей SD-карты
  * Не нужно делать, если уже делали в процессе выполнения руководства
1. Вставьте SD-карту обратно в консоль
1. Включите консоль

### Часть II - установка Homebrew Menu

1. Запустите **vWii Compat Installer** (![](/images/apps/compat_installer.png){:width="60px"})
1. Нажмите {% include inc/btn.md btn="A" %} для того, чтобы установить **Homebrew Channel**
1. Дождитесь надписи **Install succeeded**
1. Нажмите {% include inc/btn.md btn="HOME" %}, чтобы вернуться в системное меню
1. Запустите **vWii**
  * Если установка прошла успешно, на экране появится **Homebrew Channel**

### Часть III - установка и настройка Priiloader

1. Запустите **Homebrew Channel**
1. Запустите **Priiloader Installer** и дождитесь инициализации программы
1. Нажмите кнопку {% include inc/btn.md btn="+" %} на контроллере Wii 
1. По завершению работы программы, нажмите {% include inc/btn.md btn="A" %}
1. Запустите **Load Priiloader**
1. Перейдите в **System Menu Hacks** и нажмите {% include inc/btn.md btn="A" %}
1. Кнопкой {% include inc/btn.md btn="A" %} переведите в состояние **enable** следующие пункты:
  * Block Online Updates
  * Wii System Settings via Options Button
  * Remove Deflicker (не трогайте, если используете старый телевизор)
1. Выберите **System settings**, чтобы сохранить настройки
1. Нажмите {% include inc/btn.md btn="B" %}, чтобы вернуться в главное меню
1. Выберите **Homebrew Channel**, чтобы вернуться к выбору Homebrew

### Часть IV - установка cIOS

Убедитесь, что в корне SD-карты нет папок `wad` или `wads` и что нет никаких `.wad-файлов` нигде, кроме папки `/apps/`на SD-карте.
{: .notice--warning}

1. Запустите **Homebrew Channel** на vWii
1. Запустите **d2x cIOS Installer**
1. Установите параметры в верхней части экрана таким образом, чтобы они соответствовали нижеуказанным:
  + Select cIOS : **d2x-v11-beta1-vWii**
  + Select cIOS base : **56**
  + Select cIOS slot : **249**
1. Нажмите {% include inc/btn.md btn="A" %} для установки
1. Дождитесь окончания установки и нажмите {% include inc/btn.md btn="A" %} для продолжения
1. Установите параметры в верхней части экрана таким образом, чтобы они соответствовали нижеуказанным:
  + Select cIOS : **d2x-v11-beta1-vWii**
  + Select cIOS base : **57**
  + Select cIOS slot : **250**
1. Нажмите {% include inc/btn.md btn="A" %} для установки
1. Дождитесь окончания установки и нажмите {% include inc/btn.md btn="A" %} для продолжения
1. Установите параметры в верхней части экрана таким образом, чтобы они соответствовали нижеуказанным:
  + Select cIOS : **d2x-v11-beta1-vWii**
  + Select cIOS base : **58**
  + Select cIOS slot : **251**
1. Нажмите {% include inc/btn.md btn="A" %} для установки
1. Дождитесь окончания установки и нажмите {% include inc/btn.md btn="B" %} для выхода

### Часть V - применение патчей к IOS80

Этот шаг брикнет вашу vWii, если по какой-то причине будет прерван в процессе применения патчей (отключение электроэнергии, например). В таком случае для восстановления будет необходима резервная копи NAND vWii. Убедитесь, что она у вас есть, перед тем как начинать.
{: .notice--danger}

1. Из **Homebrew Channel** в vWii, запустите "**Patched IOS80 Installer for vWii**""
1. Внимательно прочтите предупреждение и подождите 30 секунд, после чего сможете продолжить
1. Нажмите {% include inc/btn.md btn="A" %} для установки
  + Все должно пройти очень быстро
1. По завершении процесса, нажмите любую кнопку, чтобы вернуться в Homebrew Channel

### Часть V - применение патчей к ww-43db

С помощью этой утилиты применяются патчи для поддержки 16:9 в ряде WiiWare игр 

1. Из **Homebrew Channel** в vWii, запустите "**ww-43-db-patcher**""
1. Дождитесь окончания инициализации патчера
1. Нажмите  нажмите {% include inc/btn.md btn="1" %} для начала работы программы
1. Дождитесь окончания работы патчера и нажмите любую кнопку для возврата в **Homebrew Channel**

### Часть VI - Установка загрузчиков игр vWii и запуск игр

Об установке игр и лоадеров подробно рассказано на этой странице - [Установка игр для vWii](https://wiiu.customfw.xyz/games-vwii)

## Список установленных программ в **Homebrew Channel**: 

* [ftpii](https://oscwii.org/library/app/ftpii) - FTP-сервер
* [Homebrew Browser 0.3](https://oscwii.org/library/app/ww-43db-patcher) - возможность загружать новейшие приложения и игры для вашей Wii непосредственно через консоль
* [Riivolution Patcher](https://oscwii.org/library/app/riivolution) - инструмент для мгновенного внесения изменений в игры, который работает с розничными дисками
* [YAWM ModMii Edition 1.0.1](https://oscwii.org/library/app/yawmME) - менеджер и установщик WAD-файлов
* [SaveGame Manager GX rev127](https://oscwii.org/library/app/SaveGame_Manager_GX) - менеджер сохранений
* [WiiXplorer SS 260](https://oscwii.org/library/app/wiixplorer-ss) - файловый менеджер
* [WiiFlow WFL 5.5.4](https://oscwii.org/library/app/wiiflow) - программа для запуска игр с карты памяти
* [USB Loader GX 3.0 r1281](https://oscwii.org/library/app/usbloader_gx) - программа для запуска игр с карты памяти

Вы можете удалить следующие программы на этом этапе:
* [Priiloader Installer 0.10.0](https://oscwii.org/library/app/priiloader) - это приложение заменяет первую часть системного меню, загружающуюся на Wii. Это позволяет загружать его перед самим меню Wii. Установщик может как установить, так и удалить priiloader
* [Load Priiloader 1.0](https://oscwii.org/library/app/loadpriiloader) - загружает меню Priiloader через Homebrew Loader
* [`d2x_cIOS_Installer-vWii.zip`](https://wii.hacks.guide/assets/files/d2x_cIOS_Installer-vWii.zip) - патчи системных модулей
* [Patched IOS80 Installer for vWii 1.0](https://oscwii.org/library/app/Patched_IOS80_Installer_for_vWii) - устанавливает патченный IOS80 без проверки подписи на vWii
* [ww-43db-patcher 0.3](https://oscwii.org/library/app/ww-43db-patcher) - обновляет базу данных соотношения сторон 4:3 для WiiWare (43DB) в архиве системного меню vWii U8, заменяя записи. Это позволяет активировать доступ к соотношению сторон 16:9 в WiiWare-играх, где принудительно используется 4:3

___

Теперь вы можете установить и использовать любое хомбрю для vWii, например, [USB Loader GX](games-vwii#запуск-wii-игр-в-vwii-через-usb-loader-gx), [Wiiflow](games-vwii#запуск-wii-игр-в-vwii-через-wiiflow), CFG USB Loader, эмуляторы, и т. д.
{: .notice--success}

Для того, чтобы научиться устанавливать игры, перейдите [сюда](games)
{: .notice--success}

Внешний жесткий диск необходимо подключать в верхний USB-порт Wii U, иначе vWii не увидит его. Нельзя использовать тот же жесткий диск, что вы используете для игр Wii U. Если вы используете жесткий диск без собственного дополнительного питания, вам понадобится [Y-cable](http://amzn.to/2mjQjin).
{: .notice--info}

Убедитесь, что все `.wad-файлы`(каналы, форвардеры, игры, и т.д.), которые вы собираетесь устанавливать, [совместимы с vWii](https://gbatemp.net/threads/340226/). Если вы случайно установите `.wad-файл` не совместимый с vWii, а предназначенный для обычной Wii, вы получите брик вашей vWii и вам придется восстанавливать её из резервной копии NAND.
{: .notice--danger}

Установка кастомных тем в vWii так же приведёт к брику vWii.
{: .notice--danger}

Удаление `.wad-файлов` вручную без знания тонкостей этого процесса, так же приведут к брику vWii.
{: .notice--danger}