# QUIK Config

- `info.ini`
- `ip.cfg` ('private' branch only)
- `qrypto.cfg` ('private' branch only)

TODO:

- Configuring the limits: `default_client_codes.ini` and `price_limits.ini`
- Grouping instrument classes into instruments markets: `markets.ini`

...

## Updated QUIK settings

| | def | new | description |
| --- | --- | --- | --- |
| **\[data]** |  |  |  |
|  `request-skipped` | 1 | 0 | _Программа - Сохранение данных_ <br> Сохранять для получаемых инструментов и параметров <br> &#x1F5F9; Данные, отражающие текущее состояние и всю историю изменений <br> &nbsp;&nbsp; :black_square_button: Получать пропущенные данные <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; > (влияет на скорость работы) |
| **\[transactions]** |  |  |  |
| `save-dialog-position` | 0 | 1 | _Торговля - Заявки - Формы ввода_ <br> :ballot_box_with_check: Запоминать положение на экране <br> &#x1F5F9; Особо выделять ключевые параметры |
| `change-operation-by-space` | 0 | 1 | _Trading - Orders_ <br> :ballot_box_with_check: Change operation by spacebar |
| `ask-confirmation` | 1 | 0 | _Торговля - Заявки_ <br> :black_square_button: Запрашивать подтверждение <br> &#x1F5F9; Запрашивать подтверждение для групповых операций |
| **\[ClosePositions]** |  |  |  |
| `ask-close-positions-confirmation` | 1 | 0 | _Торговля - Закрытие позиций_ <br> :black_square_button: Запрашивать подтверждение на закрытие позиций <br> &#x1F5F9; Снимать стоп-заявки перед закрытием позиций |
| **\[general]** |  |  |  |
| `client-transaction-ask-confirmation-for-one-request` | 1 | 0 | _Торговля - Заявки - клиентские заявки_ <br> :black_square_button: Запрашивать подтверждение при операциях с клиентскими заявками <br> &#x1F5F9; Запрашивать подтверждение при операциях с группами клиентских заявок |
| `client-transaction-show-request-is-message-window` | 0 | 1 | _Trading - Orders - Client orders_ <br> :ballot_box_with_check: Show description of client order in standart program message window |
| `accept-client-transaction-no-button-is-default` | 0 | 2 | _Trading - Orders - Client orders_ <br> &#x1F5F9; Show description of client order in standart program message window <br> &nbsp;&nbsp; Active button of the client order in standard program message form <br> &nbsp;&nbsp;&nbsp;&nbsp; &#10686; Button yes &nbsp; &#10686; Button "No" &nbsp; &#10687; Button "Cancel" |
| `use-margin-scheme-own` | 0 | 1 | _Trading - Orders_ <br> Order execution <br> &nbsp;&nbsp; :ballot_box_with_check: Calculate according only to own cash |
| `show-other-messages` | 1 | 0 | _Сообщения_ <br> При получении показывать в окне сообщения <br> &nbsp;&nbsp; &#x2610; Отмеченные как важные <br> &nbsp;&nbsp; &#x1F5F9; Ошибки транзакций <br> &nbsp;&nbsp; :black_square_button: Обычные |
| `sort-column-with-ctrl` | 0 | 1 | _Окна - Таблицы_ <br> &#x1F5F9; Плавная подсветка строк <br> :ballot_box_with_check: Сортировать по столбцу, удерживая Ctrl |
| `confirm-dnd-operation` | 1 | 0 | _Окна - Таблицы_ <br> &#x1F5F9; Перемещать и удалять столбцы с помощью drag-and-drop <br> :black_square_button: Запрашивать подтверждение при перемещении и удалении объектов с помощью drag-and-drop |
| **\[qchart-toolbar]** |  |  |  |
|  `magneto-mode` | 0 | 65538 | _Toolbars - Graph - Magent_ |
| **\[regional-settings]** |  |  |  |
|  `primary-lang-id` | 0x19 | 0x09 | Меню: Система > Настройки > Языковые установки... <br> Язык: &nbsp; :arrow_forward: English[Standard Set] |
| **\[excel]** |  |  |  |
|  `language_id` | 1 | 0 | _Программа - Экспорт данных_ <br> Экспорт по DDE <br> MS Excel: &nbsp; :arrow_forward: Английский |

## Updated Connection settings

| | def | new | description |
| --- | --- | --- | --- |
| **\[connect]** |  |  | Меню: Система > Соединения > Просмотр доступных соединений |
|  `auto-reconnect` | 0 | 1 | :ballot_box_with_check: Восстанавливать связь автоматически через ... секунд c ... до ... |
|  `check-tmo` | 250 | 150 | через :arrow_forward: 15 секунд |
|  `do-auto-reconnect-from-time` | 100000 | 94500 | c :clock10: 09:45:00 |
|  `do-auto-reconnect-to-time` | 220000 | 235900 | до :clock12: 23:59:00 |

## Full Order Log: Time and sales

| | def | new | description |
| --- | --- | --- | --- |
| **\[ALL_TRADES_DATA]** |  |  |  |
| `TQBR=SBER` |  |  | _Program - Receiving data - Anonymous trades_ <br> Instriment classes filter <br> &nbsp;&nbsp; &#x1F5F9; MOEX E&B: T+: Shares <br> &nbsp;&nbsp;&nbsp;&nbsp; Sberbank [MOEX E&B: T+: Shares] |
