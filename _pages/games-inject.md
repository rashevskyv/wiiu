---
title: "Запуск игр из других платформ с помощью встроенного эмулятора"
lang: ru
permalink: games-inject.html
author_profile: true
---

{% include toc title="Разделы" %}

## Установка игры для Wii в виде инжектов

Вы можете самостоятельно сконвертировать многие Wii игры в формат, устанавливаемый через WUPInstaller. Игры, установленные таким образом будут запускаться через главное меню самой WiiU. То есть, для их запуска не нужно будет переходить в режим vWii. Такие игры устанавливаются либо во внутреннюю память WiiU, либо на внешний USB-носитель
{: .notice--info}

### Часть I - Подготовительные работы

1. Распакуйте [WiiVC Injector Script](https://gbatemp.net/threads/release-wiivc-injector-script-gc-wii-homebrew-support.483577/){:target="_blank"} в удобное место на вашем диске и запустите его
1. Программа попросит установить **.NET Framework 3.5**, если он не был установлен и откроет окно Панели Управления "**Программы и компоненты**"
   1. Перейдите в "**Включение или отключение компонентов Windows**"
   1. Отметьте галочкой "**.NET Framework 3.5**" и нажмите **ОК**
   1. Разрешите Windows скачать необходимые файлы и дождитесь окончания установки, после чего перезапустите программу
1. В программе перейдите во вкладку "**Build Title**"
   1. В поле "**Wii U Common Key**" введите `D7B00402659BA2ABD2CB0DB27FA2B656` и нажмите **Save Key**
   1. В поле "**Rythm Heaven Fever [USA] Title Key**" введите `04EACEF7657422E61606FA7FC7DCD73D` и нажмите **Save Key**
1. Перезапустите программу

### Часть II - Использование [WiiVC Injector Script](https://gbatemp.net/threads/release-wiivc-injector-script-gc-wii-homebrew-support.483577/){:target="_blank"}

1. В верхней части программы галочками отмечаются режимы работы программы. Нас интересуют два:
   * **Wii Retail Injection** - позволяет инжектить игры от Wii
   * **GC Retail Injection** - позволяет инжектить игры от GameCube
1. Выберите режим, в соответствии с консолью, игру для которой вы хотите установить
1. Перейдите во вкладку "**Required Source Files**" и нажмите на кнопку "**Game**"
1. Выберите игру от Wii или GameCube в зависимости от выбранного режима
1. Нажмите кнопку "**Download images from cucholix's repo**", чтобы скачать иконки выбранной игры
1. Перейдите во вкладку "**Gamepad / Meta Options**"
   * В этом меню можно выбрать опции эмуляции контроллера, например заставить некоторые игры работать с контроллером WiiU, вместо контроллера от Wii. Эти настройки индивидуальны для каждой игры и выставляются экспериментально. Если у вас есть контроллеры от Wii, рекомендую просто использовать их. 
1. Перейдите во вкладку "**Build Title**" и нажмите кнопку "**BUILD**"
1. Выберите в какую папку будет собран образ 
   * Можете указать в качестве папки сразу папку "**install**" на вашей карте памяти 
1. Перенесите созданную папку с игрой (будет находится в выбранной ранее папке) на карту памяти в папку `install` и [установите игру через WUP Installer](games-wiiu)

<!--С помощью этого метода можно запускать желаемые игры через встроенный в Wii U эмулятор других консолей. Метод работает с играми от Wii, NDS, SNES, NES, N64 и GBA. *Для простоты процесс создания таких игр мы будем называть "инжект", либо "внедрение".* Внедрение будет производится с помощью программы **Ultimate VC Injector for WiiU** (UVCW). 

SNES-игры, использующие технологию SuperFX не поддерживаются. Используйте сторонний эмулятор для их запуска

Игры DSi-enchanced не поддерживаются.

## Что понадобится
* Скачайте последнюю версию Ultimate VC Injector for WiiU по ссылке `Download v1 C#` в [этой теме](https://gbatemp.net/threads/release-ultimate-vc-injector-for-wiiu.486781/){:target="_blank"}
* Образ (ром) игры, которую вы будете инжектить
* [Title Key](http://wiiu.titlekeys.gq/){:target="_blank"}
* [Wii U common key](key){:target="_blank"}

## Ultimate WiiU VC Injector

1. Запустите Ultimate WiiU VC Injector.exe
1. Выберите консоль для которой хотите сделать инжект нажав соответствующую кнопку: 

	* [NDS VC Injector](games-inject#nds-vc-injector)
	* [N64 VC Injector](games-inject#n64-vc-injector)
	* [NES VC Injector](games-inject#nes-vc-injector)
	* [GBA VC Injector](games-inject#gba-vc-injector)
	* [SNES VC Injector](games-inject#snes-vc-injector)
	* [Wii VC Injector](games-inject#wii-vc-injector)

### NDS VC Injector

1. Выберите один из вариантов в зависимости от региона вашей приставки 
1. В поле "Wii U CommonKey" введите ключ, обозначенный [здесь](key){:target="_blank"} и нажмите "Check"
1. В поле "WarioWare Touched!" введите Title ID игры, который можно найти на [этом сайте](http://wiiu.titlekeys.gq/){:target="_blank"} и нажмите "Check"
1. 

 ### N64 VC Injector


### NES VC Injector


### GBA VC Injector


### SNES VC Injector


### Wii VC Injector-->