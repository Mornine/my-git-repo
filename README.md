# my-git-repo
Мое почтение всем смотрящим!

Здесь представлена робкая попытка вспомнить "куда тыкать чтобы было красиво" :)

Задание выполнено в рамках курса разработчиков для банка ПСБ.

# Задачи
1. Создать репозиторий
2. Клонированровать репозиторий
3. Добавить файлы и коммит
4. Использовать `.gitignore`
5. Слить ветки и разрешить конфликты

## Дополнительные материалы
* pov: Когда после перерыва попросили сделать простенькие действия на гитхабе
![pov:Когда после перерыва попросили сделать простенькие действия на гитхабе:](https://sun9-78.userapi.com/impg/fhCAaJolP1l-dS3opL_eFDG58lQZykTfxYQbPQ/JaRlGJCtOvE.jpg?size=726x636&quality=96&sign=828a37cddc3966c0944ea0cb779a2757&type=album)

* Сектор анекдот на барабане! [^1]
```
В дверь постучали 10.000 раз.
«Стар Платинум» - догадался Штирлиц
```
[^1]:Я ценитель анекдотов категории Б, но мы тут приличные люди, поэтому просто локальный анекдот!

## V2: Конфликт слияния
Исправлено: Был более корректно воспроизведен конфликт при слиянии двух веток на примере файла index_v2.html.
![Скриншот консоли с конфликтом](/PIC/CONFLICT.png)

Содержимое файла index_v2.html.  
![Скриншот с конфликтующим содержимым](/PIC/CONFLICT_2.png)

Конфликт решен в сторону содержимого файла index_v2.html из ветки feature-branch

## Экстра задание
Так как история коммитов может быть немного путанной (учитывая удаление веток и переделывание основного задания) я написала небольшие пояснения к тому, что и как я делала.
1. Создана ветка test-branch и в ней переименован коммит (c9f05f0)  
2. Сделан файл file_for_replace.txt и сделан коммит для переноса (т.е. коммит который мы планируем перенести в другую ветку) (61af01c)  
3. Создана ветка feature-x и перенесен (скопирован) коммит туда с помощью cherry-pick  
4. Внесли изменения в файл file_for_replace.txt, залили на сервер  
5. Сделали ответвление feature-X - ветку feature-Y  
6. Внесли еще изменения file_for_replace.txt 
7. Удалили ветку feature-X с сервера   
8. Слили feature-Y и main.Так как конфликтов не было обнаружено ветка слилась через fast-forward - коммит мерджа не был создан, но коммиты из feature-Y залились в ветку main.  
