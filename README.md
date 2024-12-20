# Проєкт Анотації і рефлексія в Java

## Автор
- **Скомороха Олег Ігорович**
- **Телеграм**: [@olegskomoroha](https://t.me/olegskomoroha)
- **Email**: [oleg.skomoroha1@gmail.com](mailto:oleg.skomoroha1@gmail.com)
  
## Група
  ІО-25

## Опис проєкту
  Цей проект передбачає створення системи для генерації Sql запитів для управління користувачами, продуктами та замовленнями, з даними, що зберігаються в базі даних.
Проект використовує **JPA (Java Persistence API)** для зв'язування цих сутностей з таблицями бази даних, що дозволяє виконувати операції CRUD (Створення, Читання, Оновлення, Видалення) для користувачів, продуктів та замовлень.

## Основний клас
  **SqlGenerator**: Цей клас є універсальним інструментом для генерації SQL запитів для операцій **CREATE**, **INSERT**, **UPDATE** та **DELETE** для об'єктів, що відображаються на таблиці в базі даних за допомогою анотацій JPA.

## Класи для демонстрації
  1. **User**: Представляє користувача в системі, з такими властивостями як `id`, `name` (ім'я) та `age` (вік).
  2. **Product**: Представляє продукт, з атрибутами як `id`, `title` (назва) та `price` (ціна).
  3. **Order**: Представляє замовлення, яке зробив користувач, з такими деталями як `orderId` (ідентифікатор замовлення), `userId` (ідентифікатор користувача) та `amount` (сума замовлення).
## Висновки 
  За допомогою методу SqlGenerator ми змогли створити механізм для генерації SQL-запитів для різних типів даних.
**Рефлексія** дозволяє значно скоротити кількість повторюваного коду та робить програму більш гнучкою та динамічною. 
Однак цей метод має певні недоліки, такі як зниження продуктивності через додаткові операції з відображенням класів та полів.
Це було продемонстровано у вимірюванні часу виконання, де процес із рефлексією виявився повільнішим за звичайну ручну генерацію SQL-запитів.

## Вимоги
  - Java 20 або вище

## Інструкції з побудови та запуску

### 1. Клонуйте репозиторій собі на комп'ютер
  git clone https://github.com/olehskomorokha/java-advanced-lab2.git
  
### 2. Запуск проекту: 
  Запустіть головний клас Main
