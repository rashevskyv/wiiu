---
title: "Tiramisu" #
lang: ru
permalink: /tiramisu.html
author_profile: true
---

{% include toc title="Разделы" %}

**Tiramisu** - это специальная модульная среда для Wii U. С её помощью можно автоматически запускать кастомную прошивку (модифицированную версию [Mocha](https://github.com/wiiu-env/MochaPayload){:target="_blank"}) при запуске консоли. 

В сочетании с **PayloadLoader** это бесплатная и модульная альтернатива CBHC с некоторыми дополнительными функциями, такими как полная поддержка меню быстрого запуска и блокировка обновлений.

Убедитесь, что не проскочили [подготовительные этапы](get-started), перед установкой Tiramisu!
{: .notice--warning}

## Часть I - Установка PayloadLoader

{% include inc/hbl.md btn="X" env="меню **Environment Loader**" %}
1. С помощью крестовины выберите **installer** и запустите его кнопкой {% include inc/btn.md btn="A" %}
1. Выберите **Check**, чтобы проверить можно ли установить **PayloadLoader** в приложение **"Информация о здоровье и безопасности"** (**"Health and Safety Information"**)
1. Выберите **Install / Update** кнопкой {% include inc/btn.md btn="A" %}
1. С помощью крестовины выберите **Install** и запустите установку кнопкой {% include inc/btn.md btn="A" %} 
1. Выберите "**Press A to shutdown**", чтобы выключить консоль

## Часть II - Блокировка обновлений 

1. Запустите приложение **"Информация о здоровье и безопасности"** (**"Health and Safety Information"**) (желтый триугольник с восклицательным знаком) -> **Tiramisu** -> **Homebrew Launcher**
1. Выберите **UFDiine** и нажмите {% include inc/btn.md btn="A" %}, чтобы заблокировать обновления на консоли 
1. Надпись **Update folder is deleted** означает, что обновления заблокированы
1. Выключите консоль кнопокой питания и включите её

## Часть III - Автозапуск PayloadLoader

1. Запустите приложение **"Информация о здоровье и безопасности"** из главного меню вашей консоли, удерживая кнопку {% include inc/btn.md btn="X" %}, чтобы попасть в меню **Environment Loader**
1. С помощью крестовины выберите **installer** и запустите его кнопкой {% include inc/btn.md btn="A" %}
1. Выберите **Check** -> **Boot options**
1. Выберите **Switch to PayloadLoader**
1. После завершения установки нажмите {% include inc/btn.md btn="A" %}, чтобы выключить консоль
1. Теперь **PayloadLoader** будет автоматически запускаться при каждой загрузке консоли
  * Для того, чтобы изменить приложение, которое будет загружаться по-умолчанию, нажмите и удерживайте {% include inc/btn.md btn="+" %} на геймпаде во время загрузки приставки. Выберите нужный тайтл, нажав {% include inc/btn.md btn="Y" %}

## Часть IV - Автозапуск Tiramisu

1. Выключите и включите консоль. Должен запуститься "**Environment Loader**"
1. С помощью крестовины выберите **tiramisu** и нажмите {% include inc/btn.md btn="Y" %}, чтобы запускать Tiramisu при старте приставки
  * Для открытия **Environment Loader**, нажмите {% include inc/btn.md btn="X" %} при загрузке приставки
1. В меню Tiramisu **Boot Selector** наведите курсор на **"Wii U Menu"** и нажмите {% include inc/btn.md btn="Y" %}, чтобы запускать главное меню при запуске консоли
  * Для открытия Tiramisu **Boot Selector**, нажмите {% include inc/btn.md btn="+" %} при загрузке приставки

После загрузки в **Tiramisu** вы можете запустить **Homebrew Launcher** через приложение **Редактор Mii** (**Mii Maker**). Чтобы запустить сам **Редактор Mii** (**Mii Maker**), просто нажмите {% include inc/btn.md btn="HOME" %} в **Homebrew Launcher**
{: .notice--info}


___

Для того, чтобы научиться устанавливать игры, перейдите [сюда](games)
{: .notice--success}

Для информации о модификации vWii, перейдите к странице [Модификация vWii](vwii-modding).
{: .notice--success}