---
title: "Установка Aroma" #
lang: ru
permalink: /aroma.html
author_profile: true
---

{% include toc title="Разделы" %}

**Aroma** - Арома — это среда, которую можно загрузить с помощью Environment Loader. Подобно Тирамису, Арома использует ту же версию Mocha, поддерживает модули настройки, автозагрузку и быстрый запуск. Арома также предлагает несколько дополнительных функций, среди которых система плагинов, новый способ запуска homebrew-приложений, а также множество встроенных модулей и плагинов.

Убедитесь, что не пропустили [подготовительные этапы](get-started){:target="_blank"}!
{: .notice--warning}

## Часть I - Установка PayloadLoader

{% include inc/hbl.md btn="X" env="меню **Environment Loader**" %}
1. С помощью крестовины выберите **aroma** и запустите её кнопкой {% include inc/btn.md btn="A" %}
1. Появится желтый экран с предложением заблокировать обновление консоли. Нажмите {% include inc/btn.md btn="X" %}, чтобы продолжить. 
  * Приставка запустится на главный экран Wii U на котором появятся homebrew-приложения
1. Запустите **Payload-Loader Installer** (![](/images/apps/payload-loader.png){:width="60px"})
1. Выберите **Check**, чтобы проверить можно ли установить **PayloadLoader** в приложение **"Информация о здоровье и безопасности"** (**"Health and Safety Information"**) - ![](/images/apps/hs.png){:width="60px"}
1. Выберите **Install / Update** кнопкой {% include inc/btn.md btn="A" %}
1. С помощью крестовины выберите **Install** и запустите установку кнопкой {% include inc/btn.md btn="A" %} 
1. Выберите "**Press A to shutdown**", чтобы выключить консоль

## Часть II - Автозапуск PayloadLoader

1. Включите консоль
1. Запустите приложение **"Информация о здоровье и безопасности"** (**"Health and Safety Information"**) - ![](/images/apps/hs.png){:width="60px"} -  из главного меню вашей консоли
1. Запустите **Payload-Loader Installer** (![](/images/apps/payload-loader.png){:width="60px"})
1. Выберите **Check** -> **Boot options**
1. Выберите **Switch to PayloadLoader**
1. После завершения установки нажмите {% include inc/btn.md btn="A" %}, чтобы выключить консоль
  * Теперь **PayloadLoader** будет автоматически запускаться при каждой загрузке консоли
1. Выберите "**Press A to shutdown**", чтобы выключить консоль

### Homebrew 

Aroma не поддерживает старые Homebrew, написанные для запуска через Homebrew Launcher. Новые приложения должны быть написаны с поддержкой Aroma и быть в формате `.wuhb`. Скачанное приложение следует поместить в папку `wiiu\apps` на карте памяти. После этого оно появится на главном экране Wii U 

### Pretendo

[Pretendo](https://pretendo.network/){:target="_blank"} - проект с открытым исходным кодом, цель которого воссоздать Nintendo Network для консолей 3DS и Wii U, используя обратную-разработку (reverse engineering).

В данный момент всё настроено для полной совместимости с сервисом и не требует дополнительных манипуляций. Можете подключиться к Pretendo так, как вы бы делали это в случае с сервисами Nintendo 

Надпись **Using Pretendo Network** на экране при старте приставки говорит о том, что вы подключены к сервису.

### Горячие клавиши

При запуске приставки вы можете зажать одну из указанных горячих клавиш, чтобы запустить системные приложения:

* **Enviroment Loader** (удерживайте {% include inc/btn.md btn="X" %} для запуска) - позволяет запускать другие окружения, вместо aroma, а так же удалить эксплойт (через меню **installer**). Все окружения находятся по пути `sd:\wiiu\environments\%enviroment_name%\modules\setup\`. Обратите внимание, что при выборе окружения, будут запущены все модули в папке `setup` в порядке их наименования. Подробнее по [ссылке](https://gbatemp.net/threads/release-environment-loader.605382/){:target="_blank"}
* **Boot Selector** (удерживайте {% include inc/btn.md btn="+" %} для запуска) - позволяет выбрать что именно будет грузиться. По умолчанию, идёт загрузка в **главное меню Wii U** (Wii U Menu), та же для выбора доступна загрузка в **главное меню Wii** (vWii System Menu)
* **Payload Loader** (удерживайте {% include inc/btn.md btn="B" %} для запуска) - позволяет выбрать пейлоад, который будет загружен в приставку. По-умолчанию будет грузиться Enviroment Loader (default). Свои пейлоады можно положить на карту памяти по пути `sd:\wiiu\payloads\`

Обратите внимание, взлом находится на карте памяти. При запуске приставки без карты памяти, или без файлов взлома, приставка просто загрузится в главное меню, как будто она не прошита. Некоторые игры, с правильными тикетами продолжат работу, а некоторые, например, Virtual Console и форвардеры - нет.
{: .notice--warning}

### Запуск старого Homebrew в формате .elf 

1. Положите необходимое Homebrew в папку `wiiu/apps` 
1. Запустите приставку, удерживая кнопку {% include inc/btn.md btn="X" %}
1. В появившемся меню выберите **tiramisu**
1. В появившемся меню выберите **Homebrew Launcher**
  1. Вы можете загрузиться в Wii U Menu при необходимости, и выбрать **Редактор Mii (Mii Maker)**, чтобы попасть в **Homebrew Launcher** 
1. Запустите необходимое Homebrew ``

___

Для того, чтобы научиться устанавливать игры, перейдите [сюда](games)
{: .notice--success}

Информация о смене региона и русификации Wii U  и Wii [тут](wiiu-region-change)
{: .notice--success}

Для информации о модификации vWii, перейдите к странице [Модификация vWii](vwii-modding)
{: .notice--success}