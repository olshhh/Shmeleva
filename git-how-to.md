### Как создать и добавить SSH-ключ? Как клонировать репозиторий? 
---
1. В окне терминала ввести ssh-keygen -t ed25519 -C "...email"
 > git clone https://github.com/...
 
2. ssh-ключ находится в файле id_<file_name>, его необходимо прикрепить в соответствующую форму на github.

3. Чтобы добавить ключ в ssh agent, нужно написать в терминале
> eval ssh-agent -s

И добавить свой приватный ключ в ssh-agent:
> ssh-add ~/.ssh/id_<file_name>

4. Чтобы клонировать репозиторий, нужно написать в терминале
> git clone https://github.com/repository...