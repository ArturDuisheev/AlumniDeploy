1. Скачиваем рекомендуемую версию NodeJs для своей ОС. https://nodejs.org/en/download/
2. Переходим в репозиторий. cd alumni-backend-main
3. Устанавливаем node packages. npm i
4. Для запуска проекта в режиме разработки выполняем команду npm run dev.
Все скрипты можно посмотреть в package.json "scripts". Для запуска скрипта выполняем команду npm run Название скрипта
5. Для сборки используем команду npm run build.

Перед сборкой нужно зайти в файл alumni-backend-main/src/entry-pont/main.ts и закоментировать const options, const specs и строку app.use('/api-docs', swaggerUi.serve, swaggerUi.setup(specs));.
Это нужно для отключения Swager'а.

В .env ставим свои JWT_ACCESS_SECRET, JWT_REFRESH_SECRET. 
Ставим свой порт и свой API_URL. 
DB_URL желательно не трогать.

Вот данные от аккаунта MongoDB, на который настроен текущий DB_URL. Я не удалял тестовые сущности, можете их глянуть. Пароли от всех тестовых сущностей пользователей - pass123.

email: alatoo.alumnidb@gmail.com
password: 07nr1Zv3j0dm

Входите через гугл аккаунт, там данные такие же.

Свагер развернут на руте /api-docs:

ваш_url/api-docs


Рабочее пространство postman с большинством рутов, для наглядности.
https://www.postman.com/security-specialist-86217765/workspace/alumni