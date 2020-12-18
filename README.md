# Отчёт о тестировании KeyValidator

## Краткое описание

15.12.2020 - 16.12.2020 был проведен анализ установочной документации и руководства пользователя, а также функциональное, негативное тестирование и тестирование граничных значений приложения KeyValidator.

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты:
* Замечания к инструкции по установке - [Отсутствие детализации требований ОС и полученного результата после установки в "Инструкция по установке OpenJDK 11"](https://github.com/EvgeniyaSelivanova/3_JAVA_HomeWork_1.1/issues/1)
* Замечания к руководству пользователя - [Отсутствует детализация шагов запуска, вводимых ключей приложения KeyValidator в "Руководство использования KeyValidator"](https://github.com/EvgeniyaSelivanova/3_JAVA_HomeWork_1.1/issues/2) 
* Баг-репорт - [Валидность ключей из "Руководство использования" при проверке в KeyValidator не подтверждена](https://github.com/EvgeniyaSelivanova/3_JAVA_HomeWork_1.1/issues/3)
* Баг-репорт - [Не подтверждена валидность ключей из тестовых данных при проверке в KeyValidator](https://github.com/EvgeniyaSelivanova/3_JAVA_HomeWork_1.1/issues/4)
* Баг-репорт - [Не подтверждена невалидность ключей из тестовых данных при проверке в KeyValidator](https://github.com/EvgeniyaSelivanova/3_JAVA_HomeWork_1.1/issues/5)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* [Инструкция по установке OpenJDK11](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md)
* [Руководство использования KeyValidator](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md)
* [Тест-сьюит приложения KeyValidator](Test_suit.md)

В качестве тестовых данных использовались данные из [Руководство использования KeyValidator](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md):
* 00000000-0000-0000-0000-000000000000 - ожидаемый результат: ОК
* 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998 - ожидаемый результат: ОК
* 80b427f8-92cd-3aae-ba04-3927fbe17c6 - ожидаемый результат: ОК
* b295bc63-9f03-3b4b-af80-969b39f8c262 - ожидаемый результат: ОК
* 387eedc6-12e9-3b32-9881-63b6b5e85317 - ожидаемый результат: ОК
* c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180 - ожидаемый результат: ОК
* 00000000-0000-0000-0000-000000000001 - ожидаемый результат: FAIL
* 18252235-78e0-44a5-8720-556f0c7da17a - ожидаемый результат: FAIL
* e66075b6-ddad-445e-baf6-161b3289522b - ожидаемый результат: FAIL
* b6d53250-f07e-4352-a293-6102ddf7f1ca - ожидаемый результат: FAIL
* c2bc778a-1cb9-46c6-b435-0489649d2a42 - ожидаемый результат: FAIL
* 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1 - ожидаемый результат: FAIL

Тестирование производилось в следующем окружении:
* Версия и разрядность: Windows 10 Корпоративная LTS, 64 - разрядная
* Версия Java: version "11.0.9.1" 2020-11-04

