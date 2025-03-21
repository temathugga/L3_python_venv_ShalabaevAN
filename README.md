# Игнорирование виртуальных окружений

Виртуальные окружения содержат зависимости, специфичные для локальной среды разработки. 
Они могут занимать много места и содержать пути, которые не имеют смысла на других машинах. 
Поэтому их следует игнорировать и не включать в репозиторий.

# Почему мы пушим только файлы `requirements`?

Файлы `requirements.txt` (или `req-env1.txt`, `req-env2.txt`) содержат список всех зависимостей, необходимых для проекта. 
Это позволяет другим разработчикам легко воссоздать окружение, установив все зависимости одной командой `pip install -r requirements.txt`. 
Таким образом, мы экономим место в репозитории и упрощаем процесс настройки проекта на других машинах.
