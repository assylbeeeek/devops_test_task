# devops_test_task
Тестовое задание по DevOps в SolvaTechnology.

Решение задания выполненное в локальной виртуальной машине centos 8.
#Тестовое задание. DevOps
## 1. Основы Linux
### Задание: Напишите команды для выполнения следующих задач:
● Создание директории devops_test в домашнем каталоге.
```
[assylbek@centos ~]$ mkdir ~/devops_test
```
● Создание пустого файла readme.txt в созданной директории.
```
[assylbek@centos ~]$ touch ~/devops_test/readme.txt
```
● Показать текущий путь в терминале.
```
[assylbek@centos ~]$ pwd
/home/assylbek
```
## 2. Основы Git
### Задание: Выполните следующие действия с использованием Git:
● Создайте новый локальный репозиторий.
```
[assylbek@centos ~]$ mkdir devops_repo && cd devops_repo
[assylbek@centos devops_repo]$ git init
Initialized empty Git repository in /home/assylbek/devops_repo/.git/
```
● Создайте файл test.txt, добавьте в него текст “Hello DevOps”.
```
[assylbek@centos devops_repo]$ touch test.txt
[assylbek@centos devops_repo]$ echo "Hello World" > test.txt
```
● Закоммитьте изменения с сообщением “Initial commit”.
```
[assylbek@centos devops_repo]$ git add test.txt
[assylbek@centos devops_repo]$ git commit -m "Initial commit"
[master (root-commit) 3bcba68] Initial commit
 Committer: assylbek <assylbek@centos.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 test.txt
```
● Покажите историю коммитов.
```
[assylbek@centos devops_repo]$ git log
commit 3bcba6898a90ca242e57032cf29362aeef81e859 (HEAD -> master)
Author: assylbek <assylbek@centos.local>
Date:   Wed Nov 27 14:00:43 2024 +0500

    Initial commit
```
## 3. Основы сетевых технологий
### Задание: Ответьте на вопросы:
● Что такое IP-адрес и для чего он используется?

_IP адрес это - уникальный адрес компьтера в компьютерной сети. 
Позволяет компьютерам обмениваться данными в интернете или локальной сети._

● Назовите основные отличия между протоколами TCP и UDP.

_tcp устанавливает соединение перед отправкой данных, а udp не устанавливает соединение перед отправкой.
tcp более надежный, так как делает проверки на ошибки.
udp более быстрый, так как не устанавливает и не управляет соединением, вследствии чего тратит меньше ресурсов и работает быстрее._
## 4. Программирование (Bash или Python)
### Задание: Напишите скрипт на Bash или Python, который выводит числа от 1 до 10.
```
[assylbek@centos devops_repo]$ python3
Python 3.6.8 (default, Sep 10 2021, 09:13:53) 
[GCC 8.5.0 20210514 (Red Hat 8.5.0-3)] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> for i in range(1,11): print(i);
... 
1
2
3
4
5
6
7
8
9
10
```
## 5. Логическое мышление
### Задание: Решите следующую задачу:
● В одном здании находится три лампочки, управляемые тремя выключателями в
другой комнате. Как определить, какой выключатель к какой лампочке относится,
если вы можете зайти в комнату с лампочками только один раз?

Для того, чтобы определить какой выключатель от какой лампочки нужно:
1. Зайти в комнату с выключателями.
   
   ● Включить один выключатель на несколько минут, затем выключить его.
   
   ● Включить второй выключатель.
   
   ● Выключить третий выключатель.
3. Зайти в здание с лампочками.
   
   ● Лампочка, которая выключена и тёплая от первого выключателя.
   
   ● Лампочка, которая включена от второго выключателя.
   
   ● Лампочка, которая выключена от третьего выключателя.
