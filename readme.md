Crianto usuário no mysql:
                usuário                             senha
create user 'cerimonial'@'localhost' identified by 'cerimonial';
grant all privileges on *.* to 'cerimonial'@'localhost';
FLUSH PRIVILEGES;

Instalação e configuração do Phinx
composer require robmorgan/phinx

Após a instalação criar o arquivo de configuração phinx na raiz do projeto, para isso devemos rodar o comando: vendor/bin/phinx init
Em seguida devemos criar as pastas:
    '%%PHINX_CONFIG_DIR%%/db/migrations',
    '%%PHINX_CONFIG_DIR%%/db/seeds'
Estas pastas vão organizar as migrations e seeds existentes.
Podemos testar a configuração com o comando: vendor/bin/phinx test
Assim é possivel versionar o banco de dados. 

