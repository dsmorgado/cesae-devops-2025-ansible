Consegui criar playbook postgresql
criei as task para instalar dependencias postgresql, adicionar a chave do repositorio, atualizar cache e validar que esta ativo (se nao reinicia)
criei um handler para reiniciar o porgresql
criei o ficheiro db.yml
alterei o hosts para adicionar o meu ip para o bd.
Nunca o consegui aceder ao meu ip, tive sempre erro de autentição (publicKey). Mudei no hosts para ter como preferencia autenticação por password, tentei mudar as minhas configurações /etc/ssh/sshd_config.d/ para aceitar chave, mas nunca tive sucesso.

Depois criei o token no github e fiz push dos ficheiros adicionado e alterados.

Erro:
 ansible-playbook -i hosts db.yml

PLAY [Instalarr PostgreSQL 16] ***************************************************************************************************************************************************************************

TASK [Gathering Facts] ***********************************************************************************************************************************************************************************
fatal: [10.0.2.15]: UNREACHABLE! => {"changed": false, "msg": "Failed to connect to the host via ssh: ubuntu@10.0.2.15: Permission denied (publickey).", "unreachable": true}

PLAY RECAP ***********************************************************************************************************************************************************************************************
10.0.2.15                  : ok=0    changed=0    unreachable=1    failed=0    skipped=0    rescued=0    ignored=0   

