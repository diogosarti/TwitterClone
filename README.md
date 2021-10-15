# Twitter Clone

Twitter clone com funcionalidades básicas como tweet, sietema de follow, etc.
Link para teste: http://projetotwitterclonecomphp.epizy.com/
usuario padrao: jose@teste.com
senha padrao: teste123

## Desenvolvimento
Feito com PHP, myql e miniFramework PHP

## Screenshot
![Screenshot](img/Twitter-Screenshot-home.png)
![Screenshot](img/Twitter-Screenshot-1.png)
![Screenshot](img/Twitter-Screenshot-2.png)
![Screenshot](img/Twitter-Screenshot-3.png)

## Installation
Importe o querys.sql para o seu mysql database 

### Configuration File

Modifique App/Connection.php de acordo com suas credenciais do banco de dados

``` PHP
//Database Configuration
$conn = new \PDO(
				"mysql:host=localhost.epizy.com;dbname=twitterClone;charset=utf8",
				"root",
				"" 
			);
```

### Htaccess file
```
<IfModule mod_rewrite.c>
	RewriteEngine on
	RewriteCond %{REQUEST_FILENAME} !-f
	RewriteCond %{REQUEST_FILENAME} !-d
	RewriteRule ^(.*)$ index.php/$1 [L]
</IfModule>
```
