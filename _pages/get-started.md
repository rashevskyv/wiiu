---
title: "Начало" #
lang: ru
permalink: /get-started.html
author_profile: true
---

{% include toc title="Разделы" %}

Следующие шаги подготовят вашу SD-карту к установке кастомной прошивки coldboothax
{: .notice--success}

Прежде всего, нужно убедиться, что прошивка вашей приставки 5.5.0 или 5.5.1. В новой прошивке 5.5.2 пропатчена уязвимость в браузере, которую нам необходимо использовать.
{: .notice--info}

Рекомендуется использовать SD-карту не менее 16 или 32Гб, иначе вам не хватит места для дампинга и установки игр.
{: .notice--info}

SD-карта должна быть отформатирована в FAT32 (с кластером в 64КБ или 32 КБ). Большинство SD-карт изначально так и отформатированы.
{: .notice--info}

Если вы планируете форматировать SD-карту в Windows, не используйте встроенную утилиту для форматирования, это в дальнейшем может вызывать проблемы. Лучше воспользуйтесь [`guiformat`](http://www.ridgecrop.demon.co.uk/index.htm?guiformat.htm). Установите "Allocation Unit Size" в "64kb".
{: .notice--warning}

**Нельзя** называть SD-карту `wiiu`, это приведет к проблемам.
{: .notice--warning}

Прежде чем начать, рекомендуется проверить свою SD-карту на ошибки с помощью [H2testw (Windows)](h2testw-windows), [F3 (Linux)](f3-linux), или [F3X (Mac)](f3x-mac)!
{: .notice--warning}


## Что понадобится
<a name="what_need" />

* [`config.txt`]({{ base_path }}/images/config.txt)
* Свежая версия [Homebrew App Store](https://github.com/vgmoose/hbas/releases/latest)
* Свежая версия [WUP Installer GX2 (Homebrew Launcher)](http://wiiubru.com/appstore/zips/wup_installer_gx2.zip)
* Свежая версия [WUP Installer GX2 (Channel)](http://www.wiiubru.com/appstore/chan_zips/wup_installer_gx2.zip)
* Свежая версия [disc2app](https://github.com/koolkdev/disc2app/releases/latest)
* Свежая версия [hid\_to\_vpad](https://github.com/Maschell/hid_to_vpad/releases/latest)
* Свежая версия [Mocha CFW](https://github.com/dimok789/mocha/releases/latest)
* Свежая версия [savemii](https://github.com/Ryuzaki-MrL/savemii/releases/latest)
* Свежая версия [Homebrew Launcher Channel](https://github.com/dimok789/homebrew_launcher/releases/latest) *(`.zip-архив` с суффиксом _channel)*
* Предыдущая версия [the Homebrew Launcher](https://github.com/dimok789/homebrew_launcher/releases/tag/1.4) *(`homebrew_launcher.v1.4.zip`)*
* Свежая версия [Haxchi и CBHC](https://github.com/FIX94/haxchi/releases/latest) *(оба `.zip-архива`)*
* Свежая версия [NNU-Patcher](https://wiiubru.com/appstore/zips/nnupatcher.zip)


## Инструкция
<a name="instructions" />

#### Часть I - Подготовительные работы
<a name="part1" />

1. Выключите консоль
1. Вставьте SD-карту в компьютер
1. Создайте папку `wiiu` в корне SD-карты
1. Создайте папку `install` в корне SD-карты
1. Скопируйте папку `apps` из `.zip-архива` с Hombebrew App Stor в папку `/wiiu/` на SD-карте
1. Скопируйте _содержимое_ `.zip-архива` с Homebrew Launcher в корень вашей SD-карты
1. Скопируйте _содержимое_ `.zip-архива` с Haxchi в корень вашей SD-карты
1. Скопируйте _содержимое_ `.zip-архива` с CBHC в корень вашей SD-карты
1. Скопируйте `config.txt` в папку `/haxchi/` на SD-карте
1. Создайте папку `hbc` в папке `/install/` на SD-карте
1. Скопируйте _содержимое_ `.zip-архива` с Homebrew Launcher Channel в папку `/install/hbc/`на SD-карте
1. Скопируйте папку `WUP_Installer_GX2` из `.zip-архива` с WUP Installer GX2 (Channel) в папку `/install/` на SD-карте
1. Создайте папку `mocha` в папке `/wiiu/apps/` на SD-карте
1. Скопируйте `mocha.elf` из `.zip-архива` с Mocha CFW в папку `/wiiu/apps/mocha/`на SD-карте
1. Скопируйте папку `savemii` из `.zip-архива` с savemii в папку `/wiiu/apps/` на SD-карте
1. Скопируйте с заменой _содержимое_ `.zip-архива` с WUP Installer GX2 (Homebrew Launcher) в корень SD-карты
1. Скопируйте с заменой _содержимое_ `.zip-архива` с disc2app в корень вашей SD-карты
1. Скопируйте с заменой _содержимое_ `.zip-архива` с hid\_to\_vpad в корень вашей SD-карты
1. Скопируйте с заменой _содержимое_ `.zip-архива` с NNU-Patcher в корень вашей SD-карты
1. Вставьте SD-карту обратно в консоль
1. Включите консоль

#### Часть II - Блокировка обновления системы
<a name="part2" />

Обратите внимание, что если вы не заблокируете обновления этим методом на текущем и всех будущих интернет-соединениях, то все обновления для WiiU будут скачиваться и устанавливаться *автоматически* без вашего ведома и *не могут* быть отменены. 
{: .notice--danger}

Помните, что для доступа к eShop с установленными DNS, вам необходимо сначала запустить NNU-Patcher из Homebrew Launcher (NNU-Patcher - временный патч и его нужно запускать каждый раз после перезагрузки, если вам нужен доступ к eShop).
{: .notice--info}

1. Перейдите в Системные настройки (System Settings), Интернет (Internet), Подключиться к Интернету (Connect to the Internet), нажмите (X) для того, чтобы отобразить имеющиеся подключения
1. Для каждого из имеющихся подключений (и для всех созданных в будущем), проделайте нижеследующие инструкции
  Проверка соединения
  + Выберите "Изменить настройки" (Change Settings)
  + Перейдите на вторую страницу и выберите "DNS"
  + В пункте меню DNS выберите "Не получать автоматически" (Don't Auto-Obtain)
  + Введите указанные ниже адреса DNS
  + `168.235.092.108`
  + `081.004.127.020`
  + Нажмите "Подтвердить" (Confirm), а затем (B), чтобы сохранить внесенные изменения
  + Эти сервера заблокируют получение обновлений SysNAND на Wii U

___

Следующий шаг: [Homebrew Launcher](homebrew-launcher)
{: .notice--success}
