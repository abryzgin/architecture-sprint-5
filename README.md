# Rasa Chatbot Configuration and Logs

репозиторий содержит конфигурационные файлы, сценарии, логи и примеры взаимодействия с чат-ботом, разработанным на платформе [Rasa](https://rasa.com/).

## Структура проекта

- **Конфигурационные файлы и сценарии Rasa:**
    - [stories.yml](rasa_cfg/stories.yml) — сценарии диалогов.
    - [rules.yml](rasa_cfg/rules.yml) — правила работы чат-бота.
    - [nlu.yml](rasa_cfg/nlu.yml) — тренировочные данные для обработки естественного языка.
    - [domain.yml](rasa_cfg/domain.yml) — описание сущностей, намерений и ответов бота.

- **Примеры взаимодействия с чат-ботом:**
    - ![fragment of dialogue.png](fragment%20of%20dialogue.png) — скриншот фрагмента диалога.
    - [full dialogue.mov](full%20dialogue.mov) — видео полного диалога.

- **Логи работы Rasa:**
    - [log_rasa.log](log_rasa.log) — лог работы чат-бота для анализа и отладки.

## Установка и запуск

Для тренировки чат-бота:
```bash
rasa train
```

Для запуска сервера Rasa с интерфейсом API:
```bash
rasa run --enable-api --cors "*" --log-file=log_rasa.log --debug
```