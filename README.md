🤝 Social Media API (Django REST Framework)

API REST de uma rede social: os usuários criam posts públicos ou privados, enviam e aceitam pedidos de amizade, comentam, curtem e seguem outros usuários.

Tecnologias
Python, Django, Django REST Framework
Configuração por variáveis de ambiente (.env)
Coleção de requisições para Insomnia incluída no repositório
Funcionalidades
Cadastro e gerenciamento de usuários
Pedidos de amizade: enviar e aceitar
Posts públicos e privados (posts privados visíveis só para amigos)
Comentários e curtidas
Seguidores
Estrutura do projeto
App	Responsabilidade
users	Usuários
friendship_request	Pedidos de amizade
friends	Lista de amigos
followers	Seguidores
posts	Posts públicos e privados
comments	Comentários
likes	Curtidas
_project	Configurações e rotas gerais
Como rodar localmente
bash
git clone https://github.com/nakszor/social-media-django.git
cd social-media-django

python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

pip install -r requirements.txt
cp .env.example .env            # preencha as variáveis
python manage.py migrate
python manage.py runserver
Endpoints

Importe o arquivo Insomnia_2023-05-08.json no Insomnia para testar todas as rotas.

Autoria

Projeto desenvolvido em equipe na Kenzie Academy Brasil.
