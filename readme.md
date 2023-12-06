Модуль расширяющий возможности yaml. Позволяет писать в yaml файл переменные окружения в виде:
~~~
facility: ${CI_COMMIT_REF_NAME}
~~~
через использование дженерика в модели конфигурации
~~~go
Env[string|int]
~~~
допускается использовать несколько переменных окружения в одном узле yaml, например:
~~~
facility: ${SYSTEM_NAME}_${APP_NAME}
~~~