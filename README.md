![](./Assets/Lapka.png)

![](./Assets/Lapka-03.jpg)

# Лапка

Беспроводная эргономичная сплит-клавиатура для тех, у кого лапки (:

**Особенности:**
- 36 клавиш, совместима с Choc v2 свитчами
- Direct-pin подключение — при сборке не требуются диоды
- Низкопрофильный корпус (свитчи практически касаются стола)

**Структура репозитория:**

| Директория | Описание                                              |
| ---------: | :---------------------------------------------------- |
|        3MF | Проект OrcaSlicer (для примера параметров печати)     |
|     Assets | Изображения и фото                                    |
|     Fusion | Проект Autodesk Fusion 360                            |
|    Gerbers | Gerber-файлы для производства плат                    |
|      Guide | Описание [процесса сборки](./Guide/build-guide-ru.md) |
|      KiCad | Проект KiCad (схема, плата, компоненты)               |
|        STL | 3D-модели частей корпуса                              |

Ссылка на актуальную [прошивку ZMK](https://github.com/braindefender/lapka-zmk-config).
Используйте вариант подключения direct-pin, описанный в `lapka_wellum36_left.overlay` и `lapka_wellum36_right.overlay`.

Откройте GitHub Actions и найдите последний успешно собранный билд ветки `lapka-36`.
В нём будет артефакт сборки `firmware.zip`, который содержит все нужные для прошивки файлы.

Для того, чтобы превратить её в debug-прошивку, надо заменить клавиши на thumb-кластере на какие-нибудь другие.
Например, F1, F2, F3 для левой половинки сплита и F4, F5, F6 для правой.

Это позволит увидеть нажатия клавиш на [key-test.ru](https://key-test.ru).

## История изменений

### v2.1
- Изменена ссылка на репозиторий прошивки ZMK

### v2
- Добавлена поддержка Choc v1
- Изменена разметка пинов
- Обновлена шелкография, логотип перенесён на Cu слой
- Добавлен проект Fusion 360

### v1
- Первый релиз. Только для Choc v2

# Lapka

Wireless ergonomic split keyboard for those who have paws (:

**Peculiarities:**
- 36 keys, Choc v2 compatible
- Direct-pin connection — no diodes needed required
- Low-profile case (switches almost touch the table)

**Repository structure:**

| Directory | Description                                            |
| --------: | :----------------------------------------------------- |
|       3MF | OrcaSlicer project files (printing parameters example) |
|    Assets | Images and photos                                      |
|    Fusion | Autodesk Fusion 360 project                            |
|   Gerbers | Gerber-files for PCB production                        |
|     Guide | [Build guide](./Guide/build-guide-en.md)               |
|     KiCad | KiCad project (schematics, PCB design, components)     |
|       STL | 3D-models of case parts                                |

Link to the current [ZMK firmware](https://github.com/braindefender/lapka-zmk-config).
Use direct pin layout, described in `lapka_wellum36_left.overlay` and `lapka_wellum36_right.overlay`.

Open GitHub Actions and find latest successful build of branch `lapka-36`.
In that build you'll find artifact `firmware.zip`, which contain all the neccessary firmware files.

To make debug firmware, you can change thumb-cluster buttons to something else.
For example, F1, F2, F3 for left part of the split, and F4, F5, F6 for the other.

That will help to see keypresses on the [key-test.ru](https://key-test.ru).

## Changelog

### v2.1
- Changed link to ZMK Firmware repo

### v2
- Added support for Choc v1
- Changed pin layout
- Updated silk-screen, moved logo to Cu layer
- Added Fusion 360 project

### v1
- Initial release. Only for Choc v2

## Фото / Photos

### Original

![](./Assets/Lapka-01.jpg)
![](./Assets/Lapka-02.jpg)

### From awesome people

![](./Assets/photo_@f1dell.jpg)

> by [Макс / f1dell](https://t.me/f1dell)

![](./Assets/photo_@pravets_IT.jpg)

> by [Иосиф Правец](https://t.me/pravets_IT)
