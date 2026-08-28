# Реестр блоков кода

> Файл собирается автоматически. Не править руками — правьте разметку ограждений
> в главах и пересоберите.

Каждый блок кода в книге отнесён к одной кучке. Кучка определяется **прогоном через
ядро [BSLexicon](https://github.com/iMironRU/BSLexicon)**, а не по виду листинга:
блок либо исполняется, либо нет, и причина известна точно.

| Кучка | Блоков | Что это |
|---|---:|---|
| `песочница` | 18 | исполняется в тренажёре — кнопка «Запустить», проверяется гейтом |
| `набросок` | 17 | чистый язык, но пока не исполняется: не хватает контекста или точек с запятой |
| `платформа` | 0 | запросы, клиент-сервер, справочники — тренажёр этого не умеет по замыслу |
| `шаблон` | 1 | форма конструкции с плейсхолдерами в угловых скобках |
| `ловушка` | 0 | код, показанный нарочно неверным или бесконечным |
| `текст` | 12 | не код: таблица данных, вывод программы, дерево, схема, проза |
| **всего** | **48** | |

## Что с этим делать

**`песочница`** — готово. Гейт следит, чтобы оставалось исполнимым.

**`набросок`** — резерв. Каждый такой блок может стать песочницей, если дописать
недостающее. Но это правка **текста книги**, а не разметки: где-то контекст задан
в соседнем абзаце нарочно, и дублировать его в листинге — испортить подачу.
Решение по каждому — авторское.

**`платформа`**, **`шаблон`**, **`ловушка`** — так и останутся. Машина их не
проверит: тренажёр не знает языка запросов, плейсхолдер не является кодом,
а ловушка неисправна намеренно.

**`текст`** — вообще не код.

## `песочница` — 18

| Где | Первая строка | Почему |
|---|---|---|
| [chapters/02_heshirovanie/02-01_urok.md:57](../chapters/02_heshirovanie/02-01_urok.md) | `// Требования:` | исполняется |
| [chapters/02_heshirovanie/02-01_urok.md:131](../chapters/02_heshirovanie/02-01_urok.md) | `// Требования:` | исполняется |
| [chapters/02_heshirovanie/02-01_urok.md:166](../chapters/02_heshirovanie/02-01_urok.md) | `// Требования:` | исполняется |
| [chapters/03_hranenie-parolej/03-01_urok.md:92](../chapters/03_hranenie-parolej/03-01_urok.md) | `// Требования:` | исполняется |
| [chapters/03_hranenie-parolej/03-01_urok.md:154](../chapters/03_hranenie-parolej/03-01_urok.md) | `// Требования:` | исполняется |
| [chapters/04_klyuchi-sertifikaty-provajdery/04-01_urok.md:163](../chapters/04_klyuchi-sertifikaty-provajdery/04-01_urok.md) | `// Требования:` | исполняется |
| [chapters/04_klyuchi-sertifikaty-provajdery/04-01_urok.md:187](../chapters/04_klyuchi-sertifikaty-provajdery/04-01_urok.md) | `// Требования:` | исполняется |
| [chapters/04_klyuchi-sertifikaty-provajdery/04-01_urok.md:232](../chapters/04_klyuchi-sertifikaty-provajdery/04-01_urok.md) | `// Требования:` | исполняется |
| [chapters/05_shifrovanie/05-01_urok.md:59](../chapters/05_shifrovanie/05-01_urok.md) | `// Требования:` | исполняется |
| [chapters/05_shifrovanie/05-01_urok.md:117](../chapters/05_shifrovanie/05-01_urok.md) | `// Требования:` | исполняется |
| [chapters/05_shifrovanie/05-01_urok.md:163](../chapters/05_shifrovanie/05-01_urok.md) | `// Требования:` | исполняется |
| [chapters/06_elektronnaya-podpis/06-01_urok.md:134](../chapters/06_elektronnaya-podpis/06-01_urok.md) | `// Требования:` | исполняется |
| [chapters/06_elektronnaya-podpis/06-01_urok.md:193](../chapters/06_elektronnaya-podpis/06-01_urok.md) | `// Сценарий: есть текст документа и подпись к нему (в Base64` | исполняется |
| [chapters/06_elektronnaya-podpis/06-01_urok.md:248](../chapters/06_elektronnaya-podpis/06-01_urok.md) | `// Требования:` | исполняется |
| [chapters/06_elektronnaya-podpis/06-01_urok.md:298](../chapters/06_elektronnaya-podpis/06-01_urok.md) | `// Требования:` | исполняется |
| [chapters/07_realnye-zadachi/07-01_urok.md:160](../chapters/07_realnye-zadachi/07-01_urok.md) | `// Проверить, что сертификат действителен по датам.` | исполняется |
| [chapters/07_realnye-zadachi/07-01_urok.md:224](../chapters/07_realnye-zadachi/07-01_urok.md) | `// Требования:` | исполняется |
| [chapters/08_diagnostika/08-01_urok.md:210](../chapters/08_diagnostika/08-01_urok.md) | `Попытка` | исполняется |

## `набросок` — 17

| Где | Первая строка | Почему |
|---|---|---|
| [chapters/01_zachem-nuzhna-kriptografiya/01-01_urok.md:67](../chapters/01_zachem-nuzhna-kriptografiya/01-01_urok.md) | `// Требования:` | чистый язык, не хватает контекста |
| [chapters/02_heshirovanie/02-01_urok.md:102](../chapters/02_heshirovanie/02-01_urok.md) | `// Вспомогательная функция: ДвоичныеДанные → HEX-строка` | runtime: «Новый»: неизвестный тип «БуферДвоичныхДанны |
| [chapters/03_hranenie-parolej/03-01_urok.md:71](../chapters/03_hranenie-parolej/03-01_urok.md) | `СтрокаСольИПароль = Соль + Пароль` | parser: Ожидалось «;», получено «ДвоичныеДанные» |
| [chapters/05_shifrovanie/05-03_otvety.md:63](../chapters/05_shifrovanie/05-03_otvety.md) | `// Строка → Base64 → Строковый реквизит` | чистый язык, не хватает контекста |
| [chapters/07_realnye-zadachi/07-01_urok.md:34](../chapters/07_realnye-zadachi/07-01_urok.md) | `// Шаг 1: вычислить хеш файла` | runtime: Ошибка при вычислении хеша файла: «Новый»: н |
| [chapters/07_realnye-zadachi/07-01_urok.md:87](../chapters/07_realnye-zadachi/07-01_urok.md) | `// Требования:` | runtime: Ошибка при шифровании токена: «Новый»: неизв |
| [chapters/07_realnye-zadachi/07-01_urok.md:315](../chapters/07_realnye-zadachi/07-01_urok.md) | `// HMAC-SHA256: используется в AWS Signature, Telegram Bot A` | чистый язык, не хватает контекста |
| [chapters/08_diagnostika/08-01_urok.md:57](../chapters/08_diagnostika/08-01_urok.md) | `Не удалось найти сертификат. ` | parser: Конструкция «Не» пока не поддерживается ядро |
| [chapters/08_diagnostika/08-01_urok.md:70](../chapters/08_diagnostika/08-01_urok.md) | `// Диагностика: вывести все сертификаты в хранилище` | runtime: «Новый»: неизвестный тип «МенеджерКриптограф |
| [chapters/08_diagnostika/08-01_urok.md:86](../chapters/08_diagnostika/08-01_urok.md) | `Ошибка при создании подписи.` | parser: Ожидалось «;», получено «при» |
| [chapters/08_diagnostika/08-01_urok.md:99](../chapters/08_diagnostika/08-01_urok.md) | `// Проверить доступность закрытого ключа для операции подпис` | runtime: «Новый»: неизвестный тип «МенеджерКриптограф |
| [chapters/08_diagnostika/08-01_urok.md:121](../chapters/08_diagnostika/08-01_urok.md) | `Не удалось расшифровать.` | parser: Конструкция «Не» пока не поддерживается ядро |
| [chapters/08_diagnostika/08-01_urok.md:154](../chapters/08_diagnostika/08-01_urok.md) | `// Диагностика: вычислить хеш документа в двух точках и срав` | чистый язык, не хватает контекста |
| [chapters/08_diagnostika/08-01_urok.md:171](../chapters/08_diagnostika/08-01_urok.md) | `Криптографический провайдер не поддерживает данный алгоритм.` | parser: Ожидалось «;», получено «провайдер» |
| [chapters/08_diagnostika/08-01_urok.md:186](../chapters/08_diagnostika/08-01_urok.md) | `// Для операций с SHA-256 используйте тип 24` | runtime: «Новый»: неизвестный тип «МенеджерКриптограф |
| [chapters/08_diagnostika/08-01_urok.md:199](../chapters/08_diagnostika/08-01_urok.md) | `Срок действия сертификата истёк. (0x800B0101)` | parser: Ожидалось «;», получено «действия» |
| [chapters/08_diagnostika/08-03_otvety.md:86](../chapters/08_diagnostika/08-03_otvety.md) | `МенеджерКрипто = Новый МенеджерКриптографии;` | runtime: «Новый»: неизвестный тип «МенеджерКриптограф |

## `шаблон` — 1

| Где | Первая строка | Почему |
|---|---|---|
| [chapters/08_diagnostika/08-01_urok.md:227](../chapters/08_diagnostika/08-01_urok.md) | `// Вывести всё что важно знать о сертификате перед использов` | плейсхолдеры в угловых скобках |

## `текст` — 12

_Списком не приводится: это не код._

