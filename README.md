# Tasks_beQNmax
cd .. - выход из папки
cd /g:/_beQNmax/2/ - переход в данную папку 

git init - инициирует репозиторий (появится скрытая папка git )
git config --local user.name "Yura"
git config --local user.email yury.sts@gmail.com
В папке git появится файл config со строчками user
Первый раз следует устанавливать глобально. Т.е. gin config --global user.name "Yura"

Рабочие команды:
1-ое состояние
	git status - информация о статусах файлов (файлы красного цвета)
2-ое состояние
	git add -A - добавление файлов в индекс
	git status - за этими файлами git начал следить (файлы зеленого цвета)
	git add main.css - добавляем в индекс новый файл либо
	git add *.css - добавляются все файлы scc
3-ее состояние Добавление файлов в коммит:
	git commit -a -m"first commit" - создание контрольной точки (коммита)
	git status - теперь не покажет отслеживаемых файлов. Теперь будут видны только файлы которые подверглись изменению
	Чтобы закоммитеть нужно присвоить статус 2-го состояния:
	git add -A
	git commit -a -m"second commit"
git log - просмотр списка коммитов

git remote add origin https://github.com/yurasts/Tasks_beQNmax.git - путь с github.com (локальный репозиторий связывается с удаленным)
git push -u origin master - отправляем локальный проект
git push - отправка на репозиторий github.com

Перенос проекта на работу в рабочую папку. через git 
cd .. - выйти из папки
cd work - зайти в рабочую папку
На github.com в област проекта есть кнопка "Clone or download", копируем команду для переноса
git clone - команда производящая клонирование
git clone https://github.com/yurasts/project.git project_2 - project_2 папка в которую будет складываться проект

При слиянии (merge) двух проектов (не сделан git pull перед git push, т.е. пытаемся запушить изменения на измененный проект):
в коммандной строке "ctrl + C" "ctrl + C" ":wq!"

GITIGNORE
