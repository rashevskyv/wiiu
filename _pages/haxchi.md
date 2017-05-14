---
title: "Haxchi" #
lang: ru
permalink: /haxchi.html
---

Haxchi - это кастомная прошивка, которая патчит проверку подписи, проверку региона и запускает различный пользовательский код на фоне работающей прошивки.
{: .notice}

Haxchi - это эксплойт, который позволяет нам запускать CFW напрямую из системного меню без использования Homebrew Launcher.
{: .notice--info}

Если вам необходимо купить одну из игр, в которую будет внедрен эксплойт, запустите NNU-Patcher из Homebrew Launcher, после чего купите игру через eShop. После покупки игры, заново войдите в [Homebrew Launcher](homebrew-launcher).
{: .notice--primary}

#### <a name="what_need" />Что понадобится

+ Купленная копия одной из указанных игр из DS virtual console, установленная во внутреннюю память Wii U
  + **Не** устанавливайте игру от DS virtual console на USB-носитель
  + На данный момент, самая дешевая подходящая игра в eShop - Brain Age ($6.99 USD)
  + Если у вас есть купленная установленная копия Brain Age / Brain Trainin на вашей приставке, удалите ее и переустановите из eShop. Старая версия игры не заработает с Haxchi
  + После окончания процесса установки, в игру невозможно будет сыграть
  **Ваша игра от DS virtual console, используемая для Haxchi, ДОЛЖНА быть ЛЕГАЛЬНОЙ копией!**

<a name="games" />| Игры, совместимые с Haxchi|
| ------------- |
| ------------- |
| Animal Crossing: Wild World |
| Big Brain Training |
| DK: Jungle Climber |
| Dr. Kawashima's Brain Training |
| Kirby: Canvas Curse |
| Kirby: Mass Attack|
| Kirby: Squeak Squad / Kirby: Mouse Attack |
| Legend of Zelda: Phantom Hourglass, The |
| Legend of Zelda: Spirit Tracks, The |
| Mario & Luigi: Partners in Time |
| Mario Kart DS |
| New Super Mario Bros. |
| Pokemon Mystery Dungeon: Explorers of the Sky |
| Pokemon Ranger |
| Pokemon Ranger: Guardian Signs | 
| Pokemon Ranger: Shadows of Almia |
| Starfox Command |
| Super Mario 64 DS |
| Wario: Master of Disguise |
| WarioWare: Touched |
| Yoshi's Island DS |
| Yoshi's Touch & Go |

#### <a name="instructions" />Инструкция

1. Запустите инсталлятор Haxchi
1. Выберите игру от DS virtual console, в которую вы собираетесь установить Haxchi, а затем нажмите (A) для подтверждения
1. Ознакомьтесь с появившимся предупреждением и нажмите (A) для установки
1. После окончания процесса, запустите вашу игру от DS virtual console (будет называться "Haxchi")
1. Приставка перезагрузится в пропатченный SysNAND
  + Вы сможете запускать неподписанные приложения (например homebrew channel или резервные копии игр) прямо из системного меню

___

В данный момент для загрузки пропатченного SysNAND вам каждый раз будет нужно запускать Haxchi через игру для DS virtual console. На следующей странице мы установим CBHC (Coldboot Haxchi), который автоматизирует этот процесс.
{: .notice}

{% capture notice-1 %}
**Вы можете удерживать различные кнопки при запуске игры от DS virtual console для выбора загружаемой программы. Ниже краткое описание каждого из пунктов:**

    + None -> загрузка в пропатченный SysNAND
    + (A) -> Загрузка в Homebrew Launcher

{% endcapture %}

<div class="notice--info">{{ notice-1 | markdownify }}</div>

Следующий шаг: [Coldboot Haxchi](coldboot-haxchi).
{: .notice--primary}
