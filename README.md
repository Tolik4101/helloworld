# PART I
1. Создайте пустой репозиторий на сервисе github.com

<img width="1407" alt="Снимок экрана 2023-03-08 в 19 26 54" src="https://user-images.githubusercontent.com/102604371/224065623-bd2a587c-486e-4116-973a-1ebccc0a246a.png">

2. Выполните инструкцию по созданию первого коммита на странице репозитория, созданного на предыдещем шаге.
 


3. Создайте файл hello_world.cpp в локальной копии репозитория (который должен был появиться на шаге 2). Реализуйте программу Hello world на языке C++ используя плохой стиль кода. Например, после заголовочных файлов вставьте строку using namespace std;.
<img width="849" alt="Снимок экрана 2023-03-08 в 19 32 21" src="https://user-images.githubusercontent.com/102604371/224066271-b6b0f817-2073-4814-a8e1-da9dd6bf3b40.png">

4. Добавьте этот файл в локальную копию репозитория.
 
 `git init`
 
 `git add helloworld`

5. Закоммитьте изменения с осмысленным сообщением.
 
 `git commit -m ...`

6. Измените исходный код так, чтобы программа через стандартный поток ввода запрашивалось имя пользователя. А в стандартный поток вывода печаталось сообщение Hello world from @name, где @name имя пользователя.
<img width="840" alt="Снимок экрана 2023-03-08 в 19 44 35" src="https://user-images.githubusercontent.com/102604371/224067404-b04b662c-1997-4b89-a2b6-dec94716e09f.png">

`nano helloworld.cpp`

7. Закоммитьте новую версию программы. Почему не надо добавлять файл повторно git add?

Для добавления коммитов остаточно один раз добавить `git add`

8. Запуште изменения в удалёный репозиторий.

`git push -u origin main`

9. Проверьте, что история коммитов доступна в удалёный репозитории.
<img width="1392" alt="Снимок экрана 2023-03-08 в 19 51 51" src="https://user-images.githubusercontent.com/102604371/224069747-21674908-73cc-4bdf-9582-d0dbbf37569f.png">



# PART II

`git checkout -b ...`

`git merge patch1`

`git pull origin main`

`git log`

`git branch -d ...`

# PART III

`git merge`

`git push --force`

`clang-format -i --style=Mozilla`

