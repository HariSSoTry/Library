**Импортируемые модули**
json: используется для работы с JSON-файлами, которые хранят данные о книгах.

**Класс Book**
Этот класс представляет книгу и имеет следующие методы и атрибуты:

Атрибуты:
STATUS_AVAILABLE: Статус "в наличии".
STATUS_ISSUED: Статус "выдана".
id: Идентификатор книги.
title: Название книги.
author: Автор книги.
year: Год издания книги.
status: Статус книги.

Методы:
__init__(self, id, title, author, year, status): Конструктор, который инициализирует объект книги. Проверяет допустимость статуса.
set_status(self, new_status): Метод для изменения статуса книги. Проверяет допустимость нового статуса.

**Класс Library**
Этот класс представляет библиотеку, содержащую книги, и имеет следующие методы:

Атрибуты:
books: Список книг в библиотеке.

Методы:
__init__(self): Конструктор, который инициализирует объект библиотеки и загружает книги из файла.
load_books(self): Загружает книги из файла library.json.
save_books(self): Сохраняет книги в файл library.json.
add_book(self, title, author, year): Добавляет новую книгу в библиотеку.
delete_book(self, book_id): Удаляет книгу из библиотеки по ID.
search_books(self, query): Ищет книги в библиотеке по запросу (название, автор или год).
display_books(self): Показывает список всех книг в библиотеке.
change_status(self, book_id, new_status): Изменяет статус книги по ID.
show_status(self, book_id): Показывает статус книги по ID.

**Функция main()**
Эта функция содержит основную логику программы и предоставляет пользователю меню для взаимодействия с библиотекой:
Основные действия:
Добавить книгу.
Удалить книгу.
Найти книгу.
Показать все книги.
Изменить статус книги.
Показать статус книги.
Выйти из программы.
