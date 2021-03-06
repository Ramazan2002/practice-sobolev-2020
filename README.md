# Руководство по загрузке домашнего задания

1. Прежде чем начать делать домашнее задание нужно перейти в папку с репозиторием и создать ветку. Например, если дз
было задано 3 сентября 2020 года, то ветка должна иметь название `hw_03-09-20`.
```
cd %PATH_TO_REPO%
git checkout -b hw_03-09-20
```
2. В корне репозитория создаете папку с названием как у ветки, то есть `hw_03-09-20`, перейдите в нее и выполняйте дз в ней.
```
mkdir hw_03-09-20
cd hw_03-09-20
```
3. Выполняя дз, называете файлы строго как указано в задании, **иначе ваши
файлы не пройдут автопроверку**.
4. Добавьте файлы в git
```
git add .                 # добавляет все файлы
git add file1.py file2.py # добавляет каждый файл отдельно
```
5. Создайте коммит. Название у коммита должно быть такое же, как название у ветки.
```
git commit -m "hw_03-09-20"
```
6. Проверьте себя.
```
git status
```
7. Отправьте изменения.
```
git push -u origin <branch-name>
git push -u origin hw_03-09-20 # для нашего примера
```
8. Зайдите в репозиторий на Github, создайте Pull-request c датой дедлайна в названии  в формате `Homework <deadline>`, например `Homework 12-09-20`.
9. **Добавите мой аккаунт (`sviperm`) в разделе Reviwers**

## Примечание
- Если я проверил вашу домашнюю работу до дедлайна и указал на недочеты, то у Вас есть возможность исправить недочеты и получить более высокую оценку:
  - Вы исправляете ошибки;
  - пушите изменения в эту же ветку;
  - **В РАЗДЕЛЕ REVIEWERS ВОЗЛЕ МОЕГО ПРОФИЛЯ НАЖМИТЕ НА КНОПКУ `RE-REQUEST`**, чтобы я получил уведомления о Ваших исправлениях.
- За каждую домашнюю работу можно получить 1 балл:
  - каждое задание оценивается по такому принципу:
    - 0.7 функционал;
    - 0.3 соблюдение PEP8;
  - результаты складываются и делятся на количество заданий;
  - не исключаются допзадания на допбаллы.
