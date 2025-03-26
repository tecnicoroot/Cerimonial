Crianto usuário no mysql:
                usuário                             senha
create user 'cerimonial'@'localhost' identified by 'cerimonial';
grant all privileges on *.* to 'cerimonial'@'localhost';
FLUSH PRIVILEGES;

Criação composer init