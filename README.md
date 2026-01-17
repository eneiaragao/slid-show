# 🎞️ Slide Show Dinâmico - Infinite Loop

Um carrossel de imagens responsivo construído com JavaScript puro, focado em performance e transições suaves. O projeto utiliza manipulação física do DOM para criar um efeito de navegação infinita.



## 🚀 Tecnologias Utilizadas

* **HTML5:** Estrutura base com containers flexíveis.
* **CSS3 (Avançado):**
    * **Flexbox:** Para alinhamento e organização dos itens.
    * **Media Queries:** Design totalmente responsivo para celulares e desktops.
    * **Object-fit (cover):** Garante que as imagens preencham o espaço sem distorcer.
* **JavaScript (Vanilla):**
    * **Template Literals:** Carregamento dinâmico das imagens via script.
    * **DOM Manipulation:** Uso de `appendChild` e `insertBefore` para criar o efeito de loop infinito.

## 📋 Funcionalidades

- **Carregamento Dinâmico:** As imagens são injetadas no HTML a partir de um array de objetos no JavaScript.
- **Loop Infinito:** O slider nunca acaba; ao chegar na última imagem, a sequência recomeça movendo os elementos.
- **Responsividade:** Ajuste automático de dimensões para diferentes tamanhos de tela (Mobile e Desktop).
- **Interface Minimalista:** Botões de navegação intuitivos com efeitos de transição no hover.

## ⚙️ Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/projeto-slideshow.git](https://github.com/seu-usuario/projeto-slideshow.git)
    ```
2.  **Organização das Imagens:**
    Certifique-se de que as imagens estejam dentro de uma pasta chamada `img` na raiz do projeto, com os nomes:
    - `chrono.jpg`, `inuyasha.jpg`, `tenchi.jpg`, `tenjhotenge.jpg`, `yuyuhakusho.jpg`, `ippo.png`.
3.  **Execução:**
    Basta abrir o arquivo `index.html` em qualquer navegador.

---

## 🧠 Lógica de Funcionamento

Diferente de sliders que apenas mudam a posição do scroll, este projeto altera a estrutura do HTML em tempo real:



* **Ação "Next":** Pega o primeiro elemento e o move para o final do container.
* **Ação "Previous":** Pega o último elemento e o insere antes do primeiro.

---

## 📁 Estrutura de Arquivos

```text
├── index.html    # Estrutura principal
├── style.css     # Estilos e Media Queries (Responsividade)
├── script.js     # Lógica de movimentação dos itens e dados das imagens
└── img/          # Pasta com as imagens dos animes
