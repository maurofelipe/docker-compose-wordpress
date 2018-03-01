# docker-compose-wordpress
Projeto do docker-compose para stack do Wordpress

Passo a passo:<br>
1 - criar as pastas abaixo no mesmo diretório onde estiver o arquivo docker-compose.yml:<br>
dbdata e wwwdata <br>
2 - executar o comando: docker-compose up -d<br>
3 - aguardar alguns minutos e verificar o status dos containers com o comando:<br> docker-compose ps<br>
Deve retornar conforme exemplo abaixo: <br><br>
root@ntd]# docker-compose ps <br>
        Name                       Command               State           Ports         <br>
---------------------------------------------------------------------------------------<br>
wordpress_db_1          docker-entrypoint.sh mysqld      Up      0.0.0.0:3306->3306/tcp<br>
wordpress_redis_1       docker-entrypoint.sh redis ...   Up      0.0.0.0:6379->6379/tcp<br>
wordpress_wordpress_1   docker-entrypoint.sh apach ...   Up      0.0.0.0:80->80/tcp<br><br>
4 - acessar a aplicação usando seu navegador preferido pelo endereço: http://localhost<br>
5 - prosseguir a instalaçao inicial do Wordpress.<br>
FIM.
