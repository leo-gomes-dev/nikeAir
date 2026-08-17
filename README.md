# Nike Air Pro - Landing Page Imersiva

Uma landing page conceitual, responsiva e de alta performance desenvolvida para demonstrar habilidades avançadas em engenharia de interface frontend, manipulação semântica do DOM e microinterações fluidas orientadas a hardware.

⚡ **Link do Projeto:** [Acesse o Deploy no GitHub Pages](https://github.io)

---

## 🛠️ Decisões de Arquitetura e Engenharia de Interface

Este projeto foi construído recusando o uso de frameworks pesados ou bibliotecas externas redundantes de JavaScript, focando na utilização máxima de recursos nativos modernos das APIs da Web.

### 1. Acessibilidade e Semântica Nativa (`<dialog>`)
Em vez de construir estruturas complexas de modais utilizando `divs` aninhadas com manipulação manual de estados de `z-index`, o projeto adota a tag nativa **`<dialog>` do HTML5**.
* **Benefícios Técnicos:** Isolamento semântico automático para leitores de tela, captura e gerenciamento automático de foco do teclado (*focus trapping*) e suporte nativo ao fechamento através da tecla `ESC` sem acréscimo de lógica no JavaScript.

### 2. Microinterações e Performance Visual
Toda a dinâmica de animações e transformações do produto (como a flutuação horizontal e a rotação tridimensional em eixos coordenados no hover) foi implementada utilizando CSS puro através do **Tailwind CSS**.
* **Benefícios Técnicos:** As transições utilizam propriedades que ativam a aceleração de hardware do dispositivo (`transform: rotate` e `scale`), mitigando problemas de gargalo de renderização e garantindo taxas estáveis de 60fps tanto em desktops quanto em navegadores móveis mais antigos.

### 3. Layout Fluido e Prevenção de CLS
O carregamento de mídia foi planejado para evitar quebras visuais e o efeito de *Cumulative Layout Shift* (CLS). A imagem principal do calçado utiliza tratamento responsivo estrito (`max-w-md object-contain`), isolada em um container flexível de cor pura em gradiente, acelerando o tempo de primeira pintura de conteúdo (FCP) por eliminar imagens pesadas inseridas via propriedades de background.

---

## 🚀 Tecnologias Utilizadas

* **HTML5:** Estruturação semântica avançada e APIs de acessibilidade.
* **Tailwind CSS (v3/v4):** Utilitários de estilização atômica e design system unificado.
* **JavaScript Moderno (ES6):** Controle de eventos assíncronos e manipulação leve do DOM.
* **Google Fonts:** Tipografia otimizada com pré-carregamento assíncrono.

---

## 🧠 Como Rodar o Projeto Localmente

1. Clone o repositório em sua máquina:
   ```bash
   git clone https://github.com/leo-gomes-dev/nikeAir.git
   ```
2. Acesse a pasta do projeto:
   ```bash
   cd nome-do-repositorio
   ```
3. Execute o arquivo `index.html` diretamente no seu navegador ou utilize a extensão **Live Server** do VS Code para atualizações automáticas em tempo real.

---

Desenvolvido com foco em excelência técnica por **Leo Gomes** 🚀
