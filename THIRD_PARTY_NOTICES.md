# Сторонние компоненты FLOW BRIDGE Windows 0.1.8

> Проект уведомлений. Инвентаризация по зафиксированному графу Cargo для x86_64-pc-windows-msvc, с обычными зависимостями и без proc-macro. Наличие пакета в графе само по себе не доказывает присутствие всех его объектов в итоговом EXE.

Тексты из архивов зависимостей собраны в [THIRD_PARTY_LICENSE_TEXTS.txt](THIRD_PARTY_LICENSE_TEXTS.txt). Лицензии относятся к соответствующим компонентам. Собственные компоненты FLOW BRIDGE распространяются по [отдельной лицензии](LICENSE.txt).

- MIT, BSD, ISC, 0BSD и Zlib. Сохранить применимые уведомления об авторских правах и условия распространения. Для альтернативных выражений можно выбрать одну разрешённую лицензию. Для выражений с AND учитываются все применимые части, в том числе Apache-2.0 AND ISC.
- Apache-2.0. Передать текст лицензии, сохранить применимые уведомления NOTICE и указать изменения там, где это требуется. Unicode-3.0, BSL-1.0 и CDLA-Permissive-2.0 требуют отдельной проверки условий сохранения уведомлений для соответствующего кода или данных.
- В выбранном Windows-графе по метаданным не найдено MPL, GPL, LGPL или AGPL. Это предварительный результат. Вложенный код и его уведомления, Rust runtime и системные import libraries требуют отдельной сверки с составом бинарника. Наличие лицензии в Cargo.lock вне Windows-графа не означает её применимость к установщику.
- epaint 0.28.1 включает Hack, Noto Emoji, Ubuntu Light и Emoji Icon Font. Сохранить их отдельные уведомления, условия OFL, Ubuntu Font Licence и MIT, а для Hack учесть условия из Hack-Regular.txt. Ограничения на имена и самостоятельную продажу шрифтов оцениваются по тексту каждого шрифта. Системный Segoe UI читается из Windows.
- Inno Setup 6.7.3 используется как сборочный инструмент. Его код Setup входит в Installer. Сохранить уже имеющиеся copyright и адреса сайта, правильно указать происхождение и пометить модификации, если они были. Отдельно подтвердить статус коммерческого использования компилятора по правилам производителя. [Лицензия версии 6.7.3](https://raw.githubusercontent.com/jrsoftware/issrc/is-6_7_3/license.txt) · [Коммерческие лицензии](https://jrsoftware.org/isorder.php)
- Установщик поставляет приложение и flow-bridge.ico. Право использования и происхождение иконки должен подтвердить владелец. Лицензии языковых ресурсов и вложенных частей Inno Setup требуют сверки.
- Cargo build dependencies, proc-macro и тестовые зависимости учитываются отдельно. Их использование при сборке само по себе не делает их распространяемыми библиотеками. Для сгенерированных или встроенных фрагментов проверяется фактическое включение.
- Cloudflare Worker/D1 и серверные библиотеки рассматриваются отдельно от Windows Installer. Chrome и Google Flow используются как внешние продукты по их собственным условиям.

Перед утверждением нужны сверка вложенных уведомлений и подтверждение, что уведомления предоставляются получателю дистрибутива способом, требуемым каждой лицензией. Публикация этого проекта сама по себе не подтверждает соблюдение требований уже выпущенной сборкой.

## Проверенные тексты для 11 архивов Cargo

Пакеты содержат декларацию лицензии. Отдельный файл в архиве отсутствовал, поэтому взят текст из коммита, указанного в метаданных публикации соответствующего пакета. В проверенных деревьях для этих пакетов отдельных NOTICE не найдено. Для AccessKit сохранён также upstream LICENSE.chromium, поскольку его применимость зависит от включения соответствующих фрагментов. Выбор MIT относится только к перечисленным выражениям с OR.

| Пакет | Точный upstream | Выбранная лицензия | Тексты |
|---|---|---|---|
| accesskit 0.12.3 | [AccessKit/accesskit](https://github.com/AccessKit/accesskit/tree/56bf6f2f51b352b35bd4c8c72b7ed18ad9470e2f) | MIT | [LICENSE-MIT](https://github.com/AccessKit/accesskit/blob/56bf6f2f51b352b35bd4c8c72b7ed18ad9470e2f/LICENSE-MIT), [LICENSE.chromium](https://github.com/AccessKit/accesskit/blob/56bf6f2f51b352b35bd4c8c72b7ed18ad9470e2f/LICENSE.chromium) |
| accesskit_consumer 0.16.1 | [AccessKit/accesskit](https://github.com/AccessKit/accesskit/tree/1930c72276b521f06e3e006904d578948fa36955) | MIT | [LICENSE-MIT](https://github.com/AccessKit/accesskit/blob/1930c72276b521f06e3e006904d578948fa36955/LICENSE-MIT), [LICENSE.chromium](https://github.com/AccessKit/accesskit/blob/1930c72276b521f06e3e006904d578948fa36955/LICENSE.chromium) |
| accesskit_windows 0.15.1 | [AccessKit/accesskit](https://github.com/AccessKit/accesskit/tree/1930c72276b521f06e3e006904d578948fa36955) | MIT | [LICENSE-MIT](https://github.com/AccessKit/accesskit/blob/1930c72276b521f06e3e006904d578948fa36955/LICENSE-MIT), [LICENSE.chromium](https://github.com/AccessKit/accesskit/blob/1930c72276b521f06e3e006904d578948fa36955/LICENSE.chromium) |
| accesskit_winit 0.16.1 | [AccessKit/accesskit](https://github.com/AccessKit/accesskit/tree/c80cdf70421d054e9be5514c8e0f1fc455eeb375) | Apache-2.0 | [LICENSE-APACHE](https://github.com/AccessKit/accesskit/blob/c80cdf70421d054e9be5514c8e0f1fc455eeb375/LICENSE-APACHE), [LICENSE.chromium](https://github.com/AccessKit/accesskit/blob/c80cdf70421d054e9be5514c8e0f1fc455eeb375/LICENSE.chromium) |
| clipboard-win 5.4.1 | [DoumanAsh/clipboard-win](https://github.com/DoumanAsh/clipboard-win/tree/3b27cf2bfd1adcfa6e0264eb51c1025ddaf0f342) | BSL-1.0 | [LICENSE](https://github.com/DoumanAsh/clipboard-win/blob/3b27cf2bfd1adcfa6e0264eb51c1025ddaf0f342/LICENSE) |
| ecolor 0.28.1 | [emilk/egui](https://github.com/emilk/egui/tree/abab06867cdbc8966cf1de1e5429a7b7f9126af2) | MIT | [LICENSE-MIT](https://github.com/emilk/egui/blob/abab06867cdbc8966cf1de1e5429a7b7f9126af2/LICENSE-MIT) |
| eframe 0.28.1 | [emilk/egui](https://github.com/emilk/egui/tree/abab06867cdbc8966cf1de1e5429a7b7f9126af2) | MIT | [LICENSE-MIT](https://github.com/emilk/egui/blob/abab06867cdbc8966cf1de1e5429a7b7f9126af2/LICENSE-MIT) |
| egui 0.28.1 | [emilk/egui](https://github.com/emilk/egui/tree/abab06867cdbc8966cf1de1e5429a7b7f9126af2) | MIT | [LICENSE-MIT](https://github.com/emilk/egui/blob/abab06867cdbc8966cf1de1e5429a7b7f9126af2/LICENSE-MIT) |
| egui-winit 0.28.1 | [emilk/egui](https://github.com/emilk/egui/tree/abab06867cdbc8966cf1de1e5429a7b7f9126af2) | MIT | [LICENSE-MIT](https://github.com/emilk/egui/blob/abab06867cdbc8966cf1de1e5429a7b7f9126af2/LICENSE-MIT) |
| egui_glow 0.28.1 | [emilk/egui](https://github.com/emilk/egui/tree/abab06867cdbc8966cf1de1e5429a7b7f9126af2) | MIT | [LICENSE-MIT](https://github.com/emilk/egui/blob/abab06867cdbc8966cf1de1e5429a7b7f9126af2/LICENSE-MIT) |
| emath 0.28.1 | [emilk/egui](https://github.com/emilk/egui/tree/abab06867cdbc8966cf1de1e5429a7b7f9126af2) | MIT | [LICENSE-MIT](https://github.com/emilk/egui/blob/abab06867cdbc8966cf1de1e5429a7b7f9126af2/LICENSE-MIT) |

## Inno Setup и ресурсы

- Журнал сборки подтверждает Inno Setup 6.7.3, Setup.e32, чтение isunzlib.dll и языковых ресурсов Default.isl и Russian.isl. Сценарий использует ZIP. Присутствие других компонентов из дерева upstream не следует из их наличия в репозитории.
- Лицензия 6.7.3 допускает использование и распространение при сохранении применимых уведомлений и адресов сайта, указании происхождения и маркировке модификаций. Запрос производителя о покупке коммерческой лицензии изложен отдельно. Производитель указывает, что покупка не строго обязательна. Проверка бизнес-контекста остаётся у владельца. [Лицензия](https://github.com/jrsoftware/issrc/blob/is-6_7_3/license.txt) · [FAQ производителя](https://jrsoftware.org/isorder.php)
### Сверка опубликованного Installer

Проверен Installer с SHA-256 `46a4e503d7d16f769a9edb7d69c705b973759f27d05fa7e36d7197883b9a71f8` и размером 8 012 003 байта. Извлечение выполнено статически, без запуска Setup. Проверены CRC таблицы загрузчика, заголовков и блоков. Для исполняемых файлов обращено преобразование CALL/JMP, описанное в Inno Setup 6.7.3. [Формат блоков](https://github.com/jrsoftware/issrc/blob/is-6_7_3/Projects/Src/Compression.Base.pas) · [Запись DLL в Setup-0](https://github.com/jrsoftware/issrc/blob/is-6_7_3/Projects/Src/Compiler.SetupCompiler.pas)

| Позиция | Результат по опубликованному файлу | Уведомления и оставшаяся проверка |
|---|---|---|
| Setup Loader и Setup engine | Таблица загрузчика указывает на Setup engine. Распаковано 4 427 264 байта, CRC совпал, SHA-256 `bb9703e17465da263360a3d6a949de7d6587a53b932182422786f03e18b90a7b`. В связке с журналом релизной компиляции установлена версия Inno Setup 6.7.3. | Сохранить существующие copyright и URL производителя. Текст лицензии приложен. Проверить сохранность встроенных уведомлений, полноту notices для встроенного кода Setup и языковых ресурсов. |
| isunzlib.dll / zlib 1.2.3 | В конце распакованного заголовка Setup-0 найден блок с префиксом длины 29 472 байта. DLL совпала побайтно с [upstream DLL](https://github.com/jrsoftware/issrc/blob/is-6_7_3/Files/isunzlib.dll), SHA-256 `8287d0e287a66ee78537c8d1d98e426562b95c50f569b92cea9ce36a9fa57e64`. Версия 1.2.3 подтверждается строкой в DLL и [историческим заголовком](https://github.com/jrsoftware/iscompress/blob/6cd23a60d342c966a80e2aae85009172efdeca3e/zlib-dll/zlib.h). | Условия zlib и исходное уведомление включены в комплект. Сохранять корректное указание происхождения. |
| flow-bridge.exe | Извлечённый EXE совпал с манифестом сборки, SHA-256 `ffd82ab5adf2289b9f313e5593c8fb73741c3e4a122fa2ca555214cdfd6de1fb`. | Применимые notices Rust-библиотек и встроенных шрифтов собраны по графу Cargo. BLOCKED по полноте: сверить фактические статически включённые объекты, Rust runtime, условия вложенного кода и передачу notices получателю. |
| flow-bridge.ico | Извлечено 14 941 байт, SHA-256 `d40ea884fd7ce44cc40a38fdcba8d9ee6f1c51598d5699e567daaab3aa5528c9`. История файла фиксирует его присутствие в снимке исходников. | OWNER_REQUIRED. Нужны мастер-ассет, автор и подтверждение права на распространение. Хеш и история файла права не устанавливают. |

Тексты Inno Setup, zlib, зависимостей Cargo и отдельных лицензий шрифтов собраны в приложении. Полный набор обязательных notices пока не подтверждён. Для этого нужны проверка встроенных частей Setup и Rust runtime, подтверждение прав на ассет и сверка фактической передачи применимых текстов с дистрибутивом. Наличие справочного текста UniPs не доказывает, что соответствующий компонент присутствует в бинарнике.

## Граф Windows x64

| Пакет | Выражение лицензии из метаданных | Найденные тексты |
|---|---|---|

| ab_glyph 0.2.32 | Apache-2.0 | LICENSE |
| ab_glyph_rasterizer 0.1.10 | Apache-2.0 | LICENSE |
| accesskit 0.12.3 | MIT OR Apache-2.0 | См. проверенные upstream-тексты выше |
| accesskit_consumer 0.16.1 | MIT OR Apache-2.0 | См. проверенные upstream-тексты выше |
| accesskit_windows 0.15.1 | MIT OR Apache-2.0 | См. проверенные upstream-тексты выше |
| accesskit_winit 0.16.1 | Apache-2.0 | См. проверенные upstream-тексты выше |
| adler2 2.0.1 | 0BSD OR MIT OR Apache-2.0 | LICENSE-0BSD, LICENSE-APACHE, LICENSE-MIT |
| ahash 0.8.12 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| aho-corasick 1.1.5 | Unlicense OR MIT | COPYING, LICENSE-MIT, UNLICENSE |
| anstream 1.0.0 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| anstyle 1.0.14 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| anstyle-parse 1.0.0 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| anstyle-query 1.1.5 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| anstyle-wincon 3.0.11 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| arboard 3.6.1 | MIT OR Apache-2.0 | LICENSE-APACHE.txt, LICENSE-MIT.txt |
| base64 0.22.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| bitflags 2.13.2 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| block-buffer 0.10.4 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| block-buffer 0.12.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| bumpalo 3.20.3 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| bytemuck 1.25.2 | Zlib OR Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT, LICENSE-ZLIB |
| byteorder-lite 0.1.0 | Unlicense OR MIT | LICENSE-MIT, UNLICENSE |
| bytes 1.12.1 | MIT | LICENSE |
| cfg-if 1.0.5 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| chacha20 0.10.2 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| chrono 0.4.45 | MIT OR Apache-2.0 | LICENSE.txt |
| clap 4.6.7 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| clap_builder 4.6.7 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| clap_lex 1.1.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| clipboard-win 5.4.1 | BSL-1.0 | См. проверенные upstream-тексты выше |
| colorchoice 1.0.5 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| const-oid 0.10.2 | Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT |
| cpufeatures 0.2.17 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| cpufeatures 0.3.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| crc32fast 1.5.2 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| crypto-common 0.1.7 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| crypto-common 0.2.2 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| cursor-icon 1.2.0 | MIT OR Apache-2.0 OR Zlib | LICENSE-APACHE, LICENSE-MIT, LICENSE-ZLIB |
| curve25519-dalek 4.1.3 | BSD-3-Clause | LICENSE |
| data-encoding 2.11.1 | MIT | LICENSE |
| digest 0.10.7 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| digest 0.11.3 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| ecolor 0.28.1 | MIT OR Apache-2.0 | См. проверенные upstream-тексты выше |
| ed25519 2.2.3 | Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT |
| ed25519-dalek 2.2.0 | BSD-3-Clause | LICENSE |
| eframe 0.28.1 | MIT OR Apache-2.0 | См. проверенные upstream-тексты выше |
| egui 0.28.1 | MIT OR Apache-2.0 | См. проверенные upstream-тексты выше |
| egui-winit 0.28.1 | MIT OR Apache-2.0 | См. проверенные upstream-тексты выше |
| egui_glow 0.28.1 | MIT OR Apache-2.0 | См. проверенные upstream-тексты выше |
| emath 0.28.1 | MIT OR Apache-2.0 | См. проверенные upstream-тексты выше |
| epaint 0.28.1 | (MIT OR Apache-2.0) AND OFL-1.1 AND LicenseRef-UFL-1.0 | fonts/emoji-icon-font-mit-license.txt, fonts/Hack-Regular.txt, fonts/OFL.txt, fonts/UFL.txt |
| equivalent 1.0.2 | Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT |
| error-code 3.4.0 | BSL-1.0 | LICENSE |
| fdeflate 0.3.7 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| flate2 1.1.10 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| form_urlencoded 1.2.2 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| futures-core 0.3.34 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| futures-sink 0.3.34 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| futures-task 0.3.34 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| futures-util 0.3.34 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| generic-array 0.14.7 | MIT | LICENSE |
| getrandom 0.2.17 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| getrandom 0.4.3 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| glow 0.13.1 | MIT OR Apache-2.0 OR Zlib | LICENSE-APACHE, LICENSE-MIT, LICENSE-ZLIB |
| glutin 0.31.3 | Apache-2.0 | LICENSE |
| glutin-winit 0.4.2 | MIT | LICENSE |
| glutin_egl_sys 0.6.0 | Apache-2.0 | LICENSE |
| glutin_wgl_sys 0.5.0 | Apache-2.0 | LICENSE |
| hashbrown 0.17.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| http 1.5.0 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| httparse 1.10.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| hybrid-array 0.4.15 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| icu_collections 2.3.0 | Unicode-3.0 | LICENSE |
| icu_locale_core 2.3.0 | Unicode-3.0 | LICENSE |
| icu_normalizer 2.3.0 | Unicode-3.0 | LICENSE |
| icu_normalizer_data 2.3.0 | Unicode-3.0 | LICENSE |
| icu_properties 2.3.0 | Unicode-3.0 | LICENSE |
| icu_properties_data 2.3.0 | Unicode-3.0 | LICENSE |
| icu_provider 2.3.1 | Unicode-3.0 | LICENSE |
| idna 1.1.0 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| idna_adapter 1.2.2 | Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT |
| image 0.25.10 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| indexmap 2.14.2 | Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT |
| is_terminal_polyfill 1.70.2 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| itoa 1.0.18 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| libloading 0.8.9 | ISC | LICENSE |
| litemap 0.8.3 | Unicode-3.0 | LICENSE |
| lock_api 0.4.14 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| log 0.4.34 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| memchr 2.8.3 | Unlicense OR MIT | COPYING, LICENSE-MIT, UNLICENSE |
| memoffset 0.9.1 | MIT | LICENSE |
| miniz_oxide 0.8.9 | MIT OR Zlib OR Apache-2.0 | LICENSE, LICENSE-APACHE.md, LICENSE-MIT.md, LICENSE-ZLIB.md |
| miniz_oxide 0.9.1 | MIT OR Zlib OR Apache-2.0 | LICENSE, LICENSE-APACHE.md, LICENSE-MIT.md, LICENSE-ZLIB.md |
| mio 1.2.3 | MIT | LICENSE |
| moxcms 0.8.1 | BSD-3-Clause OR Apache-2.0 | LICENSE-APACHE.md, LICENSE.md |
| nohash-hasher 0.2.0 | Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT |
| num-traits 0.2.19 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| once_cell 1.21.4 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| once_cell_polyfill 1.70.2 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| owned_ttf_parser 0.25.1 | Apache-2.0 | LICENSE |
| parking_lot 0.12.5 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| parking_lot_core 0.9.12 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| percent-encoding 2.3.2 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| pin-project-lite 0.2.17 | Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT |
| png 0.18.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| potential_utf 0.1.6 | Unicode-3.0 | LICENSE |
| pxfm 0.1.30 | BSD-3-Clause OR Apache-2.0 | LICENSE-APACHE.md, LICENSE.md |
| rand 0.10.2 | MIT OR Apache-2.0 | COPYRIGHT, LICENSE-APACHE, LICENSE-MIT |
| rand_core 0.10.1 | MIT OR Apache-2.0 | COPYRIGHT, LICENSE-APACHE, LICENSE-MIT |
| raw-window-handle 0.5.2 | MIT OR Apache-2.0 OR Zlib | LICENSE-APACHE.md, LICENSE-MIT.md, LICENSE-ZLIB.md |
| raw-window-handle 0.6.2 | MIT OR Apache-2.0 OR Zlib | LICENSE-APACHE.md, LICENSE-MIT.md, LICENSE-ZLIB.md |
| regex 1.13.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| regex-automata 0.4.18 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| regex-syntax 0.8.11 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| ring 0.17.14 | Apache-2.0 AND ISC | LICENSE, LICENSE-BoringSSL, LICENSE-other-bits |
| rustls 0.23.45 | Apache-2.0 OR ISC OR MIT | LICENSE-APACHE, LICENSE-ISC, LICENSE-MIT |
| rustls-pki-types 1.15.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| rustls-webpki 0.103.15 | ISC | LICENSE |
| scopeguard 1.2.0 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| serde 1.0.229 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| serde_core 1.0.229 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| serde_json 1.0.151 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| sha1 0.11.0 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| sha2 0.10.9 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| signature 2.2.0 | Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT |
| simd-adler32 0.3.10 | MIT | LICENSE.md |
| slab 0.4.12 | MIT | LICENSE |
| smallvec 1.16.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| smol_str 0.2.2 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| socket2 0.6.5 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| stable_deref_trait 1.2.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| static_assertions 1.1.0 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| strsim 0.11.1 | MIT | LICENSE |
| subtle 2.6.1 | BSD-3-Clause | LICENSE |
| thiserror 1.0.69 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| thiserror 2.0.20 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| tinystr 0.8.4 | Unicode-3.0 | LICENSE |
| tokio 1.53.1 | MIT | LICENSE |
| tokio-tungstenite 0.30.0 | MIT | LICENSE |
| ttf-parser 0.25.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| tungstenite 0.30.0 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| typenum 1.20.1 | MIT OR Apache-2.0 | LICENSE, LICENSE-APACHE, LICENSE-MIT |
| unicode-segmentation 1.13.3 | MIT OR Apache-2.0 | COPYRIGHT, LICENSE-APACHE, LICENSE-MIT |
| untrusted 0.9.0 | ISC | LICENSE.txt |
| ureq 2.12.1 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| url 2.5.8 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| utf8_iter 1.0.4 | Apache-2.0 OR MIT | COPYRIGHT, LICENSE-APACHE, LICENSE-MIT |
| utf8parse 0.2.2 | Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT |
| uuid 1.26.1 | Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT |
| web-time 0.2.4 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| webbrowser 1.2.4 | MIT OR Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| webpki-roots 0.26.11 | CDLA-Permissive-2.0 | LICENSE |
| webpki-roots 1.0.9 | CDLA-Permissive-2.0 | LICENSE |
| winapi 0.3.9 | MIT/Apache-2.0 | LICENSE-APACHE, LICENSE-MIT |
| windows 0.48.0 | MIT OR Apache-2.0 | license-apache-2.0, license-mit |
| windows-link 0.2.1 | MIT OR Apache-2.0 | license-apache-2.0, license-mit |
| windows-sys 0.48.0 | MIT OR Apache-2.0 | license-apache-2.0, license-mit |
| windows-sys 0.60.2 | MIT OR Apache-2.0 | license-apache-2.0, license-mit |
| windows-sys 0.61.2 | MIT OR Apache-2.0 | license-apache-2.0, license-mit |
| windows-targets 0.48.5 | MIT OR Apache-2.0 | license-apache-2.0, license-mit |
| windows-targets 0.53.5 | MIT OR Apache-2.0 | license-apache-2.0, license-mit |
| windows_x86_64_msvc 0.48.5 | MIT OR Apache-2.0 | license-apache-2.0, license-mit |
| windows_x86_64_msvc 0.53.1 | MIT OR Apache-2.0 | license-apache-2.0, license-mit |
| winit 0.29.15 | Apache-2.0 | LICENSE |
| writeable 0.6.4 | Unicode-3.0 | LICENSE |
| yoke 0.8.3 | Unicode-3.0 | LICENSE |
| zerocopy 0.8.58 | BSD-2-Clause OR Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-BSD, LICENSE-MIT |
| zerofrom 0.1.8 | Unicode-3.0 | LICENSE |
| zeroize 1.9.0 | Apache-2.0 OR MIT | LICENSE-APACHE, LICENSE-MIT |
| zerotrie 0.2.5 | Unicode-3.0 | LICENSE |
| zerovec 0.11.8 | Unicode-3.0 | LICENSE |
| zip 2.4.2 | MIT | LICENSE |
| zmij 1.0.23 | MIT | LICENSE-MIT |
| zopfli 0.8.3 | Apache-2.0 | COPYING |
