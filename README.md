Consegui criar playbook postgresql
criei as task para instalar dependencias postgresql, adicionar a chave do repositorio, atualizar cache e validar que esta ativo (se nao reinicia)
criei um handler para reiniciar o porgresql
criei o ficheiro db.yml
alterei o hosts para adicionar o meu ip para o bd.
Nunca o consegui aceder ao meu ip, tive sempre erro de autentição (publicKey). Mudei no hosts para ter como preferencia autenticação por password, tentei mudar as minhas configurações /etc/ssh/sshd_config.d/ para aceitar chave, mas nunca tive sucesso.

Depois criei o token no github e fiz push dos ficheiros adicionado e alterados.
