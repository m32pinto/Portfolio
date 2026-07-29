# 🔱🎩 Portfólio Profissional - [m32pinto](portfoliodomarcos.com.br)

Bem-vindo ao repositório oficial do meu portfólio profissional! Este projeto foi desenvolvido com foco em alta performance, responsividade e na entrega de soluções inteligentes utilizando o ecossistema moderno de desenvolvimento.

---

## 🏢 Sobre a Empresa
Este projeto é mantido por **m32pinto** (empresa com CNPJ ativo), focada no desenvolvimento de automações, chatbots inteligentes, formulários personalizados de alta performance e soluções web.

---

## 📜 Histórico do Portfólio
* **Versão Anterior:** O portfólio original foi construído utilizando tecnologias tradicionais de front-end (**HTML, CSS e JavaScript puro**).
* **Migração Atual:** Com a evolução dos objetivos profissionais e o foco intensivo em **Flutter Web** e desenvolvimento de formulários dinâmicos, o projeto foi totalmente reescrito em **Flutter**. Essa mudança permitiu unificar a linguagem de programação (Dart) em toda a lógica, aproveitando a robustez e a integração nativa com o ecossistema do Google.

---

## 🛠️ Ferramentas Utilizadas
O projeto faz uso de um conjunto tecnológico moderno e eficiente:
* **Flutter & Dart:** Framework principal para o desenvolvimento da interface (UI/UX) responsiva voltada para a Web.
* **Firebase Hosting:** Plataforma de hospedagem serverless rápida e segura fornecida pelo Google.
* **Web3Forms API:** Serviço de envio de e-mails via API REST integrado ao formulário de contato do front-end.
* **Git & GitHub / GitHub Pages:** Controle de versão do código-fonte e histórico de evoluções.
* **Linux:** Sistema operacional utilizado como ambiente de desenvolvimento principal.
* **Gemini (Google):** Assistente de inteligência artificial colaborativa utilizada para suporte de código, arquitetura e refatoração.

---

## 💻 Comandos Essenciais de Gerenciamento
Aqui estão os comandos fundamentais utilizados no terminal para gerenciar, compilar e enviar atualizações do projeto:

1. **Limpar o cache do projeto (essencial antes de builds limpos):**
   ```bash
   flutter clean
2. **Baixar e atualizar as dependências (lendo o pubspec.yaml):**
   ```bash
   flutter pub get
3. **Compilar o projeto otimizado para produção Web (com injeção segura de chaves):**
   ```bash
   flutter build web --release --dart-define=WEB3FORMS_ACCESS_KEY=sua_chave_aqui
4. **Fazer o deploy manual para o Firebase Hosting:**
   ```bash
   firebase deploy --only hosting

🔄 Como Atualizar o Projeto
Caso você queira clonar este repositório e realizar atualizações no código-fonte, siga este fluxo seguro:

1. Abra o projeto no seu editor (ex: VS Code).
2. Faça as alterações desejadas nos arquivos dentro da pasta lib/.
3. No terminal, execute o processo de limpeza e compilação:
   ```bash
   flutter clean
   flutter pub get
   flutter build web --release --dart-define=WEB3FORMS_ACCESS_KEY=sua_chave_aqui
4. Envie a nova versão compilada para a nuvem:
   ```bash
   firebase deploy --only hosting

✉️ Webform para Envio de E-mails
O formulário de contato integrado ao portfólio utiliza a API do Web3Forms.

Arquitetura: O Flutter realiza uma requisição HTTP POST assíncrona enviando um payload em formato JSON com os dados do remetente (nome, e-mail, assunto e mensagem).

Segurança: Por se tratar de uma aplicação Web (Frontend), as chaves sensíveis não são expostas em arquivos de texto estáticos no servidor. Elas são injetadas de forma segura no momento da compilação utilizando a flag --dart-define do Flutter, mantendo o código blindado e profissional.

📚 Informações Relevantes para Estudantes
Se você é um estudante explorando este repositório para aprender mais sobre Flutter e o ecossistema Google, observe os seguintes pontos de destaque na arquitetura:

1. **Single Page Application (SPA):** O Flutter Web compila o código Dart em otimizações de HTML/JavaScript/Wasm, rodando de forma fluida no navegador.
2. **Clean Architecture & Separação de Responsabilidades:** A lógica de envio de e-mails (EmailService) está totalmente isolada das telas (ContactScreen), permitindo testes unitários e manutenção simplificada.
3. **Ecossistema Google:** A escolha por combinar Flutter com Firebase Hosting demonstra a sinergia perfeita entre ferramentas Google para deploy ágil, SSL automático e alta disponibilidade.

🤖 Assistente Pessoal e Desenvolvimento
Este portfólio foi construído através de uma parceria de programação colaborativa com o Gemini, atuando como um assistente de engenharia de software para estruturação de código limpo, boas práticas e resolução de desafios técnicos no Linux.

Desenvolvido com dedicação por Marcos Antonio (m32pinto).
