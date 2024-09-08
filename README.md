# Задание 1

## Выбор подхода
Для этого проекта решил использовать Webpack Module Federation по следующим причинам:

- Нет необходимости использовать разыне фреймворки
- Целесообразно использовать общий код разными модулями

## Выделенные модули

Все модули являются микрофронтэндами, включая модуль "Общие компоненты", т.к. требуется одновременное обновление компонентов во всех модулях в случае их изменения

### Общие компоненты 
Т.к. в разных частях приложения используются схожие элементы интерфейса (формы, попапы), то эти элементы можно вынести в общий модуль (сформировать в перспективе дизайн-систему), чтобы обновлять элементы одновременно и обеспечивать консистентный пользовательский опыт, а так же не дублировать код в модулях.

### Форма регистрации
Является ключевым элементом сайта, т.к. стоит на самом входе в воронку CJM. В связи с этим с формами регистраций часто проводятся эксперименты, поэтому целесообразно вынести её в отдельный модуль.

### Форма логина
Обычно форма логина меняется не часто, поэтому можно вынести её в отдельный модуль, чтобы случайно не сломать её обновлениями других компонентов, и иметь возможность тестировать её изолированно. 

### Профиль пользователя
Группа логически связанных компонентов, отвечающая за показ и редактирование профиля пользователя

### Контентная часть
Показ и создание мест

# Задание 2

https://app.diagrams.net/#H0rgba%2Farch-sprint1%2Fsprint_1%2Fsprint1_task2.drawio#%7B%22pageId%22%3A%22BleSmaJVXqo2yb7Co1eL%22%7D
