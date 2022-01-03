---
title: "Haxchi" #
lang: ru
permalink: /haxchi.html
author_profile: true
---

{% include toc title="Разделы" %}

**Haxchi** - это эксплойт, который позволяет нам запускать CFW напрямую из системного меню без использования Homebrew Launcher. Он включает в себя кастомную прошивку, которая патчит проверку подписи, проверку региона и запускает различный пользовательский код на фоне работающей прошивки.

Так же на базе **Haxchi** можно заставить взлом запускаться автоматически при запуске приставки. 

Для использования **Haxchi** нужно будет внедрить эксплойт в официально купленную игру от Nintendo DS! 

## Инструкция

### Часть I - Игры DS Virtual Console

Игра для DS Virtual Console должна быть **законно приобретённой** и установленной во **внутреннюю память** приставки. **Не** устанавливайте игру от DS virtual console на USB-носитель. 
{: .notice--warning}

#### Регистрация аккаунта и NNID 

Если у вас есть уже на аккаунте одна из игр, указанных в списке совместимости ниже, удалите её и скачайте заново, а затем сразу переходите к [установке Haxchi](#часть-ii---установка-haxchi). Проверьте наличие купленной игры в eShop, даже если у вас новый, только что созданный аккаунт, поскольку в редких случаях эти игры могут раздаваться бесплатно, тогда они будут отображаться в eShop как купленные.

+ Если при запускеe Shop у вас возникает ошибка 105-5602:
   1. Зайдите в **Системные настройки**, **Информация о консоли**, **Выбор страны проживания** и измените страну на "**Германия**", подтвердите выбор нажатием кнопки "**Изменить**"
   1. Перезагрузите приставку 
   1. Запустите **eShop** (снова будет ошибка)
   1. Зайдите в **Системные настройки**, **Информация о консоли**, **Выбор страны проживания** и измените страну на ту, что была до этого, подтвердите выбор нажатием кнопки "**Изменить**"
   1. Перезагрузите приставку 
   1. Запустите **eShop**, теперь он должен работать

Если таковой на аккаунте нет нужной игры, **создайте новую учётную запись на вашей консоли и добавить новый NNID**:

Записывайте все данные, которые вводите при создании аккаунта!
{: .notice--warning}

1. Нажмите на аватарку в левой верхней части окна и выберите "**Поменять пользователя**" (Change user)
1. Нажмите "**Добавить нового пользователя**" в верхней правой части экрана и следуйте указаниям на экране. 
1. Назовите этот аккаунт "**HAXCHI**", чтобы не запутаться. 
1. Укажите **Россию** в качестве страны проживания, если ваша консоль PAL-региона и **США**, если консоль NTSC-региона 
1. **Обязательно** разрешите **доступ к коду Nintendo Network с компьютеров и других устройств**! Если вы не сделаете этого, то не сможете добавить ваучер на аккаунт простым способом! За это будет отвечать одна из настроек в процессе создания аккаунта!

Теперь необходимо создать новый Nintendo Account: 

NNID и Nintendo Account не одно и тоже, хотя казалось бы
{: .notice--info}

1. Перейдите на [сайт Nintendo](https://accounts.nintendo.com/authorize_age_gate?redirect_after=5&redirect_uri=https%3A%2F%2Faccounts.nintendo.com%2F){:target="_blank"} и создайте аккаунт, заполнив все необходимые поля
1. После того, как вы войдёте в созданный аккаунт на ПК, нажмите **Edit** возле **Linked accounts** и выберите **Nintendo Network ID**
1. Войдите в ваш NNID и привяжите его к аккаунту

#### Список совместимый DS Virtual Console игр

Если у вас уже куплена одни из игр из списка ниже, скачайте её на свою приставку и переходите к следующей части
{: .notice--warning}

Если у вас не получается скачать игру на самой приставке, купите игру через сайт!
{: .notice--warning}

| ------------- | ----- | ----- | ----- |
| Animal Crossing: Wild World | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Animal-Crossing-Wild-World-270011.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/animal-crossing-wild-world-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000023019){:target="_blank"} |
| Big Brain Academy | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Big-Brain-Academy-270143.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/big-brain-academy-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000013967){:target="_blank"} |
| Brain Age: Train Your Brain in Minutes a Day! | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Dr-Kawashima-s-Brain-Training-How-Old-is-Your-Brain--270627.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/brain-age-train-your-brain-in-minutes-a-day-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000006826){:target="_blank"} |
| Donkey Kong: Jungle Climber | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Donkey-Kong-Jungle-Climber-270506.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/dk-jungle-climber-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000014168){:target="_blank"} |
| Dr. Kawashima’s Brain Training: How Old is Your Brain? | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Dr-Kawashima-s-Brain-Training-How-Old-is-Your-Brain--270627.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/brain-age-train-your-brain-in-minutes-a-day-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000006826){:target="_blank"} |
| Kirby: Canvas Curse / Kirby: Power Paintbrush | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Kirby-Power-Paintbrush-271287.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/kirby-canvas-curse-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000015447){:target="_blank"} |
| Kirby: Mass Attack | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Kirby-Mass-Attack-271265.html#Overview){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/kirby-mass-attack-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000017169){:target="_blank"} |
| Kirby: Squeak Squad / Kirby: Mouse Attack | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Kirby-Mouse-Attack-271276.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/kirby-squeak-squad-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000014167){:target="_blank"} |
| The Legend of Zelda: Phantom Hourglass | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/The-Legend-of-Zelda-Phantom-Hourglass-273289.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/the-legend-of-zelda-phantom-hourglass-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000017170){:target="_blank"} |
| The Legend of Zelda: Spirit Tracks | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/The-Legend-of-Zelda-Spirit-Tracks-273300.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/the-legend-of-zelda-spirit-tracks-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000017168){:target="_blank"} |
| Mario & Luigi: Partners in Time | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Mario-Luigi-Partners-in-Time-271595.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/mario-luigi-partners-in-time-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000013367){:target="_blank"} |
| Mario Kart DS | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Mario-Kart-DS-271518.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/mario-kart-ds-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000011949){:target="_blank"} |
| New Super Mario Bros. | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/New-Super-Mario-Bros--271969.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/new-super-mario-bros-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000011947){:target="_blank"} |
| Pokemon Mystery Dungeon: Explorers of the Sky | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Pokemon-Mystery-Dungeon-Explorers-of-Sky-272409.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/pokemon-mystery-dungeon-explorers-of-sky-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000023018){:target="_blank"} |
| Star Fox Command | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Star-Fox-Command-273113.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/star-fox-command-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000014227){:target="_blank"} |
| Super Mario 64 DS | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Super-Mario-64-DS-273179.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/super-mario-64-ds-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000015449){:target="_blank"} |
| Wario: Master of Disguise | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Wario-Master-of-Disguise-273553.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/wario-master-of-disguise-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000014228){:target="_blank"} |
| WarioWare: Touched! | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/WarioWare-Touched--273564.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/warioware-touched-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000013308){:target="_blank"} |
| Yoshi’s Island DS | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Yoshi-s-Island-DS-273630.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/yoshis-island-ds-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000013369){:target="_blank"} |
| Yoshi Touch & Go | [EUR](https://www.nintendo.eu/Games/Nintendo-DS/Yoshi-Touch-Go-273641.html){:target="_blank"} | [USA](https://www.nintendo.com/games/detail/yoshi-touch-go-wii-u/){:target="_blank"} | [JPN](https://www.nintendo.co.jp/titles/20010000006827){:target="_blank"} |

* Отключите все USB-носители от приставки, иначе игра будет установлена на них, а нам она нужна во внутренней памяти приставки
* Если ваша приставка американка или японка, то вы можете купить игру прямо через eShop на самой приставке. Если при покупке магазин отказывается работать с вашей картой, то вам придется купить [$10 Nintendo eShop Gift Card](https://www.amazon.com/gp/product/B01LZNGPY3/ref=ppx_yo_dt_b_d_asin_title_o00?ie=UTF8&psc=1){:target="_blank"}, а затем использовать добавить её на приставке.
* Игру в Европе можно купить **только** добавив деньги на ваш аккаунт: 
   1. На ПК запустите браузер и перейдите в [eShop](https://www.nintendo.ru/-/Nintendo-eShop/Nintendo-eShop-1806894.html){:target="_blank"}
   1. Залогиньтесь под вашим аккаунтом с помощью **Кода Nintendo Network**, который привязан к вашей приставке 
|   * Если вы не можете получить доступ к NNID с ПК, измените настройку "**доступ с компьютеров и других устройств**" в разделе "**Настройка пользователя**", который находится в меню, вызываемом по нажатию на аватарку на главном экране
|   * Подробнее об этой процедуре можно прочитать [здесь](https://www.nintendo.ru/-/Nintendo-2DS-Nintendo-3DS/-/Nintendo-eShop/-Nintendo-eShop--1626660.html){:target="_blank"}
   1. Перейдите на страницу [пополнения баланса](https://ec.nintendo.com/my/balance_add){:target="_blank"} и введите пароль от вашей учетной записи
   1. Выберите способ пополнения баланса и положите минимальное количество денег на свой счёт (для России - 750 рублей)
   1. После того, как деньги будут добавлены, вам нужно объединить вашу учетную запись и ваш NNID. Для этого перейдите в [меню магазина](https://ec.nintendo.com/my/#/){:target="_blank"}
   1. Нажмите на ссылку "**Объединить средства**", которая будет располагаться внизу справа, под методами оплаты
   1. После того, как вы объедините средства, вы можете перейти в eShop, в раздел **Nintendo DS** на вашей консоли и наконец купить игру **Dr. Kawashima's Brain Training**
* Если ваша игра после покупки не начала качаться автоматически, зайдите в eShop на приставке, найдите список купленных игр и установите игру принудительно 
* Используйте приложение Google Translate и перевод через камеру на вашем смартфоне, если интерфейс приставки на незнакомом для вас языке 

После взлома можете создавать и использовать другие аккаунты, если это необходимо. Главное не удаляйте тот, из которого была куплена игра, в которую установлен Haxchi!
{: .notice--danger}

### Часть II - Запуск Homebrew Launcher

{% include inc/hbl.md %}

### Часть III - Установка Haxchi

1. Запустите инсталлятор **Haxchi**
1. Выберите игру от DS virtual console, в которую вы собираетесь установить Haxchi, а затем нажмите {% include inc/btn.md btn="A" %} для подтверждения
1. Ознакомьтесь с появившимся предупреждением и нажмите {% include inc/btn.md btn="A" %} для установки
1. После окончания процесса, игра, в которую вы установили **Haxchi** сменит название и иконку и будет запускать по-умолчанию **HaxchiCFW**
  + Вы сможете запускать неподписанные приложения (например Homebrew Channel или резервные копии игр) прямо из системного меню

___

В данный момент для запуска CFW вам каждый раз будет нужно запускать *Haxchi* из главного меню приставки. На следующей странице мы установим **CBHC (Coldboot Haxchi)**, который автоматизирует этот процесс.
{: .notice--info}

Вы можете удерживать кнопку {% include inc/btn.md btn="A" %} после запуска **Haxchi**, чтобы попасть в **Homebrew Launcher**
{: .notice--info}

___

## Дальнейшие действия

### [Остаться на Haxchi](homebrew-launcher-channel)

На вашей приставке уже установлен эксплойт Haxchi.

Использование этого метода не несёт в себе никаких рисков, но каждый раз после перезагрузки вам придётся активировать взлом вручную, запукская **Haxchi** с главного экрана приставки

___

### [Установка Coldboot Haxchi](coldboot-haxchi)

**CBHC (Coldboot Haxchi)** изменяет системный тайл, запускающийся по-умолчанию при старте SysNAND, на игру из DS virtual console, которая настроена на запуск CFW, что позволяет запускать кастом сразу при загрузке приставки.

Использование этого эксплойта менее безопасно, поскольку единственный способ запустить систему - использовать специально подготовленную игру от DS. Удалив или переместив эту игру вы не сможете загрузить приставку! Поэтому, используя этот метод, нужно будет соблюдать ряд простых правил безопасности, о чем будет написано далее.