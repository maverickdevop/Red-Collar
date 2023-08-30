# Проект на позицию Red Collar
 
Проект содержит в себе тестовые сценарии авторизации и создания нового пользователя на странице Battle.net

## Инструменты

- Python 3.10
- Selenium WebDriver
- PyTest
- WebdriverManager
- Allure

## Структура проекта

Положительные сценарии для авторизации в аккаунт
Создание нового пользователя
Дополнительно: Можно создать класс с проверками на негативные сценарии (Ввод пустого/невлидного email/password). Добавить логин для пользователя меньше 18 лет

Проект организован следующим образом:

- `tests/` - директория с тестовыми файлами
- `pages/` - директория с классами страниц (Page Object Model). Здесь содержатся классы, описывающие элементы и поведение каждой страницы приложения.
- `conftest.py` - файл конфигурации для инициализации драйвера. Здесь вы можете настраивать фикстуры, которые будут использоваться в ваших тестовых сценариях.


## Установка и настройка

1. Создайте виртуальное окружение:
   ```shell
   python -m venv venv

2. Установите зависимости из файла requirements.txt:
   ```shell
   pip install -r requirements.txt


3. Для запуска тестов используйте команду:
   ```shell
   pytest tests/* --browser_name=firefox

4. Для визуализации результатов теста можно создать Allure результаты
   ```shell
   pytest tests/* --browser_name=firefox --alluredir=results
   allure serve results
