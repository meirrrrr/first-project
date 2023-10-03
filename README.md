# Hello this is my project for learn git commands.
---
## Also learn some terminal commands like:
1. mkdir
2. touch
3. pwd
4. cp
5. mv
6. rm
---
## Git commands:
1. git add
2. git commit
3. git log
4. git status
5. git push
---
Code highlighter
```
<h1>Guess My Number!</h1>
      <p class="between">(Between 1 and 20)</p>
      <button class="btn again">Again!</button>
      <div class="number">?</div>
```
---
## Head
Файл head - один из служебный файлов папки .git . Он указывает на коммит, который сделан последним (то есть самый новый). 
Когда делаем коммит, Git обновляет refs/heads/master записывает в него хеш последнего коммита. Получается, что HEAD тоже обновляется, так как ссылается на refs/heads/master.

---
## Статусы файлов в git
![Цикл](https://pictures.s3.yandex.net/resources/M2_T5_1686651284.png)
1. Файл только создан. Git про него еще не знает. Состояние **untracked**
2. Файл добавили в staging area с помощью **git add**.
   - Возможно, изменили файл ещё раз. Состояния: staged, modified (+ tracked).
   - Ещё раз выполнили git add. Состояние: staged (+ tracked).
3. Сделали коммит с помощью **git commit**. Состояние **tracked**.
4. Изменили файл. Состояние: **modified (+ tracked)**.
5. Снова добавили в staging area с помощью **git add**. Состояния: **staged (+ tracked)**.
6. Сделали коммит. Состояния: **tracked**.
---
## git amend
- `--amend` рассчитан на работу с последним коммитом (HEAD).
- Дополнить коммит новыми файлами можно с помощью git commit `--amend --no-edit` . Благодаря опции --no-edit сообщение к коммиту останется таким, каким и было.
- Изменить сообщение к коммиту позволяет команда `git commit --amend -m "Обновлённое сообщение коммита"`.

