# docker_zabbix_postgresql-
Este arquivo compose para docker serve para instalar  o zabbix com postgresql em qual quer vps ou servidor QUE TENHA DOCKER E DOCKER COMPOSE ou mesmo usar o stack do PORTAINER
com cpus x86/x64 ou ARM64.
apos a instalação inserir o ip no navegado do seu servidor http://0.0.0.0:8182 logar como Admin e senha zabbix 
para corrigir o erro de agent zabbix não colocar o ip do container usar o nome de host como no exemplo abaixo

![zabbix-agent](https://github.com/turbonetlink/docker_zabbix_postgresql-/assets/12984495/2a9c49ea-061a-4fea-af4c-47688ef4436c)
não esqueção de liberar as postas no firewall
51820/udp
51821/tcp 
51413/tcp 
8182/tcp 
10050/tcp 
10051/tcp
10052/tcp
161/tcp
162/udp
fiz usando o ufw 
apt-get install ufw
ufw add porta/tcp
depois que terminar de adicionar  ligue o ufw
ufw enable


se tiver se lascando com o grafana como eu me lasquei segue o que funcionou pra min na imagem abaixo
endereço http://zabbix-frontend:8080/api_jsonrpc.php

![zabbix grafana 1](https://github.com/turbonetlink/docker_zabbix_postgresql-/assets/12984495/0c78cb1b-e86c-4c26-bd23-98411944355f)


espero que ajudem quem esteja se lascando !


