# Jogo Heroi-Vilão com Banco de Dados

# 🎮 Descrição
O Jogo Herói e Vilão é uma aplicação web que simula uma batalha entre um herói e um vilão. Os usuários podem interagir escolhendo ações para os personagens, como atacar, defender, usar poção e correr. A cada ação realizada, o estado dos personagens é atualizado e exibido na interface do usuário.
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">


# Índice 
* [Descrição do Jogo](#-descrição-do-jogo)
* [Características do Jogo](#-características-do-jogo)
* [Tecnologias Utilizadas](#-tecnologias-utilizadas)
* [Funcionalidades](#-funcionalidades)
* [Orientação de Utilização](#-orientação-de-utilização)
* [Interface](#-interface)
* [Como Jogar](#-como-jogar)
* [Licença](#licença)


   
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

# 👩‍💻 Características do Jogo 
- Batalha entre um herói e um vilão.
- Interface interativa que permite aos usuários escolherem ações para os personagens.
- Atualização em tempo real do estado dos personagens.
- Histórico de ações realizadas durante a partida.
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

# 💻 Tecnologias Utilizadas 
- Frontend: Vue.js
- Backend: Node.js com Express
- Banco de Dados: Microsoft SQL Server
- Hospedagem: Render (Backend) e Netlify (Frontend)

- Frontend:
    - Vue.js - Framework JavaScript para a construção de interfaces de usuário interativas.
    - HTML5 e CSS3 - Para a estrutura e estilização da interface do usuário.
    - Fetch API - Usado para fazer requisições HTTP para o backend e interagir com os recursos do servidor de forma assíncrona.
- Backend:
    - Node.js - Ambiente de execução JavaScript do lado do servidor.
    - Express.js - Framework web utilizado para criar e gerenciar rotas HTTP, além de fornecer middleware para habilitar funcionalidades como CORS e parse de JSON.
    - MSSQL -  Usado como driver para se conectar e interagir com o banco de dados SQL Server.
- Banco de Dados:
  - Microsoft SQL Server (Azure): Banco de dados relacional hospedado no Microsoft Azure para armazenar dados dos jogadores, personagens e histórico do jogo.
- Hospedagem:
    - Render (Backend): Utilizado para hospedar o servidor backend, fornecendo uma infraestrutura escalável e confiável para executar sua aplicação Node.js.
[Link Render ospedado ](https://prova-marcio.onrender.com/)
    - Netlify (Frontend): Utilizado para hospedar o frontend, fornecendo uma maneira simples e eficiente de distribuir sua aplicação estática HTML, CSS e JavaScript.
[Link Netlify ospedado ](https://heroivilaojogo.netlify.app/) 
 
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">


# 🖥️ Funcionalidades:
- Login e Cadastro: Os jogadores podem se cadastrar e fazer login para acessar o jogo.
- Batalha: Durante a batalha, os jogadores podem realizar diferentes ações, como atacar, defender, usar poções de cura e correr.
- Atualização de Vida: Após cada ação, a vida do herói e do vilão é atualizada no banco de dados.
- Histórico de Ações: Todas as ações realizadas durante a partida são registradas em um histórico e armazenadas no banco de dados.
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

# 🗒️ Orientação de Utilização

### 🚀 Pré-requisitos

- Node.js instalado na máquina local.
- Banco de dados Microsoft SQL Server configurado e acessível.
    
<h3> ⚙️  Instalação de Dependências </h3>
1. Clone o Repositório: Faça uma cópia do repositório para o seu ambiente local.

       git clone https://github.com/ellendias01/Prova-Marcio.git
2. Navegue até o Diretório do Projeto: Acesse o diretório do projeto recém-clonado.

       cd Prova-Marcio
3. Instale as Dependências do Frontend: Navegue até o diretório do frontend e instale as dependências.

       cd frontend
       npm install
4. Instale as Dependências do Backend: Navegue até o diretório do backend e instale as dependências.

       cd ../backend
       npm install

    
<h3> 📊 Configuração do Banco de Dados </h3>
Configure o Banco de Dados MSSQL: No arquivo config.js no diretório backend, configure as credenciais do banco de dados.

```javascript
const config = {
user: "seu_usuario",
password: 'sua_senha',
server: "seu_servidor",
database: "nome_do_banco_de_dados",
options: {
encrypt: true // Dependendo da configuração do seu servidor SQL Server
}
};
```
<h3> 🧑‍💻 Execução do Projeto </h3>
1. Inicie o Servidor Backend: Execute o servidor backend.
   
        node server.js
2. Inicie o Servidor Frontend: Execute o servidor frontend.

       npm run serve
  
3. Acesse o Jogo: Abra o navegador e acesse http://localhost:8080 para iniciar o jogo.

<h3> 🎮 Uso </h3>

- Na interface do jogo, escolha as ações disponíveis para o herói e o vilão.
- Observe a atualização em tempo real da vida dos personagens e o histórico de ações realizadas.
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

# :flower_playing_cards: Interface

### Tela inicial - tela de Login 
| Tela   | Imagem                                                                                                  |
|--------|---------------------------------------------------------------------------------------------------------|
| Login  | <img src="https://github.com/ellendias01/Tela-de-Login-e-Sing-In/assets/145167118/b46c7635-e782-46c6-b940-a7f9fb99154a" alt="login" width="700">  |
| Sing In| <img src="https://github.com/ellendias01/Tela-de-Login-e-Sing-In/assets/145167118/5cad4d7f-da3e-45e2-a3f8-d82d4a15852e" alt="singin" width="700"> |

### Tela do jogo 
![tela principal](https://github.com/ellendias01/Prova-Marcio/assets/145167118/eeb2c82d-065e-45df-aa2a-dce1def127f4)
| Personagem | Herói | Vilão |
|------------|-------|-------|
| Imagem     | ![Herói](https://github.com/ellendias01/Prova-Marcio/assets/145167118/c6c9f3b7-67fa-4b48-969f-a5edcd03e3a1) | ![Vilão](https://github.com/ellendias01/Prova-Marcio/assets/145167118/6ad208b4-b72b-4e9c-8309-fdc4dc527763) |

### Tela Dashboard 
| Tela                               | Imagem                                                                                                   |
|------------------------------------|----------------------------------------------------------------------------------------------------------|
| Tela sem informação                | ![Tela sem informação](https://github.com/ellendias01/Prova-Marcio/assets/145167118/063c2d26-9b54-45e1-88ee-ae2e787477bd) |
| Tela com informação                | ![Tela com informação](https://github.com/ellendias01/Prova-Marcio/assets/145167118/a4586a32-3900-4ba1-a2c0-136243902a5f) |

### Video do Site funcionando 


https://github.com/ellendias01/Prova-Marcio/assets/145167118/8b6e122c-b8de-4ac4-8cb9-478d28f17496



<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

# 🕹️Como Jogar

1. Abra o navegador e acesse o endereço [Jogo Heroi Vilão](https://heroivilaojogo.netlify.app/login) para iniciar o jogo.
2. Faça login com suas credenciais ou crie uma nova conta.
3. Interaja com o jogo clicando nos botões disponíveis para atacar, defender, usar poção ou correr.
4. Observe o status dos personagens e o histórico de ações para acompanhar o progresso do jogo.
5. Divirta-se!

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

# Licença
Este projeto é distribuído sob a Licença MIT. Consulte o arquivo [LICENSE](https://github.com/ellendias01/Prova-Marcio/blob/main/LICENSE) para obter mais detalhes.
