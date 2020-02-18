---
title: "Homebrew Launcher (Channel)" #
permalink: /homebrew-launcher-channel.html
lang: ru
author_profile: true
---

{% include toc title="Разделы" %}

Мы установим Homebrew Channel таким образом, что при запуске кастомной прошивки, Homebrew Channel появится в виде иконки в системном меню.

## Инструкция

### Часть I - Установка каналов

1. Запустите **Homebrew Launcher**
	+ Пользователи **CBHC** должны нажать кнопку {% include inc/btn.md btn="HOME" %} во время загрузки для доступа к меню CBHC, где необходимо выбрать Homebrew Launcher
	+ Пользователи Haxchi должны сначала запустить Haxchi, а затем запустить его еще раз, удерживая {% include inc/btn.md btn="A" %}, чтобы войти в Homebrew Launcher
	+ Пользователи Mocha CFW должны просто запустить Homebrew Launcher
1. Запустите WUP Installer GX2
	+ Если WUP Installer GX2 падает с ошибкой "**DSi Exception Has Occurred**", перезапустите приставку и попробуйте заново.
1. Отметьте галочками "**HBL**" и "**WUP Installer GX2**"
1. Нажмите "**Install**" для установки, а затем "**Yes**" для подтверждения
1. Выберите "**NAND**" в качестве места установки
1. Нажмите {% include inc/btn.md btn="HOME" %}, а затем Закрыть программу (Close the software) для выхода из установщика по завершении установки

___

Теперь вы можете запускать Homebrew Launcher из кастомной прошивки, просто воспользовавшись Homebrew Channel.
{: .notice}

Для того, чтобы научиться устанавливать игры, перейдите [сюда](games)
{: .notice--success}

Помните, что для доступа к eShop с установленными DNS, вам необходимо сначала запустить NNU-Patcher из Homebrew Launcher (NNU-Patcher - временный патч и его нужно запускать каждый раз после перезагрузки, если вам нужен доступ к eShop).
{: .notice--info}

Помните, что если вы перенесёте WUP Installer GX2 на USB-носитель (через Системные настройки), он сможет устанавливать приложения только на него же.
{: .notice--warning}

Для информации о том, как сохранять игры с дисков в формате, пригодном для установки в систему для последующей игры без диска, перейдите к странице с [disc2app](disc2app).
{: .notice--success}

Для информации об установке модов vWii в SysNAND, перейдите к странице [vWii Modding](vwii-modding).
{: .notice--success}

Для информации о безопасном удалении кастомной прошивки и возвращении консоли к заводскому состоянию, перейдите на страницу [Удаление кастомной прошивки](uninstall-cfw).
{: .notice--warning}
