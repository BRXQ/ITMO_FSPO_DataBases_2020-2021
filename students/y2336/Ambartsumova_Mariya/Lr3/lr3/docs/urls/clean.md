## Таблица "Уборка"

| Поле             | Тип данных | Первичный ключ | Внешний ключ | Уникальность | Ограничения  |
| -----------------| -----------| -------------  | -------------| -------------| -------------|
| id               | int        |        +       |       -      |       +      |       -      |
| date             | date       |        -       |       -      |       +      |       -      | 
| time             | time       |        -       |       -      |       +      |       -      | 
| hotel_number_id  | int        |        -       |       +      |       +      |       -      | 
| cleaner_id       | int        |        -       |       +      |       +      |       -      | 
| administrator_id | int        |        -       |       +      |       +      |       -      | 