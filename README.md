# Лабораторная работа №6: Система контроля версий
## Цель работы
Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием. 
## Ход работы
### 1. Создание аккаунта на сайте GitHub
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/1.png)
### 2. Создание копии репозитория
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/2.png)

### 3. Установка Git
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/3.png)

### 4. Настройка клиента Git
```sh
git config --global user.name "4217 Lavelina A. S."
git config --global user.email "loliklovelik@gmail.com"

```
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/4.png)

### 5. Клонирование личного удалённого репозитория на компьютер
```sh
 git clone + [ссылка на репозиторий]

```
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/5.png)

### 6. Добавление файла в удаленный репозиторий, подтягивание изменений
Добавила файл `new` через интерфейс GitHub. Подтянула изменения в локальный репозиторий \
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/6.png)
### 7. История операций 

```sh
git log
```
Ветка master \
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/7.png)
Ветка branch1 \
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/6.png)
### 8. Последние изменения

```sh
git show

```
Ветка master \
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/9.png)
Ветка branch1 \
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/10.png)


### 9. Слияние в ветку master и удаление побочной ветки
```sh
git merge branch1
git add .
git commit -m"merger"

```
Слияние \
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/11.png)

Файл до разрешения конфликта \

Конфликт возник из-за того, что файлы содержали в себе две противоречущие информации. Конфликт был решен путём удаления лишних строк в файле.

Файл после разрешения конфликта \


### 10. Несколько изменений
```sh
git add .
git commit -m"changes2"
git add .
git commit -m"changes3"
```
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/12.png)

### 11. Откат последнего коммита
```sh
git revert + [id последнего коммита]
```
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/13.png)
### 11. Создание ветки для отчёта
```sh
git branch otchet
```
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/14.png)
### 12. История операций
```sh
git log --pretty=format:'%h %cd | %an | %s' --date=format:'%F %R'

```
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/15.png)
### 13. Загрузка изменений в удалённый репозиторий
```sh
git push origin otchet
```
![изображение](https://github.com/loliklovelik/LR6/blob/otchet/photos/16.png)
## Вывод
В ходе данной лабораторной работы были изучены базовые возможности системы управления версиями и был получен опыт работы с Git Api, локальным и удаленным репозиторием.
