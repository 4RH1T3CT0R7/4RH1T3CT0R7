```
  ARTEM LYTKIN
  ============
  $ whoami
  software engineering student, BMSTU, Moscow
```

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Lua](https://img.shields.io/badge/Lua-2C2D72?style=flat-square&logo=lua&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

I am a software engineering student at Bauman Moscow State Technical University.

Most of what I do falls into two piles. One is ordinary systems work: a contest
platform in Go that ran live tournaments for my university, and eleven patches
merged into the Linux staging tree. The other is finding out what a system can be
talked into doing when nobody designed it for that, which is how DOOM ended up
running on regex substitutions and a raycaster ended up inside a font file.

I also translate games into Russian in my spare time, which turns out to be a
surprisingly good way to learn how other people build software.

## Projects

<table>
<tr>
<td width="50%" valign="top">

### [doom-regex](https://github.com/4RH1T3CT0R7/doom-regex)

[![stars](https://img.shields.io/github/stars/4RH1T3CT0R7/doom-regex?style=flat-square&logo=github&logoColor=white&label=stars&labelColor=21262d&color=e3b341)](https://github.com/4RH1T3CT0R7/doom-regex/stargazers)

<img src="https://raw.githubusercontent.com/4RH1T3CT0R7/doom-regex/main/docs/doom_regex_clip.gif" width="100%">

DOOM running on nothing but regex find-and-replace. One 96 MB string, 544 rules,
byte-identical to native DOOM. Turns out PCRE2 substitution is enough to be a
computer, if you are patient.

</td>
<td width="50%" valign="top">

### [ttf-doom](https://github.com/4RH1T3CT0R7/ttf-doom)

[![stars](https://img.shields.io/github/stars/4RH1T3CT0R7/ttf-doom?style=flat-square&logo=github&logoColor=white&label=stars&labelColor=21262d&color=e3b341)](https://github.com/4RH1T3CT0R7/ttf-doom/stargazers)

<img src="https://raw.githubusercontent.com/4RH1T3CT0R7/ttf-doom/main/docs/media/demo.gif" width="100%">

A 3D raycaster living inside a TrueType font's hinting virtual machine. I wrote a
small compiler from a C-like DSL down to TrueType bytecode, and the glyph does the
rendering. The whole engine is 6.5 KB.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [balatro-port-tui](https://github.com/4RH1T3CT0R7/balatro-port-tui)

[![stars](https://img.shields.io/github/stars/4RH1T3CT0R7/balatro-port-tui?style=flat-square&logo=github&logoColor=white&label=stars&labelColor=21262d&color=e3b341)](https://github.com/4RH1T3CT0R7/balatro-port-tui/stargazers)

<img src="https://raw.githubusercontent.com/4RH1T3CT0R7/balatro-port-tui/main/assets/demo.gif" width="100%">

Balatro in your terminal, running the game's original Lua with no modifications.
It is a reimplementation of the LOVE2D engine in Rust, with a software rasteriser
and nine shaders emulated on the CPU.

</td>
<td width="50%" valign="top">

### [TJudge](https://github.com/4RH1T3CT0R7/TJudge)

[![stars](https://img.shields.io/github/stars/4RH1T3CT0R7/TJudge?style=flat-square&logo=github&logoColor=white&label=stars&labelColor=21262d&color=e3b341)](https://github.com/4RH1T3CT0R7/TJudge/stargazers)

<img src="https://raw.githubusercontent.com/4RH1T3CT0R7/4RH1T3CT0R7/main/assets/tjudge-demo.gif" width="100%">

A tournament platform for game theory contests, used in production at Bauman Code
Games. Go and React, matches executed in isolated Docker containers, ELO ratings,
live standings over WebSocket.

</td>
</tr>
</table>

## Merged upstream

| Project | What I changed |
| --- | --- |
| [![Linux](https://img.shields.io/badge/Linux_kernel-FCC624?style=flat-square&logo=linux&logoColor=black)](https://github.com/search?q=repo%3Atorvalds%2Flinux+author%3A4RH1T3CT0R7&type=commits) | Eleven patches in `drivers/staging`, across `most/dim2`, `sm750fb`, `nvec`, `fbtft` and `media/av7110`. Error path fixes, device-based logging, replacing `BUG()` with proper error returns |
| [![GitHub CLI](https://img.shields.io/badge/GitHub_CLI-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/cli/cli/pull/12686) | Added a `--no-upstream` flag to `gh repo clone` |
| [![Docker](https://img.shields.io/badge/Docker_CLI-2496ED?style=flat-square&logo=docker&logoColor=white)](https://github.com/docker/cli/pull/6800) | Made `docker cp` report both content size and transferred size |
| [![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)](https://github.com/grafana/grafana/pull/118156) | Fixed the active tab indicator on custom datasource config pages |
| [![Superset](https://img.shields.io/badge/Apache_Superset-20A6C9?style=flat-square&logo=apachesuperset&logoColor=white)](https://github.com/apache/superset/pull/37980) | Kept percentage formatting intact for small numbers in tables |
| [![Docusaurus](https://img.shields.io/badge/Docusaurus-3ECC5F?style=flat-square&logo=docusaurus&logoColor=white)](https://github.com/facebook/docusaurus/pull/11743) | Used the category key for generated-index translation lookup |
| [![Telegram](https://img.shields.io/badge/Telegram_Desktop-26A5E4?style=flat-square&logo=telegram&logoColor=white)](https://github.com/telegramdesktop/tdesktop/pull/30179) | Restored the expandable quote button in the caption field |
| [![Windows Terminal](https://img.shields.io/badge/Windows_Terminal-4D4D4D?style=flat-square&logo=windowsterminal&logoColor=white)](https://github.com/microsoft/terminal/pull/19931) | Focused the terminal on click-drag while search is open |
| [![PowerToys](https://img.shields.io/badge/PowerToys-0078D4?style=flat-square&logo=microsoft&logoColor=white)](https://github.com/microsoft/PowerToys/pull/50093) | Fixed Screen Ruler's edge detection at the screen edge and an overflow in its bounds-mode colour comparison |
| [![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi_Imager-A22846?style=flat-square&logo=raspberrypi&logoColor=white)](https://github.com/raspberrypi/rpi-imager/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Seven fixes, mostly around polkit on immutable distros, stale WiFi settings, file dialogs, the localisation grid and a fallback chime for Linux |
| [![Bambu Lab](https://img.shields.io/badge/Bambu_Studio-00AE42?style=flat-square&logo=bambulab&logoColor=white)](https://github.com/bambulab/BambuStudio/pull/9664) | Fixed window drag lag on Windows |
| [![Flipper](https://img.shields.io/badge/Flipper_One-FF8200?style=flat-square&logo=flipper&logoColor=white)](https://github.com/flipperdevices/flipperone-mcu-firmware/pull/70) | Wrote the build and firmware update documentation |
| [![bitchat](https://img.shields.io/badge/bitchat-000000?style=flat-square&logo=bluetooth&logoColor=white)](https://github.com/permissionlesstech/bitchat/pull/1069) | Fixed a crash when opening a private message a second time |
| [![PPSSPP](https://img.shields.io/badge/PPSSPP-5B6DCD?style=flat-square)](https://github.com/hrydgard/ppsspp/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Four fixes: the Win32 debugger's breakpoint list refreshes after memcheck changes, its VFPU register view shows values and scrolls, the folder buttons open again on Linux, and the save dialog takes a save's date from PARAM.SFO |
| [![Gitea](https://img.shields.io/badge/Gitea-609926?style=flat-square&logo=gitea&logoColor=white)](https://github.com/go-gitea/gitea/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Three fixes: OpenPGP signatures are no longer verified against an SSH instance key, default compare links name the head repository, and co-author trailers that are not RFC 5322 addresses are parsed |
| [![Fyne](https://img.shields.io/badge/Fyne-1A9FD9?style=flat-square)](https://github.com/fyne-io/fyne/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Four fixes: a nil panic when a file dialog is sized before `Show()`, rasters drawn from the top left of their bounds, submenus taller than the window now scroll, and widgets behind an inner window no longer set the cursor |
| [![CircuitPython](https://img.shields.io/badge/CircuitPython-7B3FE4?style=flat-square&logo=adafruit&logoColor=white)](https://github.com/adafruit/circuitpython/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Three fixes: `TimeAlarm` validates its epoch time, `WaveFile` pads 8-bit samples correctly at the end of a file, and the unix port builds on arm64 |
| [![Wails](https://img.shields.io/badge/Wails-D32F2F?style=flat-square)](https://github.com/wailsapp/wails/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Plugged a `Calloc` leak in the v2 Linux and macOS frontends, and dropped the precompiled example binaries from v3 |
| [![Space Station 14](https://img.shields.io/badge/Space_Station_14-1C6EA4?style=flat-square)](https://github.com/space-wizards/space-station-14/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Defibrillators no longer report on whatever else the patient is strapped to, and the Crewsimov law board is called Crewsimov internally too |
| [![Flameshot](https://img.shields.io/badge/Flameshot-009688?style=flat-square)](https://github.com/flameshot-org/flameshot/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Fixed the pin size on scaled Windows screens, and added a same-language fallback for locales without their own translation |
| [![RetroArch](https://img.shields.io/badge/RetroArch-000000?style=flat-square)](https://github.com/libretro/RetroArch/pull/19584) | Restored the widget scale override range on console and mobile builds |
| [![micro](https://img.shields.io/badge/micro-2E3440?style=flat-square)](https://github.com/micro-editor/micro/pull/4179) | Made the linter plugin compare paths with `filepath.Base()`, so linter messages stop being dropped |
| [![hashcat](https://img.shields.io/badge/hashcat-111111?style=flat-square)](https://github.com/hashcat/hashcat/pull/4617) | Fixed the salt length reported by hash mode 3710 with the optimized kernel |
| [![Throne](https://img.shields.io/badge/Throne-1A73E8?style=flat-square&logo=v2fly&logoColor=white)](https://github.com/throneproj/Throne/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Six fixes: a core crash on Remove Invalid, the system proxy clearing itself on exit, stale results from a finished latency sweep, screen-reader names in the hotkey, routing and profile dialogs, and a routing dialog that grew as wide as the longest profile name |
| [![Millennium Dawn](https://img.shields.io/badge/Millennium_Dawn-8B0000?style=flat-square)](https://github.com/MillenniumDawn/Millennium-Dawn/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | 66 merged pull requests in this Hearts of Iron IV mod: the intelligence agency system, several economy exploits, AI behaviour and a number of national focus trees |

Across all of this I have opened pull requests against 52 projects that are not
mine. Another 57 of them are still open, in 33 projects including Kubernetes,
VS Code, Moby, Ollama, Next.js, TensorFlow, Supabase, Tailscale, OBS Studio,
Notepad++ and both Arduino IDEs.

## Russian game localizations

Four games that never got an official Russian release, or got a bad one.

- **[Suzerain](https://steamcommunity.com/sharedfiles/filedetails/?id=2908967542)**
  is the big one. Published in December 2022 and still updated today, with 11k
  readers and 693 people keeping it in their favourites. Done with a team of
  translators over about three years.
- **[Night Call](https://github.com/4RH1T3CT0R7/russian-localisation-night-call)**
  covers 5,371 dialogue passages, 789 interface keys and every passenger name,
  through a BepInEx plugin with generated Cyrillic SDF atlases.
- **[Interrogation](https://github.com/4RH1T3CT0R7/interrogation-russian-translation)**
  covers all 60 localization files and 30 or so interrogations, plus 23 Cyrillic
  fonts including the system one.
- **[Not Tonight](https://github.com/4RH1T3CT0R7/not-tonight-russian)** covers the
  base game and the One Love DLC, roughly 8,000 keys.

## Stack

```
languages    Go, Python, Rust, C, C#, Lua
backend      PostgreSQL, Redis, Chi, REST, WebSocket, gRPC
infra        Docker, Prometheus, Grafana, Loki, Linux
ml           TensorFlow, PyTorch
low level    TrueType hinting VM, Lua VM, Sixel, terminal rendering
```

## Background

Studying software engineering at BMSTU, department IU7, second year. Before that,
an engineering class with a gold medal, and a 70 percent scholarship to Central
University.

Winner of the BMSTU "Step into the Future" olympiad in computer science, winner of
the "Engineers of the Future" conference with a neural network project, and a prize
winner at the Moscow School Olympiad and the regional stage of the All-Russian
Olympiad.

I write about my projects too. There is
[an article on Habr](https://habr.com/ru/articles/1020668/) about how ttf-doom
works, and [a piece in Xakep](https://xakep.ru/2026/06/17/ttf-doom/) on running
code inside the TrueType virtual machine.

## Outside code

Video games as an art form, which is most of why I translate them. 3D printing.
Engineering that has no practical reason to exist. Music, more or less constantly.

## Contact

[![Telegram](https://img.shields.io/badge/Telegram-@artem__lyt-26A5E4?style=flat-square&logo=telegram&logoColor=white)](https://t.me/artem_lyt)
[![Email](https://img.shields.io/badge/Email-iprintercanon@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:iprintercanon@gmail.com)

<hr>

```
  АРТЁМ ЛЫТКИН
  ============
  $ whoami
  студент программной инженерии, МГТУ им. Баумана, Москва
```

Я учусь на программной инженерии в МГТУ имени Баумана.

То, чем я занимаюсь, делится примерно на две части. Первая это обычная системная
работа: контест-платформа на Go, которая отработала живые турниры в университете,
и одиннадцать патчей, принятых в staging-ветку ядра Linux. Вторая это выяснение,
что можно уговорить систему сделать, если её для этого никто не проектировал.
Именно так DOOM оказался запущен на одних лишь заменах по регулярному выражению,
а рейкастер поселился внутри файла шрифта.

Ещё я перевожу игры на русский, и это неожиданно хороший способ разобраться, как
другие люди пишут софт.

## Проекты

<table>
<tr>
<td width="50%" valign="top">

### [doom-regex](https://github.com/4RH1T3CT0R7/doom-regex)

[![stars](https://img.shields.io/github/stars/4RH1T3CT0R7/doom-regex?style=flat-square&logo=github&logoColor=white&label=stars&labelColor=21262d&color=e3b341)](https://github.com/4RH1T3CT0R7/doom-regex/stargazers)

<img src="https://raw.githubusercontent.com/4RH1T3CT0R7/doom-regex/main/docs/doom_regex_clip.gif" width="100%">

DOOM, работающий на одних заменах по регулярным выражениям. Одна строка на 96 МБ,
544 правила, результат побайтово совпадает с оригинальным DOOM. Оказалось, замены
PCRE2 достаточно, чтобы быть компьютером, если не торопиться.

</td>
<td width="50%" valign="top">

### [ttf-doom](https://github.com/4RH1T3CT0R7/ttf-doom)

[![stars](https://img.shields.io/github/stars/4RH1T3CT0R7/ttf-doom?style=flat-square&logo=github&logoColor=white&label=stars&labelColor=21262d&color=e3b341)](https://github.com/4RH1T3CT0R7/ttf-doom/stargazers)

<img src="https://raw.githubusercontent.com/4RH1T3CT0R7/ttf-doom/main/docs/media/demo.gif" width="100%">

Трёхмерный рейкастер внутри виртуальной машины хинтинга шрифта TrueType. Я написал
небольшой компилятор из C-подобного языка в байт-код TrueType, и рендерингом
занимается сам глиф. Весь движок весит 6.5 КБ.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [balatro-port-tui](https://github.com/4RH1T3CT0R7/balatro-port-tui)

[![stars](https://img.shields.io/github/stars/4RH1T3CT0R7/balatro-port-tui?style=flat-square&logo=github&logoColor=white&label=stars&labelColor=21262d&color=e3b341)](https://github.com/4RH1T3CT0R7/balatro-port-tui/stargazers)

<img src="https://raw.githubusercontent.com/4RH1T3CT0R7/balatro-port-tui/main/assets/demo.gif" width="100%">

Balatro в терминале, запускающая оригинальный Lua-код игры без единой правки.
Это переписанный на Rust движок LOVE2D с программным растеризатором и девятью
шейдерами, которые считаются на процессоре.

</td>
<td width="50%" valign="top">

### [TJudge](https://github.com/4RH1T3CT0R7/TJudge)

[![stars](https://img.shields.io/github/stars/4RH1T3CT0R7/TJudge?style=flat-square&logo=github&logoColor=white&label=stars&labelColor=21262d&color=e3b341)](https://github.com/4RH1T3CT0R7/TJudge/stargazers)

<img src="https://raw.githubusercontent.com/4RH1T3CT0R7/4RH1T3CT0R7/main/assets/tjudge-demo.gif" width="100%">

Турнирная платформа для соревнований по теории игр, работала в проде на Bauman
Code Games. Go и React, матчи исполняются в изолированных контейнерах, рейтинг по
ELO, таблица обновляется в реальном времени через WebSocket.

</td>
</tr>
</table>

## Принятые правки в чужие проекты

| Проект | Что сделал |
| --- | --- |
| [![Linux](https://img.shields.io/badge/Linux_kernel-FCC624?style=flat-square&logo=linux&logoColor=black)](https://github.com/search?q=repo%3Atorvalds%2Flinux+author%3A4RH1T3CT0R7&type=commits) | Одиннадцать патчей в `drivers/staging`: `most/dim2`, `sm750fb`, `nvec`, `fbtft` и `media/av7110`. Обработка ошибок, логирование через устройство, замена `BUG()` на нормальный возврат ошибки |
| [![GitHub CLI](https://img.shields.io/badge/GitHub_CLI-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/cli/cli/pull/12686) | Добавил флаг `--no-upstream` в `gh repo clone` |
| [![Docker](https://img.shields.io/badge/Docker_CLI-2496ED?style=flat-square&logo=docker&logoColor=white)](https://github.com/docker/cli/pull/6800) | Научил `docker cp` показывать и размер содержимого, и размер переданного |
| [![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)](https://github.com/grafana/grafana/pull/118156) | Починил индикатор активной вкладки на страницах настройки источников данных |
| [![Superset](https://img.shields.io/badge/Apache_Superset-20A6C9?style=flat-square&logo=apachesuperset&logoColor=white)](https://github.com/apache/superset/pull/37980) | Сохранил процентный формат для малых чисел в таблицах |
| [![Docusaurus](https://img.shields.io/badge/Docusaurus-3ECC5F?style=flat-square&logo=docusaurus&logoColor=white)](https://github.com/facebook/docusaurus/pull/11743) | Поправил поиск перевода для сгенерированного оглавления категории |
| [![Telegram](https://img.shields.io/badge/Telegram_Desktop-26A5E4?style=flat-square&logo=telegram&logoColor=white)](https://github.com/telegramdesktop/tdesktop/pull/30179) | Вернул кнопку разворачивания цитаты в поле подписи |
| [![Windows Terminal](https://img.shields.io/badge/Windows_Terminal-4D4D4D?style=flat-square&logo=windowsterminal&logoColor=white)](https://github.com/microsoft/terminal/pull/19931) | Сделал так, чтобы терминал получал фокус при выделении мышью с открытым поиском |
| [![PowerToys](https://img.shields.io/badge/PowerToys-0078D4?style=flat-square&logo=microsoft&logoColor=white)](https://github.com/microsoft/PowerToys/pull/50093) | Починил в Screen Ruler поиск границ у самого края экрана и переполнение при сравнении цветов в режиме рамки |
| [![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi_Imager-A22846?style=flat-square&logo=raspberrypi&logoColor=white)](https://github.com/raspberrypi/rpi-imager/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Семь правок: polkit на неизменяемых дистрибутивах, залипавшие настройки WiFi, файловые диалоги, сетка полей локализации и запасной звук для систем без freedesktop-звуков |
| [![Bambu Lab](https://img.shields.io/badge/Bambu_Studio-00AE42?style=flat-square&logo=bambulab&logoColor=white)](https://github.com/bambulab/BambuStudio/pull/9664) | Убрал лаг перетаскивания окна в Windows |
| [![Flipper](https://img.shields.io/badge/Flipper_One-FF8200?style=flat-square&logo=flipper&logoColor=white)](https://github.com/flipperdevices/flipperone-mcu-firmware/pull/70) | Написал документацию по сборке и прошивке |
| [![bitchat](https://img.shields.io/badge/bitchat-000000?style=flat-square&logo=bluetooth&logoColor=white)](https://github.com/permissionlesstech/bitchat/pull/1069) | Починил падение при повторном открытии личной переписки |
| [![PPSSPP](https://img.shields.io/badge/PPSSPP-5B6DCD?style=flat-square)](https://github.com/hrydgard/ppsspp/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Четыре правки: список точек останова в отладчике Win32 обновляется после изменения memcheck, регистры VFPU показывают значения и прокручиваются, кнопки открытия папок снова работают на Linux, а диалог сохранений берёт дату из PARAM.SFO |
| [![Gitea](https://img.shields.io/badge/Gitea-609926?style=flat-square&logo=gitea&logoColor=white)](https://github.com/go-gitea/gitea/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Три правки: подписи OpenPGP больше не проверяются ключом SSH-инстанса, ссылки сравнения по умолчанию называют head-репозиторий, трейлеры соавторов не по RFC 5322 разбираются |
| [![Fyne](https://img.shields.io/badge/Fyne-1A9FD9?style=flat-square)](https://github.com/fyne-io/fyne/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Четыре правки: падение по nil при изменении размера файлового диалога до `Show()`, растр рисуется от левого верхнего угла своих границ, подменю выше окна прокручиваются, а виджеты под внутренним окном больше не меняют курсор |
| [![CircuitPython](https://img.shields.io/badge/CircuitPython-7B3FE4?style=flat-square&logo=adafruit&logoColor=white)](https://github.com/adafruit/circuitpython/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Три правки: `TimeAlarm` проверяет тип времени, `WaveFile` правильно дополняет 8-битные сэмплы в конце файла, unix-порт собирается на arm64 |
| [![Wails](https://img.shields.io/badge/Wails-D32F2F?style=flat-square)](https://github.com/wailsapp/wails/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Убрал утечку `Calloc` во фронтендах v2 для Linux и macOS и выкинул скомпилированные бинарники примеров из v3 |
| [![Space Station 14](https://img.shields.io/badge/Space_Station_14-1C6EA4?style=flat-square)](https://github.com/space-wizards/space-station-14/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Дефибриллятор больше не отчитывается о том, к чему пристёгнут пациент, а плата законов Crewsimov теперь и внутри называется Crewsimov |
| [![Flameshot](https://img.shields.io/badge/Flameshot-009688?style=flat-square)](https://github.com/flameshot-org/flameshot/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Починил размер закреплённого снимка на масштабированных экранах Windows и добавил фолбэк на перевод того же языка |
| [![RetroArch](https://img.shields.io/badge/RetroArch-000000?style=flat-square)](https://github.com/libretro/RetroArch/pull/19584) | Вернул диапазон настройки масштаба виджетов на консольных и мобильных сборках |
| [![micro](https://img.shields.io/badge/micro-2E3440?style=flat-square)](https://github.com/micro-editor/micro/pull/4179) | Научил плагин линтера сравнивать пути через `filepath.Base()`, чтобы сообщения линтера не терялись |
| [![hashcat](https://img.shields.io/badge/hashcat-111111?style=flat-square)](https://github.com/hashcat/hashcat/pull/4617) | Исправил длину соли, которую режим 3710 сообщает для оптимизированного ядра |
| [![Throne](https://img.shields.io/badge/Throne-1A73E8?style=flat-square&logo=v2fly&logoColor=white)](https://github.com/throneproj/Throne/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | Шесть правок: падение ядра на Remove Invalid, системный прокси не сбрасывался при выходе, устаревшие результаты завершённой проверки задержек, имена полей для экранных дикторов в диалогах хоткеев, маршрутов и профиля, и диалог маршрутов, растягивавшийся по самому длинному имени профиля |
| [![Millennium Dawn](https://img.shields.io/badge/Millennium_Dawn-8B0000?style=flat-square)](https://github.com/MillenniumDawn/Millennium-Dawn/pulls?q=is%3Apr+author%3A4RH1T3CT0R7+is%3Amerged) | 66 принятых пул-реквестов в мод для Hearts of Iron IV: система разведки, несколько экономических эксплойтов, поведение ИИ и целый ряд древ национальных фокусов |

Всего я открывал пул-реквесты в 52 чужих проекта. Ещё 57 из них сейчас открыты,
в 33 проектах, среди которых Kubernetes, VS Code, Moby, Ollama, Next.js,
TensorFlow, Supabase, Tailscale, OBS Studio, Notepad++ и обе среды Arduino.

## Русские локализации игр

Четыре игры, у которых официального русского не было вовсе или он был плохим.

- **[Suzerain](https://steamcommunity.com/sharedfiles/filedetails/?id=2908967542)**
  это самый большой проект. Опубликован в декабре 2022 и обновляется до сих пор,
  11 тысяч читателей и 693 человека держат его в избранном. Делали командой
  переводчиков примерно три года.
- **[Night Call](https://github.com/4RH1T3CT0R7/russian-localisation-night-call)**
  это 5371 диалоговый пассаж, 789 ключей интерфейса и все имена пассажиров, через
  плагин BepInEx со сгенерированными кириллическими SDF-атласами.
- **[Interrogation](https://github.com/4RH1T3CT0R7/interrogation-russian-translation)**
  это все 60 файлов локализации, три десятка допросов и 23 кириллических шрифта,
  включая системный.
- **[Not Tonight](https://github.com/4RH1T3CT0R7/not-tonight-russian)** это базовая
  игра плюс дополнение One Love, около восьми тысяч ключей.

## Стек

```
языки          Go, Python, Rust, C, C#, Lua
бэкенд         PostgreSQL, Redis, Chi, REST, WebSocket, gRPC
инфраструктура Docker, Prometheus, Grafana, Loki, Linux
ml             TensorFlow, PyTorch
низкий уровень TrueType hinting VM, Lua VM, Sixel, отрисовка в терминале
```

## Образование и награды

Программная инженерия в МГТУ имени Баумана, кафедра ИУ7, второй курс. До этого
инженерный класс с золотой медалью и грант на обучение в Центральном университете
на 70 процентов.

Победитель олимпиады МГТУ «Шаг в будущее» по информатике, победитель конференции
«Инженеры будущего» с проектом по нейронным сетям, призёр Московской олимпиады
школьников и регионального этапа Всероссийской олимпиады.

Про свои проекты я иногда пишу. Есть
[статья на Хабре](https://habr.com/ru/articles/1020668/) о том, как устроен
ttf-doom, и [материал в «Хакере»](https://xakep.ru/2026/06/17/ttf-doom/) про
запуск кода внутри виртуальной машины TrueType.

## Вне кода

Видеоигры как форма искусства, во многом поэтому я их и перевожу. Трёхмерная
печать. Инженерия, у которой нет практических причин существовать. Музыка,
более или менее постоянно.

## Связь

[![Telegram](https://img.shields.io/badge/Telegram-@artem__lyt-26A5E4?style=flat-square&logo=telegram&logoColor=white)](https://t.me/artem_lyt)
[![Email](https://img.shields.io/badge/Email-iprintercanon@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:iprintercanon@gmail.com)

<hr>

<img src="https://github-readme-stats.vercel.app/api?username=4RH1T3CT0R7&show_icons=true&theme=dark&hide_border=true&include_all_commits=true&count_private=true" height="150">
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=4RH1T3CT0R7&layout=compact&theme=dark&hide_border=true&langs_count=8" height="150">
