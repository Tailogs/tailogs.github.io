# tailogs.github.io

## О проекте

`tailogs.github.io` - это мой личный сайт, который включает в себя различные посты и материалы, написанные с использованием собственного препроцессора на языке C. Этот проект демонстрирует мои навыки в программировании и веб-разработке, а также служит в качестве платформы для размещения моих публикаций и проектов.

## Структура проекта

Вот как организованы файлы и папки в проекте:

- `index.html` - Главная страница сайта.
- `LICENSE` - Лицензия проекта.
- `README.md` - Этот файл.
- `icon/` - Папка с иконками.
  - `icon.png` - Основная иконка сайта.
- `src/` - Исходный код проекта.
  - `main.c` - Основной исходный файл, содержащий код препроцессора.
  - `Makefile` - Makefile для сборки проекта.
  - `*.o`, `*.exe` - Скомпилированные файлы (игнорируются Git).
  - `*.js`, `*.css` - JavaScript и CSS файлы для веб-сайта.
  - `*.txt` - Текстовые файлы, используемые для создания постов.

## Как это работает

Препроцессор, написанный на языке C, читает текстовые файлы с постами, преобразует их в HTML и сохраняет результат в файлы `.html`. Этот процесс включает:

- Обработку разметки (курсив, жирный текст).
- Генерацию HTML-страниц с использованием шаблонов.
- Логирование ошибок и отладочной информации.

### Примеры работы

Рассмотрим пример текстового файла `chan.txt`, который используется для генерации HTML:

**chan.txt**
```
# Заголовок поста
Дата: 2024-09-04
Это *жирный текст* и _курсивный текст_.
---
# Заголовок второго поста
Дата: 2024-09-04
Это второй пост.
```

После запуска препроцессора, результатом будет HTML-файл `chan.html` с преобразованным содержимым.


## Как использовать

### Установка

1. **Склонируйте репозиторий:**

    ```bash
    git clone https://github.com/tailogs/tailogs.github.io.git
    cd tailogs.github.io\src
    ```

2. **Соберите проект:**

    ```bash
    make
    ```

### Использование

1. **Создайте или отредактируйте текстовый файл с постами, например, `chan.txt`.**

2. **Скомпилируйте препроцессор:**

    ```bash
    make
    ```

3. **Запустите скомпилированную программу:**

    ```bash
    xtailogs.exe
    ```

4. **Проверьте результат в `chan.html` в корне проекта.**

## Лицензия

Проект лицензирован под [LICENSE](LICENSE).
