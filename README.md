**# 🍕 UaiEats | Plataforma Full-Stack de Delivery de Comida**

Projeto de portfólio completo que simula uma plataforma de entrega de comida com arquitetura desacoplada. O sistema demonstra alta proficiência em gerenciamento de estado complexo, segurança de API (JWT) e proteção de rotas front-end/back-end.

**# 🌟 Visão Geral do Projeto**

O UaiEats é um sistema ponta a ponta que permite aos usuários visualizar cardápios, montar um carrinho de compras, finalizar pedidos e gerenciar suas contas. O projeto é divido em dois serviços independentes: 

-Frontend (Cliente e Admin): Aplicação React/Vite.

-Backend (API): API RESTful construída com Django e Django REST Framework.



**# 🚀 Tecnologias e Arquitetura**

**Frontend**

-Tecnologia: React (Vite)

-Destaques: Componentização, Uso de Hooks (useState, useEffect, useContext), Design responsivo com CSS Puro.

**Backend e APIs**

-Tecnologia: Django / Django REST Framework (DRF)

-Destaques: Modelos de dados relacionais, ViewSets otimizados para API.

**Segurança e Persistência**

-Autenticação: JWT (Simple JWT) com Login, Cadastro, Refresh Token e Verificação de Conta por E-mail.

-Persistência/Segurança (Crucial): Uso de Axios Interceptors para lógica de renovação automática de token e garantir que o estado de isAdmin persista após o F5.



**# ✨ Destaques Funcionais**

-Persistência de Login (F5 Resolvida): Implementação de lógica no AuthContext para garantir que o estado de autenticação (papel do usuário e tokens) persista após o recarregamento da página.

-Gerenciamento de Carrinho: Lógica otimizada para adição, remoção e atualização de quantidade de itens no carrinho.

-APIs e Rotas Protegidas: Uso de AdminRoute no frontend e IsAuthenticated no backend para proteger o Painel Administrativo e o Perfil do Cliente.

-Gerenciamento de Usuários (Admin): Funcionalidade de listar, desativar/ativar e excluir usuários via endpoint RESTful (/api/users/).



**# ⚙️ Guia de Início Rápido**

**Siga estes passos para executar a aplicação completa localmente.**

**-Pré-requisitos**

-Você precisará de Python (com pip) e Node.js (com npm) instalados.


**1-Configurar Backend (API):**

cd uaieats_project/backend

pip install -r requirements.txt

**Crie o arquivo .env com SECRET_KEY, EMAIL_HOST_USER, etc.**

python manage.py makemigrations && python manage.py migrate


**2-Iniciar Servidor Django:**

python manage.py runserver


**3-Configurar Frontend (Cliente):**

cd ../frontend

npm install


**4-Iniciar Aplicação React:**

npm run dev


O **frontend** estará disponível em **http://localhost:5173.**



**🔗 Links Úteis**

 * **Documentação Detalhada (GitHub Pages):** https://lycanrf.github.io/UaiEats/
* **Acesso à API (Local):** `http://127.0.0.1:8000/api/`

