# Логгер сообщений

Этот проект включает библиотеку для записи сообщений в журнал и консольное приложение, которое демонстрирует её работу. Библиотека поддерживает три уровня важности сообщений: INFO, WARNING и ERROR.

## Особенности

- Запись сообщений в текстовый файл.
- Фильтрация сообщений по уровню важности.
- Многопоточная обработка сообщений.
- Простое консольное приложение для тестирования.

## Требования

- Компилятор `g++` (поддерживающий стандарт C++17).
- Операционная система: Linux (например, Ubuntu/Debian).

## Сборка проекта

1. Клонируйте репозиторий:
   ```bash
   git clone https://github.com/ваш-логин/loging_project.git
   cd loging_project

2. Соберите проект:
make
Это создаст:

Динамическую библиотеку liblogger.so.

Исполняемый файл my_app.

3. Очистите проект (удалите скомпилированные файлы):
make clean
