# ⚙️ Processo de Desenvolvimento – Lógica de Programação

Documentação do fluxo de trabalho, metodologia e etapas de criação da aplicação interativa desenvolvida para o **Mundo SENAI 2026**.

---

## 🎯 Objetivo do Processo

Criar uma ferramenta interativa e didática que servisse como guia visual durante as apresentações do curso de **Técnico em Informática para Internet**, explicando os fundamentos da Lógica de Programação para o público geral.

---

## 📅 Etapas de Desenvolvimento
### 1. Planejamento & Definição de Escopo
- Definição dos 4 tópicos principais: *Algoritmos*, *Variáveis*, *Estruturas de Controle* e *Universalidade da Lógica*.
- Escolha da abordagem didática baseada em elementos visuais e interativos em vez de slides estáticos.

### 2. Design e Experiência do Usuário (UX/UI)
- Criação do layout responsivo com visual adaptável para monitores, notebooks e dispositivos móveis.
- Implementação da paleta de cores institucional SESI/SENAI (Azul `#00468C`, Laranja `#F47B20`).
- Integração de elementos lúdicos animados via CSS e SVG (engrenagens e circuitos dinâmicos).

### 3. Implementação Técnica
- **HTML5:** Estruturação semântica em formato de *Slide Deck* acessível.
- **CSS3:** Uso de variáveis globais, CSS Grid/Flexbox e animações controladas por keyframes (`@keyframes`).
- **JavaScript (Vanilla):**
  - Sistema de troca de slides por teclado (`←` / `→`) e toque.
  - Manipulação do DOM para execução em tempo real dos simuladores (`SE/SENÃO`, `ENQUANTO`, Quiz).

### 4. Testes e Ajustes
- Testes de acessibilidade e redução de movimento (`prefers-reduced-motion`).
- Otimização do desempenho de renderização dos SVGs e animações.

### 5. Publicação e Hospedagem
- Versionamento do código-fonte através do **GitHub**.
- Configuração do serviço de hospedagem e deployment contínuo na plataforma **Render**.

---

## 👥 Organização da Equipe e Papéis

| Integrante | Responsabilidades no Projeto |
| :--- | :--- |
| **Gabriel** | Pesquisa de conteúdo didático e estruturação dos exemplos lógicos. |
| **Gustavo** | Desenvolvimento das estruturas HTML e estilização CSS dos slides. |
| **Henzo** | Implementação dos scripts JavaScript e lógica das interações. |
| **Marcos** | Gerenciamento do repositório Git/GitHub e configuração do Render. |
| **Pedro** | Elaboração da apresentação verbal e roteiro de demonstração. |
| **Rafael** | Criação dos componentes visuais, animações SVG e design de interface. |

---

## 🛠️ Desafios Encontrados e Soluções

- **Desafio:** Manter o fluxograma legível e com rolagem suave à medida que os nós eram adicionados.  
  **Solução:** Implementação da função `scrollTo` com comportamento suave (`behavior: 'smooth'`) acionada via `requestAnimationFrame`.

- **Desafio:** Garantir performance consistente em diferentes navegadores sem usar bibliotecas pesadas.  
  **Solução:** Desenvolvimento em JavaScript puro (Vanilla ES6+), eliminando dependências externas.
