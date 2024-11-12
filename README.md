# Learn-Ubuntu

Всякие мыслишки:
1. Описать, как отключать доступ по паролю
2. Как настраивать SSH
    - https://selectel.ru/blog/tutorials/how-to-generate-ssh/
    - https://selectel.ru/blog/ssh-keys/
    - https://phoenixnap.com/kb/ssh-to-connect-to-remote-server-linux-or-windows#ftoc-heading-8
    - https://phoenixnap.com/kb/ssh-with-key
    - `cd ..` - чтобы попасть в папку /home
    - `sudo mkdir .ssh`
    - `cd .ssh`
    - `sudo nano authorized_keys`
        - Перенёс в него данные из публичного ключа
3. Как можно поймать майнер
4. Как узнать, какие ещё есть доступные аргументы для команд
    - `--help`, `-h`
         - краткая форма бывает иногда занята...
         - Например у той же `ls` -  `-h`, `--human-readable` - with -l and -s, print sizes like 1K 234M 2G etc.
6. Как создавать пользователя и зачем
    - `sudo useradd -m <имя пользователя>`
        - `-m`, `--create-home` - create the user's home directory
        - Есть `-p`, `--password PASSWORD` - encrypted password of the new account
            - То есть можно при создании пользователя ему сразу и пароль навесить
    - ? есть ли другие команды
    - ? зачем создавать нового пользователя
        - > Do not run steamcmd while operating as the root user. Doing so is a security risk.
            - https://developer.valvesoftware.com/wiki/SteamCMD#Linux
7. Установка пароля для пользователя
   - `sudo passwd <имя пользователя>`
8. Как изменять права
    - `sudo adduser <имя пользователя> sudo`
        - https://askubuntu.com/a/1414685
    - `sudo` - get root previges
    - `adduser` - used for adding users and adding user to groups for more info run `adduser --help`
    - `<название пользователя>` the user to add to the group
    - `sudo` - the group to add the user
    - СУДЯ ПО ВСЕМУ ПРАВА НАДО МЕНЯТЬ ДЛЯ ВСЕХ СОЗДАННЫХ ПОЛЬЗОВАТЕЛЕЙ, иначе можно получать ошибку `<имя пользователя> is not in the sudoers file.`
9. Как проверять, какие права установлены
    - `ls -l ~/.ssh/`
        - **TODO** Выяснить, что значат эти команды
10. Как удалить папку и файлы внутри
   - `rm -rf <название папки>`
   - ? что означают каждая из команд
       - `rm` - скорее всего сокращение от слова **remove**
   - https://rebrainme.com/blog/linux/kak-udalyat-fajly-i-direktorii-v-linux/
11. Как выполнить команду из под конкретного пользователя
    - `sudo -u <имя пользователя> {команда}`
         - `-u`, `--user=user` - run command (or edit file) as specified user name or ID
     - Например `sudo -u <имя пользователя> -s` запустит терминал(shell) из под этого пользователя
         - `-s`, `--shell` - run shell as the target user; a command may also be specified
12. Установка приложений(application)
    - `apt-get`
    - 

# Почитать
1. https://www.pathname.com/fhs/pub/fhs-2.3.html
2. https://www.tutorialspoint.com/unix/what-is-linux.htm
3. 
