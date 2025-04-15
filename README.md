![](./Images/Lapka.png)

# Лапка

Беспроводная эргономичная сплит-клавиатура для тех, у кого лапки (:

**Особенности:**
- 36 клавиш, совместима с Choc v2 свитчами
- Direct-pin подключение — при сборке не требуются диоды
- Низкопрофильный корпус (свитчи практически касаются стола)

**Структура репозитория:**

| Директория | Описание                                              |
| ---------: | :---------------------------------------------------- |
| 3MF        | Проект OrcaSlicer (для примера параметров печати)     |
| Gerbers    | Gerber-файлы для производства плат                    |
| Guide      | Описание [процесса сборки](./Guide/build-guide-ru.md) |
| Images     | Изображения и фото                                    |
| KiCad      | Проект KiCad (схема, плата, компоненты)               |
| STL        | 3D-модели частей корпуса                              |

Ссылка на актуальную [прошивку ZMK](https://github.com/braindefender/wellum/tree/master/firmware/zmk/wellum36).
Используйте вариант подключения direct-pin, описанный в `wellum36_left.overlay` и `wellum36_right.overlay`.

Для того, чтобы превратить её в debug-прошивку, надо заменить клавиши на thumb-кластере на какие-нибудь другие.
Например, F1, F2, F3 для левой половинки сплита и F4, F5, F6 для правой. 

Это позволит увидеть нажатия клавиш на [key-test.ru](https://key-test.ru).

# Lapka

Wireless ergonomic split keyboard for those who have paws (:

**Peculiarities:**
- 36 keys, Choc v2 compatible
- Direct-pin connection — no diodes needed required
- Low-profile case (switches almost touch the table)

**Repository structure:**

| Directory | Description                                            |
| --------: | :----------------------------------------------------- |
| 3MF       | OrcaSlicer project files (printing parameters example) |
| Gerbers   | Gerber-files for PCB production                        |
| Guide     | [Build guide](./Guide/build-guide-en.md)               |
| Images    | Images and photos                                      |
| KiCad     | KiCad project (schematics, PCB design, components)     |
| STL       | 3D-models of case parts                                |

Link to the current [ZMK firmware](https://github.com/braindefender/wellum/tree/master/firmware/zmk/wellum36). 
Use direct pin layout, described in `wellum36_left.overlay` and `wellum36_right.overlay`.

To make debug firmware, you can change thumb-cluster buttons to something else.
For example, F1, F2, F3 for left part of the split, and F4, F5, F6 for the other.

That will help to see keypresses on the [key-test.ru](https://key-test.ru).

## TODO

- add Fusion360 project files
- add real photos