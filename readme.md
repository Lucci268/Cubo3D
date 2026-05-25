# 🧊 Cubo Mágico 3D - Simulador Interativo
# =Alunos= 
* **Luciano Henrique Pereira Cordeiro - 00000853712**
* **Paulo Barbosa Apolinário Neto - 00000853095**
* **Rafael Cavalcanti Montenegro - 00000863823**


Um simulador de Cubo Mágico (Rubik's Cube) tridimensional altamente interativo, renderizado direto no navegador. Este projeto foi desenvolvido como uma aplicação prática de **Computação Gráfica**, focando na aplicação de renderização 3D, transformações geométricas (matrizes de rotação e pivôs locais/globais), iluminação de estúdio realista e mapeamento de câmera orbital.

---

## 💻 Sobre o Projeto

O objetivo deste projeto é simular com precisão a mecânica e a estética de um Cubo Mágico profissional. Em vez de texturas simples, a malha 3D foi construída peça por peça: cada "cubinho" possui um núcleo de plástico escuro sólido, com adesivos coloridos individuais finamente posicionados sobre suas faces, reagindo dinamicamente à iluminação do ambiente. 

A interface de usuário (UI) foi desenhada com um estilo *Glassmorphism* (efeito de vidro translúcido), flutuando sobre o canvas WebGL para permitir o controle total sem poluir a visualização da cena.

## ✨ Funcionalidades

* **Manipulação 3D Completa:** Arraste com o mouse para orbitar a câmera 360º ao redor do cubo e use o *scroll* para aplicar zoom.
* **Controles Independentes de Faces:** Selecione qualquer face (U, D, L, R, F, B) via botões na tela ou pelo teclado.
* **Animação Baseada em Matrizes:** Rotações suaves em sentido horário ou anti-horário que garantem que as peças mantenham o alinhamento perfeito no espaço sem distorções (evitando *Gimbal Lock*).
* **Sistema de Embaralhamento (Scramble):** Algoritmo que realiza 20 movimentos aleatórios rápidos para misturar o cubo.
* **Iluminação de Estúdio Profissional:** Combinação de luz ambiente, luz principal com projeção de sombras (*Key Light*), preenchimento (*Fill Light*) e luz de contorno (*Rim Light*).
* **Contador de Movimentos:** Rastreamento de ações em tempo real integrado à interface.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5 & CSS3:** Estruturação da página e estilização da interface (UI) sobreposta.
* **JavaScript (ES6):** Lógica de estado do cubo, controle de eventos e cálculos matemáticos.
* **Three.js (WebGL):** Biblioteca gráfica principal para abstração da renderização 3D, gerenciamento de cena, geometrias, materiais (Phong) e luzes.

---

## 🤖 Inteligência Artificial e Modelagem

Toda a base do código, incluindo a estruturação matemática dos eixos e a modelagem geométrica (criação programática dos núcleos pretos e dos adesivos coloridos), foi gerada e otimizada utilizando a inteligência artificial **Manus**. 

A Manus auxiliou na arquitetura do código para separar eficientemente a manipulação do DOM da engine 3D, garantindo cálculos matemáticos robustos na hora de agrupar as peças dinamicamente em "pivôs" invisíveis para realizar as rotações das faces isoladas.

### 📝 Prompt Utilizado

Para alcançar a lógica central e o visual apresentados neste repositório, a orientação inicial fornecida à IA seguiu a seguinte diretriz de engenharia de prompt:

> *"Escreva o código de um simulador de Cubo Mágico 3D Premium interativo usando a biblioteca Three.js em um único arquivo HTML. A estética deve ser realista: os cubos menores precisam ser pretos, com adesivos coloridos individuais (com espessura) colados em suas faces externas. A cena precisa de iluminação de estúdio sofisticada (sombras, luz de contorno). A lógica de rotação deve agrupar as peças num pivô para girar faces específicas de forma animada (sem quebrar as coordenadas ao longo do tempo). Crie também uma interface translúcida em CSS por cima do canvas com botões para escolher a face (U, D, L, R, F, B), rotacionar (horário/anti-horário), embaralhar automaticamente, resetar e mostrar o número de movimentos. Implemente controles de câmera orbital pelo mouse."*

---
