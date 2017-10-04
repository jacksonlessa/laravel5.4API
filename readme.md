## Instalação do projeto

```
composer install
php artisan key:generate
```

Ao rodar o comando será solicitado o nome de usuário do apache, o padrão é "www-data", caso esteja no servidor de produção ou homologação, verificar antes de instalar.

**Arquivo .env**

Se necessário, editar o arquivo .env de acordo com os dados do ambiente.

**Criação do banco de dados**

```
mysql -uroot -proot -e "create database laraveloauth;"
```

**Criação das tabelas do banco de dados**

```
php artisan migrate:refresh --seed
```
