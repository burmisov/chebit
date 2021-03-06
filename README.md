# CHEBIT

[Ближайшие мероприятия](#events) | [Задачки](#tasks)

---

Это документация сообщества программистов "ИТ в солнечной Чувашии". Группа в телеграмм: https://t.me/itcheb

Документация поддерживается активными членами сообщества и открыта к изменению.

Ревьюеры:

* Данил Письменный – [@dapi](https://github.com/dapi)
* Александр Баталов – [@abataloff](https://github.com/abataloff)
* Сергей Бурмисов – [@burmisov](https://github.com/burmisov)

Шлите PullRequest-ы.

# Почему и для чего этот репозиторий?

* Нас объединяет увлечение IT технологиями, а именно - программированием.
* У нас есть информация, который мы рады делиться с остальными.
* github - отличное для этого место.

# И все?

А еще это хороший способ показать начинаюми прогаммистам,как проходит работа с изменением общего кода (в нашем случае текстов). Как выглядит обсуждение, как выглядит приемка изменения, кто принимает, почему он, по каким правилам, как формируются эти правила, кто участвует в их обсуждении и т.п. А это важный навык для работы в современной команде.

---

# Tasks

Это тестовые задачки, который могут быть оплачены в случае принятия их заказчиком.

## Задача N1. Монитор логов

Задача: мониторить в реальном времени лог-файл, в случае обнаружения строки с нужным вхождением – запустить указанную программу и передавать ей найденную строку первым параметром.

Пример использования: мы хотим получать сигналы когда происходит посещение нужного адреса на веб-сервере.

Требования:

1. Иметь возможность запуска в режиме команды без ухода в фон.
1. Иметь опцию для запуска в фоновом режиме (режим демона)
2. Корретно обрабатывать ротацию лога.

Пример вызова:

```
# Просмотрит весь access.log и для, каждой строки,
# в которой присутсвует слово index.html запустит
# команду echo с параметром в виде полного содержимого
# этой строки. Завершится после прохождения всего файла.
monitor /var/log/nginx/access.log index.html echo


# Тоже самое, только останется в памяти в виде демона и при каждом появлении нужного вхождения будет запускать команду echo
monitor /var/log/nginx/access.log index.html echo -d
```

Желаемый язык: Ruby, Go, Clojure.

Результат скинуть в виде Pull Request к этому репозиторию в каталоге `./tasks/task1-log_monitor/ВАШ_НИК_НА_GITHUB`

Заказчик: Данил Письменный (техдир Unicornex), danil@brandymint.ru, telegram@pismenny

Дата создания: 23 марта. Результаты принимаются до 15-го апреля.

---

# Events

* Ближайшие мероприятия

## [Draft] 21 Апреля / Миникурс по процессам разработки от Scrum-мастера

Дата проведения: 21.04.2018

Время начала: В первой половине дня (точное время будет позже)

Тезисы: Проект и продукт, их отличия; почему ничего не летит без капитана; ожидания от каждого участника процесса.

Длительность: Примерно 4-5 часов

Место: Предварительно Корпус Б в ЧувГУ ([на карте](https://yandex.com/maps/-/CBelQBtIhA)

Больше информации: Вот [тут](https://www.facebook.com/abataloff88/posts/1732969540095173?pnref=story)

Комментарии: Просьба заполнить [анкету](https://goo.gl/forms/jgF8OSQofWfsJKeD3) для понимания аудитории

## [Draft] 28-29 Апреля, Unitalks
