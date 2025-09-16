# Создаем директорию проекта и переходим в нее  
mkdir my-project  
cd my-project  
  
# Инициализируем Git-репозиторий  
git init  
  
# Создаем файл README.md  
echo "# Мой учебный проект" > README.md  
  
# Добавляем файл в индекс и делаем первый коммит  
git add README.md  
git commit -m "Initial commit with README file"  
# Создаем новую ветку и переключаемся на нее  
git branch feature/auth  
git checkout feature/auth  
  
# Или можно сделать это одной командой:  
# git checkout -b feature/auth  
  
# Добавляем новую строку в README  
echo "Функция авторизации в разработке" >> README.md  
  
# Проверяем изменения  
git status  
  
# Добавляем изменения и делаем коммит  
git add README.md  
git commit -m "Add auth development note to README"  
# Переключаемся обратно в основную ветку  
git checkout main  # или git checkout master, если используется master  
  
# Сливаем изменения из feature/auth  
git merge feature/auth  
  
# Удаляем ненужную ветку (опционально)  
git branch -d feature/auth  

