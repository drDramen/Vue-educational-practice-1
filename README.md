# Vue-educational-practice-1

Створити SPA за допомогою vue-cli

1. В компоненті App.vue розмістити json обєкт user (взяти тут https://jsonplaceholder.typicode.com/users?_limit=1)
2. створити набір компонентів для розподілення та необхідної інформації (відповідно до малюнку компоненти мають бути наступні: CommonInfo(name, username, email), Address(street ...) ), окремо компонент Geo (lat, lng), ContactInfo (phone, site), Company (...)

    - кожен з компонентів повинен вміти приймати параметри з даного обєкту, та відображати у звичайних <p>, (верстка за бажанням)

    - компонент CommonInfo (повинен вміти формувати ініціали з перших літер поля name)

    - компонент Address (повинен вміти формувати один рядок з 4-х полів адреси в одну)

    - компонент Geo (повинен вміти формувати рядок у форматі JSON типу "{"lat": "-37.3159", "lng": "81.1496"}")

    - компонент ContactInfo (повинен формувати номер телефону без частини "x56442")

    - компонент Company (повинен вміти формувати "slug", тобто взяти назву, літери в нижній регістр, пробіли замінити на мінус)

    - компонент "Geo" використати в компоненті "Address", Тобто зробити вложеним

## users

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
