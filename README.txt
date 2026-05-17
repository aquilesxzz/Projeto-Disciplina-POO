README - cadastro-produtos

Instruções rápidas:

1) Coloque a pasta 'cadastro-produtos' dentro da pasta do seu servidor local (ex: XAMPP -> htdocs/, Laragon -> www/).
2) Importe o arquivo backend/create_db.sql no phpMyAdmin ou execute no MySQL para criar o banco 'loja' e a tabela 'produtos'.
3) Ajuste credenciais (se necessário): backend/db_connect.php (por padrão: user=root, senha vazia).
4) Inicie Apache e MySQL e abra no navegador:
   http://localhost/cadastro-produtos/index.php
5) O front usa fetch() para se comunicar com os scripts PHP em backend/*.php.

Observações de segurança e melhorias sugeridas:
- Em produção não use usuário root sem senha. Crie um usuário específico com permissões restritas.
- Valide e sanitizar dados com mais rigor no servidor.
- Implemente CSRF, autenticação, e upload de imagens (se precisar).
- Opcional: trocar statements para PDO e usar transactions onde fizer sentido.
