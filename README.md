GameVerse 🎮
============

O **GameVerse** é uma plataforma de gestão de coleções de videojogos desenvolvida como parte da disciplina de Orientação a Objetos. A aplicação utiliza a arquitetura **BMVC (Bottle Model View Controller)** para oferecer uma experiência FullStack completa, permitindo a gestão de utilizadores e de uma biblioteca de jogos.


🚀 Funcionalidades
------------------

### 👤 Gestão de Utilizadores

*   **Registo e Login**: Sistema de autenticação seguro utilizando hashing de passwords com bcrypt.
    
*   **Perfis Personalizados**: Suporte para upload de fotos de perfil e nomes de utilizador únicos.
    
*   **Painel de Controle**: Os utilizadores podem editar as suas informações (e-mail, senha, nome e foto) ou apagar a sua conta permanentemente.
    

### 🎮 Gestão de Jogos (CRUD)

*   **Exploração Pública**: Visualização da coleção de jogos disponível para todos os visitantes.
    
*   **Painel Administrativo**: Utilizadores autenticados podem adicionar novos jogos, editar detalhes de títulos existentes ou removê-los da base de dados.
    
*   **Upload de Capas**: Sistema de armazenamento de imagens para as capas dos jogos.
    

🛠️ Tecnologias Utilizadas
--------------------------

*   **Linguagem**: Python 3.12.
    
*   **Framework Web**: Bottle.
    
*   **Segurança**: bcrypt para proteção de credenciais.
    
*   **Frontend**: HTML5, CSS3 e JavaScript Vanilla.
    
*   **Persistência**: Ficheiros JSON para armazenamento de dados de jogos e utilizadores.
    
*   **Infraestrutura**: Docker e Docker Compose para isolamento de ambiente.
    

📂 Estrutura do Projeto
-----------------------

*   app/controllers/: Contém a lógica de negócio e o controlador principal (application.py).
    
*   app/models/: Definições das classes de dados User e Game.
    
*   app/views/html/: Templates da interface (HTML e TPL).
    
*   app/static/: Recursos estáticos como CSS, JavaScript e imagens.
    
*   data/: Diretório de persistência dos ficheiros JSON.
    
*   route.py: Arquivo principal que define as rotas da aplicação.
    

⚙️ Como Executar
----------------

### Utilizando BASH (Local)

1.  Certifique-se de que o Python está instalado no seu sistema.
    
2.  Bashpython route.py
    

### Utilizando Docker

1.  Bashdocker build -t bmvci .
    
2.  Bashdocker run -d -p 8080:8080 -v $(pwd):/app bmvci
