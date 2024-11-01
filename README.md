# Learn-Ubuntu

Всякие мыслишки:
1. Описать, как отключать доступ по паролю
2. Как настраивать SSH
3. Как можно поймать майнер
4. Как узнать, какие ещё есть доступные аргументы для команд
    - `--help`, `-h`
         - краткая форма бывает иногда занята...
6. Как создавать пользователя и зачем
    - `sudo useradd -m <название пользователя>`
        - `-m`, `--create-home` - create the user's home directory
        - Есть `-p`, `--password PASSWORD` - encrypted password of the new account
            - То есть можно при создании пользователя ему сразу и пароль навесить
    - ? есть ли другие команды
    - ? зачем создавать нового пользователя
        - > Do not run steamcmd while operating as the root user. Doing so is a security risk.
            - https://developer.valvesoftware.com/wiki/SteamCMD#Linux
7. Установка пароля для пользователя
   - `sudo passwd <пароль>`
8. Как изменять права
    - `sudo adduser <название пользователя> sudo`
        - https://askubuntu.com/a/1414685
    - `sudo` - get root previges
    - `adduser` - used for adding users and adding user to groups for more info run `adduser --help`
    - `<название пользователя>` the user to add to the group
    - `sudo` - the group to add the user
9. Как удалить папку и файлы внутри
   - rm -rf <название папки>
     - ? что означают каждая из команд
