---
title: "Homebrew Launcher (Channel)" #
lang: ru
permalink: /homebrew-launcher-channel.html
author_profile: true
---

{% include toc title="Разделы" %}

Мы установим Homebrew Channel таким образом, что при запуске патченной SysNAND, Homebrew Channe появится в виде иконки в системном меню.

## Что понадобится

* Свежая версия [WUP Installer GX2 (Channel)](http://www.wiiubru.com/appstore/chan_zips/wup_installer_gx2.zip)
* Свежая версия [Homebrew Launcher Channel](https://github.com/dimok789/homebrew_launcher/releases/latest) *(`.zip-архив` с суффиксом _channel)*

## Инструкция

### Часть I - Подготовительные работы

1. Выключите консоль
1. Вставьте SD-карту в компьютер
1. Создайте папку `install` в корне SD-карты
1. Создайте папку `hbc` в папке `/install/` на SD-карте
1. Скопируйте _содержимое_ `.zip-архива` с Homebrew Launcher Channel в папку `/install/hbc`
1. Скопируйте _содержимое_ `.zip-архива` с WUP Installer GX2 (Channel) в папку `/install/`

### Часть II - Установка каналов

1. Запустите Homebrew Launcher
	+ Пользователи CBHC должны нажать кнопку (HOME) во время загрузки для доступа к меню CBHC, где необходимо выбрать Homebrew Launcher
	+ Пользователи Haxchi должны сначала запустить Haxchi, чтобы пропатчить SysNAND, а затем запустить его еще раз, удерживая (A), чтобы запустить Homebrew Launcher
	+ Пользователи Mocha CFW должны сперва запустить Mocha CFW, а затем перезапустить Homebrew Launcher
1. Запустите WUP Installer GX2
	+ Если WUP Installer GX2 падает с ошибкой "DSi Exception Has Occurred", перезапустите приставку и попробуйте заново.
1. Отметьте галочками "hbc" и "WUP Installer GX2"
1. Нажмите "Install" для установки, а затем "Yes" для подтверждения
1. Выберите "NAND" в качестве места установки
1. Нажмите (HOME), а затем Закрыть программу (Close the software) для выхода из установщика по завершении установки

___

Теперь вы можете запускать Homebrew Launcher из патченного SysNAND, просто воспользовавшись Homebrew Channel.
{: .notice}

Для того, чтобы научиться устанавливать игры, перейдите [сюда](games)
{: .notice--success}

Помните, что для доступа к eShop с установленными DNS, вам необходимо сначала запустить NNU-Patcher из Homebrew Launcher (NNU-Patcher - временный патч и его нужно запускать каждый раз после перезагрузки, если вам нужен доступ к eShop).
{: .notice--info}

Помните, что если вы перенесете WUP Installer GX2 на USB-носитель (через Системные настройки), он сможет устанавливать приложения только на него же.
{: .notice--warning}

В целях безопасности крайне *желательно* выполнить резервное копирование NAND, следуя [инструкции](nand-backup).
{: .notice--success}

Для информации о том, как сохранять игры с дисков в формате, пригодном для установки в систему для последующей игры без диска, перейдите к странице с [disc2app](disc2app).
{: .notice--success}

Для информации об установке модов vWii в SysNAND, перейдите к странице [vWii Modding](vwii-modding).
{: .notice--success}

Для информации о безопасном удалении кастомной прошивки и возвращении консоли к заводскому состоянию, перейдите на страницу [Удаление кастомной прошивки](uninstall-cfw).
{: .notice--warning}
