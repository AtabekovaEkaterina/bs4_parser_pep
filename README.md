# bs4_parser_pep
В проекте реализован парсер, который поможет вам быть в курсе новостей в мире Python. Функции программы и режимы парсера запускаются через аргументы командной строки.


# Режимы работы парсера:
**whats_new** — собирает ссылки на статьи о нововведениях в Python, переходить по ним и забирать информацию об авторах и редакторах статей.

**latest_versions** — собирает информацию о статусах версий Python.

**download** — cкачивает архив с актуальной документацией.

**pep** — развитие языка Python сопровождается документами PEP и парсер собирает данные обо всех документах PEP:
- сравнивает статусы на странице PEP со статусом в общем списке и записывает в журнал логов несоответствие
- считает количество PEP в каждом статусе и общее количество PEP


# Программа умеет выводить данные следующими способами:
- построчно по умолчанию
- в виде таблицы
- записывать в файл


# Технологии
![image](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue) Python 3.9


# Инструкция по запуску
1. Клонируйте репозиторий 
```
git@github.com:AtabekovaEkaterina/bs4_parser_pep.git
```
2. В дирктории проекта создайте и активируйте виртуальное окружение, обновите менеджер пакетов pip:
```
python3 -m venv venv
```
```
source venv/bin/activate
```
```
python -m pip install --upgrade pip
```
3. Установите зависимости из файла requirements.txt
```
pip install -r requirements.txt
```


# Инструкция по работе с парсером
Для работы с парсером необходимо перейти в директорию scr
1. Получить справку по аргументам командной строки:<br/> 
` python main.py -h` или `python main.py --help`
2. Запустить парсер в нужно режиме работы с выводом данных по умолчанию:<br/>
`python main.py {указать необходимый режим}`
3. Дополнительный способ вывода данных в таблицу:<br/>
`python main.py {указать необходимый режим} -o pretty`<br>
или<br>
`python main.py {указать необходимый режим} --output pretty`
4. Дополнительные способ сохранения данных в файл:<br/>
`python main.py {указать необходимый режим} -o file`<br>
или<br>
`python main.py {указать необходимый режим} --output file`
5. Очистка кеша:<br/>
`python main.py {указать необходимый режим} -c`<br>
или<br>
`python main.py {указать необходимый режим} --clear-cache`


# Автор
Екатерина Атабекова<br>
