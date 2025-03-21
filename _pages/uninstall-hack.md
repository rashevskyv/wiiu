---
title: "Удаление ColdbootHax или Haxchi" #
lang: ru
permalink: /uninstall-hack.html
author_profile: true
---

{% include toc title="Разделы" %}

Мы удалим CFW из вашей Wii U. Метод удаления не зависит от метода установки. По окончанию инструкции, приставка вернется к изначальной конфигурации.
{: .notice--info}

Чтобы понять какой взлом у вас стоит, перейдите в **Системные настройки** (System Settings), **Управление данными** (Data Management). Если вы видите значок **CBHC** (![](/images/apps/cbhc.png){:width="60px"}) или **Haxchi** (![](/images/apps/haxchi.png){:width="60px"}), то у вас соответствующий взлом. Если этих значков нет, запустите браузер Wii U: если автоматически запускается Homebrew Launcher, у вас **Indexiine**
{: .notice--info}

## Часть I - Удаление из Wii U

### CBHC

1. Запустите **Homebrew Launcher Channel**
1. Запустите инсталлятор **CBHC**
1. Выберите ту игру от DS virtual console, из которой мы удаляем CBHC, а затем нажмите {% include inc/btn.md btn="A" %} для подтверждения выбора
  * Если игр установлено несколько и вы не уверены в какую именно внедрён взлом, методом исключения определите это, глянув на установленные игры в главном меню консоли, либо удаляйте взлом из каждой по очереди. 
1. Ознакомьтесь с появившимся предупреждением и нажмите {% include inc/btn.md btn="B" %} для удаления
1. Когда процесс завершится, вы вернетесь в системное меню
  * Надпись "**Removed coldboothax**" означает, что CBHC удалён успешно
1. **Перезагрузите Wii U** и убедитесь, что консоль сразу загружается в меню!
1. Откройте **Системные настройки** (System Settings), **Управление данными** (Data Management) и удалите вашу игру от DS virtual console
  * Игра будет отображаться так же как и тайтл CBHC и будет называться **DO NOT TOUCH ME**. Удалите этот тайтл ТОЛЬКО, если уверены, что CBHC успешно убран из консоли!
  * Вы можете установить игру от DS virtual console из eShop заново

### Haxchi

1. Откройте **Системные настройки** (System Settings), **Управление данными** (Data Management) и удалите вашу игру от DS virtual console
  * Игра будет отображаться так же как и тайтл Haxchi и будет называться **Haxchi**. 

### Indexiine

1. Запустите браузер, чтобы войти в Homebrew Launcher
1. Запустите **Indexiine-Installer**
1. Нажмите {% include inc/btn.md btn="B" %}, чтобы удалить Indexiine.
1. Убедитесь, что Wii U больше не запускает автоматически Homebrew Launcher при запуске браузера

## Часть II - Удаление из SD-карты

{% capture notice-3 %}
Удалите все файлы и папки из корня SD-карты, **кроме** указанных ниже (некоторых, а то и всех, может на карте не оказаться):

    + DCIM
    + private

{% endcapture %}

<div class="notice--info">{{ notice-3 | markdownify }}</div>

___

[Закрыть страницу](javascript:window.close();)
{: .notice--success}