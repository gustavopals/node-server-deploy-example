acessar render.com

acessar sing in

realizar login

### banco de dados

clique em new postgresql

de um nome ao banco : nodedeploy-pg

selecione uma região : Ohio (Banco e backend devem estar na mesma região para latencia)

selecione o plano : free

create database

nota: internal database url é o link de acesso interno para aplicações hospedadas no render e a external para acessar de outros locais (sua maquina por exemplo)

nota: access control - controle de acessos via IP

### webservice

acessar new -> web service

conecte sua conta do github

selecione o repositório do seu projeto

de um nome para seu web-service: nodedeploy-api

build command: npm i && npm run build && npx prisma migrate deploy

start command: npm run start

clique em advanced 

adicione uma nova variavel de ambiente: DATABASE_URL postgres://nodedeploy_pg_urfd_user:AGP6BHW4OQZFhdMGWM4GHcSU2otg6QGk@dpg-cg15467dvk4ronsb0sag-a/nodedeploy_pg_urfd

clique em create web service

acompanhe o log de deploy








