# 2 тестовых задания компании HardQode

## 1 задание сделать фильтры пользователей

ссылка на готовое задание: https://codesandbox.io/s/users-app-forked-szfrjd

1. Реализовать показ списка пользователей (имя и возраст через запятую)

2. Показывать текст Loading... при загрузке пользователей вместо списка пользователей.

3. Обработать возможную ошибку при вызове requestUsers (можно проверить при помощи функции requestUsersWithError), показать текст ошибки вместо списка пользователей.

4. Реализовать фильтрацию по имени (передавая в аргументе поле name в функцие requestUsers, например: requestUsers({name: "Jack", ...})). Значение по умолчанию - пустая строка.

5. Реализовать фильтрацию по возрасту (передавая в аргументе поле age в функцие requestUsers - requestUsers({age: "26", ...})). Значение по умолчанию - пустая строка.

6. Реализовать возможность смены страницы и количества элементов на странице - requestUsers({limit: 4, offset: 4, ...}). Здесь offset это не номер страницы, а сдвиг (offset = (page - 1) \* limit), Значения по умолчанию: offset - 0, limit - 4.

7. При получении пустого списка от функции requestUsers показывать сообщение Users not found

## 2 сделать так чтобы выводились имена авторов и отзывы

ссылка на готовое задание: https://codesandbox.io/s/books-mapping-forked-q9swyr

Техническое задание:
// Доработать приложение App, чтобы в отрисованном списке
// были реальные отзывы, автор книги и автор отзыва.
// Данные об отзывах и пользователях можно получить при помощи асинхронных
// функций getUsers, getReviews

// функция getBooks возвращает Promise<Book[]>
// функция getUsers возвращает Promise<User[]>
// функция getReviews возвращает Promise<Review[]>

// В объектах реализующих интерфейс Book указаны только uuid
// пользователей и обзоров

// // В объектах реализующих интерфейс BookInformation, ReviewInformation
// указана полная информация об пользователе и обзоре.
