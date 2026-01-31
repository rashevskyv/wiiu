---
title: "Модифікація vWii" #
lang: uk
permalink: /vwii-modding.html
author_profile: true
---

{% include toc title="Розділи" %}

Ми встановимо Homebrew Channel та інші модифікації для вбудованого у Wii U емулятора Wii (vWii - virtual Wii).

Пам'ятайте, що без оригінального контролера Wii ви не зможете зайти у vWii
{: .notice--warning}

Якщо ви хочете змінити регіон вашої vWii на європейський, перейдіть [сюди](wiiu-region-change). Після виконання цієї інструкції прошивати vWii вже не потрібно буде. Ви можете виконати зміну регіону замість прошивки vWii. Результат буде ідентичним
{: .notice--info}

## Інструкція

### Частина I - Підготовчі роботи

1. Вимкніть консоль
1. Вставте SD-карту в комп'ютер
1. Скопіюйте _вміст_ `.zip-архіву` {% include inc/sdfiles.md %} у корінь вашої SD-карти
  * Не потрібно робити, якщо вже робили в процесі виконання посібника
1. Вставте SD-карту назад у консоль
1. Увімкніть консоль

### Частина II - встановлення Homebrew Menu

1. Запустіть **vWii Compat Installer** (![](/images/apps/compat_installer.png){:width="60px"})
1. Натисніть {% include inc/btn.md btn="A" %} для того, щоб встановити **Homebrew Channel**
1. Дочекайтеся напису **Install succeeded**
1. Натисніть {% include inc/btn.md btn="HOME" %}, щоб повернутися в системне меню
1. Запустіть **vWii**
  * Якщо встановлення пройшло успішно, на екрані з'явиться **Homebrew Channel**

### Частина III - встановлення та налаштування Priiloader

1. Запустіть **Homebrew Channel**
1. Запустіть **Priiloader Installer** і дочекайтеся ініціалізації програми
1. Натисніть кнопку {% include inc/btn.md btn="+" %} на контролері Wii 
1. По завершенню роботи програми натисніть {% include inc/btn.md btn="A" %}
1. Запустіть **Load Priiloader**
1. Перейдіть до **System Menu Hacks** і натисніть {% include inc/btn.md btn="A" %}
1. Кнопкою {% include inc/btn.md btn="A" %} переведіть у стан **enable** наступні пункти:
>  * Block Online Updates
>  * Wii System Settings via Options Button
>  * Remove Deflicker (не чіпайте, якщо використовуєте старий телевізор)
1. Виберіть **System settings**, щоб зберегти налаштування
1. Натисніть {% include inc/btn.md btn="B" %}, щоб повернутися в головне меню
1. Виберіть **Homebrew Channel**, щоб повернутися до вибору Homebrew

### Частина IV - встановлення cIOS

Переконайтеся, що в корені SD-карти немає папок `wad` або `wads` і що немає жодних `.wad-файлів` ніде, крім папки `/apps/` на SD-карті.
{: .notice--warning}

1. Запустіть **Homebrew Channel** у vWii
1. Запустіть **d2x cIOS Installer**
1. Встановіть параметри у верхній частині екрана так, щоб вони відповідали вказаним нижче:
>  + Select cIOS : **d2x-v11-beta1-vWii**
>  + Select cIOS base : **56**
>  + Select cIOS slot : **249**
1. Натисніть {% include inc/btn.md btn="A" %} для встановлення
1. Дочекайтеся закінчення встановлення та натисніть {% include inc/btn.md btn="A" %} для продовження
1. Встановіть параметри у верхній частині екрана так, щоб вони відповідали вказаним нижче:
>  + Select cIOS : **d2x-v11-beta1-vWii**
>  + Select cIOS base : **57**
>  + Select cIOS slot : **250**
1. Натисніть {% include inc/btn.md btn="A" %} для встановлення
1. Дочекайтеся закінчення встановлення та натисніть {% include inc/btn.md btn="A" %} для продовження
1. Встановіть параметри у верхній частині екрана так, щоб вони відповідали вказаним нижче:
>  + Select cIOS : **d2x-v11-beta1-vWii**
>  + Select cIOS base : **58**
>  + Select cIOS slot : **251**
1. Натисніть {% include inc/btn.md btn="A" %} для встановлення
1. Дочекайтеся закінчення встановлення та натисніть {% include inc/btn.md btn="B" %} для виходу

### Частина V - застосування патчів до IOS80

Цей крок перетворить вашу vWii на «цеглу» (brick), якщо з якоїсь причини буде перерваний у процесі застосування патчів (наприклад, відключення електроенергії). У такому разі для відновлення буде необхідна резервна копія NAND vWii. Переконайтеся, що вона у вас є, перед тим як починати.
{: .notice--danger}

1. З **Homebrew Channel** у vWii запустіть "**Patched IOS80 Installer for vWii**"
1. Уважно прочитайте попередження і почекайте 30 секунд, після чого зможете продовжити
1. Натисніть {% include inc/btn.md btn="A" %} для встановлення
  * Все має пройти дуже швидко
1. По завершенні процесу натисніть будь-яку кнопку, щоб повернутися в Homebrew Channel

### Частина V - застосування патчів до ww-43db

За допомогою цієї утиліти застосовуються патчі для підтримки 16:9 у низці WiiWare ігор 

1. З **Homebrew Channel** у vWii запустіть "**ww-43-db-patcher**"
1. Дочекайтеся закінчення ініціалізації патчера
1. Натисніть {% include inc/btn.md btn="1" %} для початку роботи програми
1. Дочекайтеся закінчення роботи патчера і натисніть будь-яку кнопку для повернення в **Homebrew Channel**

### Частина VI - Встановлення завантажувачів ігор vWii та запуск ігор

Про встановлення ігор та лоадерів детально розповів на цій сторінці — [Встановлення ігор для vWii](https://wiiu.customfw.xyz/games-vwii)

## Список встановлених програм у **Homebrew Channel**

* [ftpii](https://oscwii.org/library/app/ftpii) - FTP-сервер
* [Homebrew Browser 0.3](https://oscwii.org/library/app/ww-43db-patcher) - можливість завантажувати новітні додатки та ігри для вашої Wii безпосередньо через консоль
* [Riivolution Patcher](https://oscwii.org/library/app/riivolution) - інструмент для миттєвого внесення змін в ігри, який працює з роздрібними дисками
* [YAWM ModMii Edition 1.0.1](https://oscwii.org/library/app/yawmME) - менеджер та установник WAD-файлів
* [SaveGame Manager GX rev127](https://oscwii.org/library/app/SaveGame_Manager_GX) - менеджер збережень
* [WiiXplorer SS 260](https://oscwii.org/library/app/wiixplorer-ss) - файловий менеджер
* [WiiFlow WFL 5.5.4](https://oscwii.org/library/app/wiiflow) - програма для запуску ігор з карти пам'яті
* [USB Loader GX 3.0 r1281](https://oscwii.org/library/app/usbloader_gx) - програма для запуску ігор з карти пам'яті

Ви можете видалити наступні програми на цьому етапі:
* [Priiloader Installer 0.10.0](https://oscwii.org/library/app/priiloader) - цей додаток замінює першу частину системного меню, що завантажується на Wii. Це дозволяє завантажувати його перед самим меню Wii. Установник може як встановити, так і видалити priiloader
* [Load Priiloader 1.0](https://oscwii.org/library/app/loadpriiloader) - завантажує меню Priiloader через Homebrew Loader
* [`d2x_cIOS_Installer-vWii.zip`](https://wii.hacks.guide/assets/files/d2x_cIOS_Installer-vWii.zip) - патчі системних модулів
* [Patched IOS80 Installer for vWii 1.0](https://oscwii.org/library/app/Patched_IOS80_Installer_for_vWii) - встановлює патчений IOS80 без перевірки підпису на vWii
* [ww-43db-patcher 0.3](https://oscwii.org/library/app/ww-43db-patcher) - оновлює базу даних співвідношення сторін 4:3 для WiiWare (43DB) в архіві системного меню vWii U8, замінюючи записи. Це дозволяє активувати доступ до співвідношення сторін 16:9 у WiiWare-іграх, де примусово використовується 4:3

___

Тепер ви можете встановити та використовувати будь-яке хомбрю для vWii, наприклад, [USB Loader GX](games-vwii#запуск-wii-ігр-у-vwii-через-usb-loader-gx), [Wiiflow](games-vwii#запуск-wii-ігр-у-vwii-через-wiiflow), CFG USB Loader, емулятори тощо.
{: .notice--success}

Для того, щоб навчитися встановлювати ігри, перейдіть [сюди](games)
{: .notice--success}

Зовнішній жорсткий диск необхідно підключати у верхній USB-порт Wii U, інакше vWii не побачить його. Не можна використовувати той самий жорсткий диск, який ви використовуєте для ігор Wii U. Якщо ви використовуєте жорсткий диск без власного додаткового живлення, вам знадобиться [Y-cable](http://amzn.to/2mjQjin).
{: .notice--info}

Переконайтеся, що всі `.wad-файли` (канали, форвардери, ігри тощо), які ви збираєтеся встановлювати, [сумісні з vWii](https://gbatemp.net/threads/340226/). Якщо ви випадково встановите `.wad-файл`, не сумісний з vWii, а призначений для звичайної Wii, ви отримаєте брік вашої vWii і вам доведеться відновлювати її з резервної копії NAND.
{: .notice--danger}

Встановлення кастомних тем у vWii так само призведе до бріку vWii.
{: .notice--danger}

Видалення `.wad-файлів` вручну без знання тонкощів цього процесу так само призведе до бріку vWii.
{: .notice--danger}

___

[Закрыть страницу](javascript:window.close();)
{: .notice--success}