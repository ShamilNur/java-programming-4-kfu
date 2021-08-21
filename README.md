# KFU-Programming-Java-4

**Веб-приложение, написанное с использованием Spring MVC Framework, HTML5, CSS3.**

## **Технологии:**
1) Spring MVC, Spring Boot, Spring Security, JPA+Spring Data JPA, AOP (Aspects for Logging)
2) JavaScript+jQuery, AJAX, HTML5, CSS3, Bootstap 4.0
3) REST API
3) PostgreSQL
4) API VK для реализации авторизации по протоколу OAuth2

## **Структура семестровой работы:**

1. **Архитектуры (слои абстракции)**
- Проект основан на Spring Boot и построен по модели MVC, логика *Controller->Service->Repository*.
- Используются DTO-, Forms-классы, где это уменьшает связность, абстрагирует архитектуру.
- Соблюдены принципы SOLID. Весь код корректно поделен на пакеты.

2. **Валидация данных. Работа с базой (репозитории, 4 сущности, M2M, O2M, свои запросы). CRUD**
- Предусмотрена проверка данных, защита от повторной отправки там, где это нужно.
- Приложение имеет аутентификацию, авторизацию, регистрацию. Это реализовано с помощью Spring Security.
- Приложение хранит данные в СУБД PostgreSQL. Для работы с СУБД использовано JPA+Spring Data JPA.
- Система работает с 5 сущностями. Есть связи M2M, O2M.
- Для одной из сущностей полностью реализован CRUD.

3. **HTML5, CSS3, JavaScript**
- Для красивой визуализации применены Bootstrap, JavaScript+jQuery. Использован AJAX.

4. **Использование продвинутых техник/технологий, в т.ч. Spring**
- Логгирование с помощью AOP (для обработки исключений)
- Описание конфигураций, конвертеров, централизованная обработка исключений и т.д.
- Организация REST API для одной сущности (User).

5. **Использование стороннего API. Авторизация по протоколу OAuth 2.0**
- Не использована специальная библиотека для этого API, а самостоятельно описаны запросы на уровне HTTP для авторизации через ВКонтакте.
