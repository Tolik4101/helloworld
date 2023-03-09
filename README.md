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

1. В локальной копии репозитория создайте локальную ветку patch1.

`git checkout -b ...`

<img width="825" alt="Снимок экрана 2023-03-08 в 19 53 12" src="https://user-images.githubusercontent.com/102604371/224071320-190b4c85-e817-44e1-93ac-3e03bc5fa17a.png">

2. Внесите изменения в ветке patch1 по исправлению кода и избавления от using namespace std;.

<img width="708" alt="Снимок экрана 2023-03-08 в 20 01 33" src="https://user-images.githubusercontent.com/102604371/224071546-ed1d944f-d611-407d-8c15-1f925283c824.png">

3. commit, push локальную ветку в удалённый репозиторий.

<img width="851" alt="Снимок экрана 2023-03-08 в 20 02 59" src="https://user-images.githubusercontent.com/102604371/224071807-c6606a27-79ab-438d-bcf2-ba1f0ef4d7ef.png">

4. Проверьте, что ветка patch1 доступна в удалёный репозитории.

<img width="1404" alt="Снимок экрана 2023-03-08 в 20 03 43" src="https://user-images.githubusercontent.com/102604371/224071961-b2b49097-5f6d-4449-9c91-d73797932b73.png">

5. Создайте pull-request patch1 -> master.

`git pull origin main`

6. В локальной копии в ветке patch1 добавьте в исходный код комментарии.

<img width="841" alt="Снимок экрана 2023-03-08 в 20 09 04" src="https://user-images.githubusercontent.com/102604371/224072639-0c9e1d02-b4f9-4cba-aba1-92045cb20da7.png">

7. commit, push.

<img width="1413" alt="Снимок экрана 2023-03-08 в 20 10 22" src="https://user-images.githubusercontent.com/102604371/224072849-9bdf6771-7e6d-4163-9e12-d8e02356ef95.png">

8.Проверьте, что новые изменения есть в созданном на шаге 5 pull-request

<img width="1425" alt="Снимок экрана 2023-03-08 в 20 07 09" src="https://user-images.githubusercontent.com/102604371/224072542-0aea64ee-8351-49b8-8cf3-7d44f29a58dc.png">

9.В удалённый репозитории выполните слияние PR patch1 -> master и удалите ветку patch1 в удаленном репозитории.

`git merge patch1`

<img width="1411" alt="Снимок экрана 2023-03-08 в 20 29 36" src="https://user-images.githubusercontent.com/102604371/224073980-fa91d486-861f-4c8e-a18e-56f45913a358.png">

10. Локально выполните pull.

11. С помощью команды git log просмотрите историю в локальной версии ветки master.

`git log`

<img width="840" alt="Снимок экрана 2023-03-08 в 20 36 02" src="https://user-images.githubusercontent.com/102604371/224073892-cf1be1f5-7056-451a-b791-84712df28af9.png">

12. Удалите локальную ветку patch1.

`git branch -d ...`

<img width="842" alt="Снимок экрана 2023-03-08 в 20 25 06" src="https://user-images.githubusercontent.com/102604371/224074157-9a95453a-b12a-45c5-9b2b-73d54b628805.png">

# PART III

1. Создайте новую локальную ветку patch2.

`git checkout -b ...`

2. Измените code style с помощью утилиты clang-format. Например, используя опцию -style=Mozilla.

`clang-format -i --style=Mozilla`

3. commit, push, создайте pull-request patch2 -> master.

<img width="1414" alt="Снимок экрана 2023-03-08 в 20 53 20" src="https://user-images.githubusercontent.com/102604371/224075829-191f6b5e-2b2d-427c-a266-d12b173d6c31.png">

4. В ветке master в удаленном репозитории измените комментарии, например, расставьте знаки препинания, переведите комментарии на другой язык.

5. Убедитесь, что в pull-request появились конфликтны.

<img width="1398" alt="Снимок экрана 2023-03-08 в 21 10 17" src="https://user-images.githubusercontent.com/102604371/224076151-31a3833e-a30d-42aa-99b8-be26a1d634f1.png">

6. Для этого локально выполните pull + rebase (точную последовательность команд, следует узнать самостоятельно). Исправьте конфликты.

`$ git pull origin main --rebase`

7. Сделайте force push в ветку patch2
<img width="741" alt="Снимок экрана 2023-03-08 в 21 29 36" src="https://user-images.githubusercontent.com/102604371/224076769-7e390b84-541e-4d92-b885-e61d1adc9219.png">

`git push --force`

8. Убедитель, что в pull-request пропали конфликтны.
 <img width="1401" alt="Снимок экрана 2023-03-08 в 21 28 20" src="https://user-images.githubusercontent.com/102604371/224076490-3bbdb99e-b6f0-4f66-bb52-0ee7f6ff90c8.png">
 
 9. Вмержите pull-request patch2 -> master.

`git merge`





