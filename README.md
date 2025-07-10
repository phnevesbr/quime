# Quime - Plataforma de Quizzes Sociais 🚀

![Quime Screenshot](URL_DA_SUA_IMAGEM_AQUI) <!-- TIRE UM PRINT BONITO OU FAÇA UM GIF! -->

**Live Demo:** [Clique aqui](https://infoscgg22.elementfx.com/) <!-- LINK PARA O PROJETO FUNCIONANDO -->

## 📝 Sobre o Projeto

Quime é uma aplicação web full-stack que permite aos usuários criar, compartilhar e jogar quizzes interativos. O projeto foi desenvolvido como uma plataforma social completa, focada em engajamento e gamificação, com sistemas de ranking, multiplayer em tempo real, loja de itens e conquistas.

## ✨ Features Principais

*   **Autenticação de Usuários:** Sistema seguro de registro e login com sessões PHP.
*   **Criação de Quizzes:** Fluxo intuitivo com 4 etapas para criar quizzes personalizados, escolhendo tema, modo de jogo e perguntas.
*   **Modos de Jogo Variados:** Normal, Tempo, Aposta e Detetive, cada um com uma lógica de pontuação única.
*   **Multiplayer em Tempo Real:** Lobbies para desafiar amigos em partidas ao vivo, com placar atualizado dinamicamente via long-polling.
*   **Sistema de Gamificação:**
    *   **Níveis e XP:** Usuários ganham XP e sobem de nível.
    *   **Moedas e Loja:** Moeda virtual para comprar itens cosméticos (molduras) e boosts.
    *   **Missões e Conquistas:** Sistema de missões diárias/semanais e um painel de conquistas para reter usuários.
*   **Perfis de Usuário:** Páginas de perfil personalizáveis com estatísticas, avatares, molduras e listas de quizzes.
*   **Rankings Globais:** Rankings separados para os melhores jogadores e os quizzes mais populares.
*   **Interface Responsiva:** Design moderno e totalmente adaptado para desktop e dispositivos móveis.

## 🛠️ Tecnologias Utilizadas

*   **Frontend:** HTML5, CSS3, JavaScript (ES6+ com Módulos)
*   **Backend:** PHP 7.4+ (API RESTful)
*   **Banco de Dados:** MySQL / MariaDB
*   **Ferramentas Adicionais:** `html2canvas` para geração de imagens de resultado.

## ⚙️ Instalação e Execução Local

1.  Clone o repositório: `git clone https://github.com/seu-usuario/quime.git`
2.  Importe o banco de dados usando o arquivo `database.sql`.
3.  Configure as credenciais do banco de dados no arquivo `api/db_connection.php`.
4.  Execute o projeto em um servidor local compatível com PHP e MySQL (XAMPP, WAMP, etc.).
5.  Acesse `http://localhost/quime` no seu navegador.

## 🛡️ Destaques Técnicos e de Segurança

*   **Prevenção de SQL Injection:** Todas as queries ao banco de dados utilizam **Prepared Statements**.
*   **Prevenção de XSS:** Validação e sanitização de dados de entrada do usuário (`htmlspecialchars`).
*   **Prevenção de Abuso:** Implementado um sistema de **Rate Limiting** para ações críticas como registro e criação de quizzes.
*   **API Estruturada:** O backend funciona como uma API, separando a lógica de negócio da apresentação.
*   **Código Modular:** O JavaScript é dividido em módulos (`state`, `api`, `ui`, etc.) para melhor organização e manutenibilidade.
