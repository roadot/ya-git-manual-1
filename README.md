# H2 Подсказки по GIT


git init - инициализация
git add --all - добавить
rm .git
git commit -m "comment"
git status
git log - посмотреть историю коммитов

Генерация SSH
ssh-keygen -t ed25519 -C "Email привзянный к GitHUB"
или 
ssh-keygen -t rsa -b 4096 -C "Email привзянный к GitHUB"
* passphrase можно не указывать поначалу - это пароль на ключ )

Копирование ключей .pub
Перейти в папку cd ~/.ssh
открыть файл cat *.pub
Скопировать содержимое
Вставить в GitHub -> Settings -> SSH and GPG Keys -> New SSH Key:
Title: название ключа
Key Type: Authentication Key
Key: Вставить из буфера скопированный ключ
нажать ADD SSH key

Проверить ключ: ssh -T git@github.com
Убедиться, что репозитории связаны: git remote -v

Перый раз свзяать ветку:
git push -u origin master


регистрация на GitHub

cd ~/dev/first-project/
git remote add origin git@github.com:roadot/ya-git-manual-1.git
