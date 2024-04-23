Данный репозиторий содержит тестовые сценарии требований к продукту компании "Ростелеком Информационные технологии". 

Тестовые сценарии проверяют формы "Авторизация" и "Регистрация" сайта компании Ростелеком.

Для написания автотестов применялись следующие техники тест-дизайна:
1. Классы эквивалентности. 
2. Граничные значения.

Данные техники были использованы для проверки таких элементов, как имя, фамилия и пароль формы "Регистрация", поскольку в требованиях к их заполнению указано, что данные элементы должны содержать определенное число символов.

Для этого были определены эквивалентные классы и границы для каждого из них, затем выбраны по одному значению для каждого класса, значения, находящиеся на границе этих классов с минимальным отклонением, а также само граничное значение. 

Как запускать тесты.

Установить все требования:

pip3 install -r requirements
Загрузите Selenium WebDriver с https://chromedriver.chromium.org/downloads (выберите версию, совместимую с вашим браузером)

Запустите тесты:

python -m pytest -v --driver Chrome --driver-path C:/seleniumdriver/chromedriver.exe tests/test_rtc.py
