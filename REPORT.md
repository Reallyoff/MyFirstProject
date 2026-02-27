# Отчет по практической работе  
## «Введение в систему контроля версий Git»

**Выполнил:** Беков Сергей ИС-301  
**Дата:** 27.02.2026  

---

## 1. Цель работы  
> Научиться основам работы с Git:  
> - инициализация репозитория  
> - создание коммитов  
> - работа с ветками  
> - разрешение конфликтов  
> - публикация проекта на GitHub  

---

## 2. Выполненные этапы  
### Часть 1. Локальная работа  
####  Этап 1–3: Инициализация и первые коммиты  
Были выполнены следующие команды:
git init
git add index.html
git commit -m "feat: create index page"
git commit -m "feat: add description"

---

####  Этап 4: Работа с ветками  
git checkout -b develop
git add styles.css
git commit -m "feat: add styles"
git checkout master
git merge develop

---

####  Этап 5: Разрешение конфликта  
Был создан конфликт при слиянии веток `master` и `develop`.  
Файл `index.html` содержал маркеры конфликта:
<<<<<<< HEAD
<h1>Главная ветка</h1> ======= <h1>Ветка разработки</h1> >>>>>>> develop ```
Конфликт был разрешён вручную, оставлен заголовок:
<h1>Главная ветка разработки</h1>

---

Часть 2. Работа с GitHub

---

 Этап 6: Публикация проекта
git remote add origin https://github.com/Reallyofff/MyFirstProject
git push -u origin master

---

 Этап 7: Клонирование и работа с веткой
cd Desktop/FriendProject
git clone https://github.com/Reallyofff/MyFirstProject
cd MyFirstProject
git checkout -b feature/contact
notepad contact.html
git add .
git commit -m "feat: add contact page"
git push -u origin feature/contact

---

Этап 8: Pull Request
На GitHub был создан Pull Request из ветки feature/contact в master.
После проверки изменений выполнено слияние.
Локальный репозиторий обновлён командой:
git pull origin master


---

3. Скриншоты

Скриншот_1.
Конфликт в терминале

<img src="https://raw.githubusercontent.com/Reallyoff/MyFirstProject/master/screenshot1.png" width="500">

Скриншот_2.
Маркеры конфликта в файле

<img src="https://raw.githubusercontent.com/Reallyoff/MyFirstProject/master/screenshot2.png" width="500">

Скриншот_3.
Граф коммитов

<img src="https://raw.githubusercontent.com/Reallyoff/MyFirstProject/master/screenshot3.png" width="500">

Скриншот_4.
Создание репозитория

<img src="https://raw.githubusercontent.com/Reallyoff/MyFirstProject/master/screenshot4.png" width="500">

Скриншот_5.
Репозиторий на GitHub

<img src="https://raw.githubusercontent.com/Reallyoff/MyFirstProject/master/screenshot5.png" width="500">

Скриншот_6.
Создание Pull Request

<img src="https://raw.githubusercontent.com/Reallyoff/MyFirstProject/master/screenshot6.png" width="500">

Скриншот_7.
Успешное слияние

<img src="https://raw.githubusercontent.com/Reallyoff/MyFirstProject/master/screenshot7.png" width="500">

---

4. Используемые команды

 git init(Инициализация репозитория), git add(Добавление файлов в индекс),git commit -m "message"(Создание коммита),git checkout -b branch_name(Создание и переход в новую ветку),git merge branch_name(Слияние веток),git remote add origin URL(Подключение удалённого репозитория),git push -u origin branch( Отправка ветки на GitHub),git pull origin branch(Получение изменений с GitHub),git log --graph --oneline(Просмотр истории коммитов)	                                

---


