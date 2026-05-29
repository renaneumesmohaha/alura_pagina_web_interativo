# alura_pagina_web_interativo# 🌱 Terra do Amanhã | Interface Interativa & Acessibilidade

O projeto **Terra do Amanhã** é uma Landing Page conceitual focada no futuro do agronegócio sustentável e da agricultura de precisão. O grande diferencial técnico deste projeto está na fusão de um **design editorial premium** com um **Hub de Acessibilidade 100% interativo** desenvolvido em JavaScript Vanilla.

---

## 🎯 Objetivo da Aplicação

Demonstrar de forma prática como a interatividade web pode (e deve) ser usada para promover a inclusão digital. Através de manipuladores de eventos e inovações com APIs nativas de navegadores, o projeto garante que pessoas com deficiências visuais ou dificuldades de leitura consumam o conteúdo de forma confortável.

---

## 🕹️ Recursos Interativos Desenvolvidos

O painel flutuante (Hub de Acessibilidade) conta com três pontos principais de interação dinâmica via JavaScript:

### 1. Controle Deslizante de Fonte (Slider Input)
* **Como funciona:** Um seletor de alcance (`input type="range"`) captura as alterações de valor feitas pelo usuário em tempo real.
* **Lógica Técnica:** O JavaScript intercepta o evento `input`, calcula o novo valor em pixels (entre 12px e 24px) e altera a propriedade `fontSize` diretamente no elemento `<body>`. Como o layout utiliza unidades relativas, todo o texto do site se ajusta de forma harmônica e proporcional.

### 2. Alternador de Modo Escuro / Alto Contraste (Toggle Switch)
* **Como funciona:** Um botão customizado estilizado para simular um interruptor elétrico de ligar/desligar.
* **Lógica Técnica:** Ao clicar, o JavaScript executa um `classList.toggle('dark')` na raiz do documento HTML. O framework Tailwind CSS identifica a classe ativa e substitui instantaneamente todas as variáveis de cores do site, oferecendo uma experiência de alto contraste confortável para ambientes escuros.

### 3. Mecanismo de Texto-para-Voz (Text-to-Speech)
* **Como funciona:** Um botão dinâmico que inicia ou encerra a narração por voz inteligente do conteúdo exposto no site.
* **Lógica Técnica:** Consome a **Web Speech API** nativa do ecossistema moderno de navegadores. O script mapeia as seções através da classe `.section-narrative`, gera uma fila organizada de leitura (`SpeechSynthesisUtterance`) e narra de forma contextualizada os títulos e textos, alterando o design do botão para o estado de "Parar" em tempo real.

---

## 🛠️ Tecnologias Utilizadas

* **Estrutura:** HTML5 Semântico e atributos ARIA para acessibilidade estrutural.
* **Estilização & Responsividade:** Tailwind CSS (carregado via CDN para prototipagem ágil).
* **Interatividade Dinâmica:** JavaScript Vanilla (ES6+) focado em manipulação do DOM e escuta de eventos (`addEventListener`).
* **Tipografia:** Google Fonts (`Playfair Display` para títulos e `Inter` para leitura corrida).

---

## 🚀 Como Executar o Projeto

1. Faça o download ou clone a pasta contendo os arquivos.
2. Certifique-se de manter o `index.html` e este `README.md` organizados na raiz do seu diretório.
3. Abra o arquivo `index.html` em qualquer navegador web (Google Chrome, Safari, Microsoft Edge ou Mozilla Firefox).
4. Interaja com os botões do painel no canto inferior direito para testar os recursos dinâmicos.