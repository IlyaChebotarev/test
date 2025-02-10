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
Соберите проект:

```bash
make
Это создаст:

Динамическую библиотеку liblogger.so.

Исполняемый файл my_app.

Очистите проект (удалите скомпилированные файлы):

```bash
make clean
Использование
Запуск приложения
Запустите приложение, указав файл журнала и уровень важности по умолчанию:

```bash
./my_app log.txt 0
log.txt — имя файла журнала.

0 — уровень важности по умолчанию (INFO).

Взаимодействие с приложением
Введите сообщение:

```bash
Введите сообщение: Это тестовое сообщение
Введите уровень важности:

```bash
Введите уровень важности (0 - INFO, 1 - WARNING, 2 - ERROR): 0
Для завершения работы введите exit.

Примеры
Запуск приложения:

```bash
./my_app log.txt 0
Ввод данных:

```bash
Введите сообщение: Приложение запущено
Введите уровень важности (0 - INFO, 1 - WARNING, 2 - ERROR): 0

Введите сообщение: Обнаружена ошибка
Введите уровень важности (0 - INFO, 1 - WARNING, 2 - ERROR): 2

Введите сообщение: exit
Проверка файла журнала:

```bash
cat log.txt
Вывод:

[2023-10-05 14:35:00] [INFO] Приложение запущено
[2023-10-05 14:35:15] [ERROR] Обнаружена ошибка
