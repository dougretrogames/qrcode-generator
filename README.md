# 📱 Gerador de QR Code Personalizado

<p align="center">
  <img src="https://img.shields.io/badge/Status-Conclu%C3%ADdo-success?style=for-the-badge" alt="Status Concluído">
  <img src="https://img.shields.io/badge/Licen%C3%A7a-MIT-blue?style=for-the-badge" alt="Licença MIT">
  <img src="https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/Privacidade-100%25%20Local-6D5DFC?style=for-the-badge" alt="100% Client-Side">
</p>

---

Um **Gerador de QR Code** moderno, responsivo, gratuito e **100% executado localmente no navegador (client-side)**. Crie códigos QR altamente personalizáveis com diferentes formatos de pixels, molduras com textos de chamada (CTA), logos de redes sociais, controle de cores HEX e exportação em PNG de alta definição.

🔗 **Acesse a aplicação online:** [https://dougretrogames.github.io/qrcode-generator/](https://dougretrogames.github.io/qrcode-generator/)

---

## ✨ Funcionalidades

- ⚡ **Pré-visualização em Tempo Real:** Renderização instantânea no elemento HTML5 `<canvas>` com *debounce* inteligente.
- 🎨 **Estilização de Módulos (Pixels):**
  - Quadrado (*Square*)
  - Arredondado (*Rounded*)
  - Pontos (*Dots*)
  - Arredondado Suave (*Soft Rounded*)
  - Círculos (*Circle*)
- 🖼️ **Molduras e Banners Promocionais (Frames):**
  - Posições: *Superior*, *Inferior*, *Lateral Esquerda*, *Lateral Direita* e *Completa*.
  - Texto customizável (Ex: "Acesse aqui", "Siga nosso perfil", "Cardápio").
  - Ajuste dinâmico de tamanho de fonte (`fitText`) para evitar quebras.
  - Controle de espessura da moldura (slider em pixels).
  - Cores personalizadas para o fundo e o texto da moldura.
  - Opção de cantos arredondados.
- 🌐 **Ícones de Redes Sociais Embutidos:**
  - Adicione logos oficiais sobre o centro do QR Code: WhatsApp, Instagram, YouTube, Facebook, LinkedIn, X, Telegram, TikTok, Discord e Threads.
  - Contorno de proteção em silhueta (*outline*) com a mesma espessura da margem do QR Code, acompanhando o formato exato de cada ícone.
  - Elevação automática da correção de erro para **H (Alta - 30%)** ao ativar ícone, garantindo 100% de legibilidade do QR Code.
- 🎯 **Controle de Correção de Erro (ECC):**
  - **L** (Baixa ~7%)
  - **M** (Média ~15%)
  - **Q** (Boa ~25%)
  - **H** (Alta ~30%)
- 🎨 **Paleta de Cores e Seletor HEX:**
  - 10 cores predefinidas em swatches rápidos.
  - Seletor de cores nativo (Color Picker) + entrada manual de código HEX para frente (foreground) e fundo (background).
- 📐 **Múltiplas Resoluções de Saída:**
  - De 128 × 128 px até 1024 × 1024 px (128px, 256px, 384px, 512px, 640px, 768px, 896px, 1024px) para uso digital ou impressão gráfica em alta qualidade.
- 💾 **Exportação e Compartilhamento:**
  - **Baixar PNG:** Download direto da imagem gerada.
  - **Compartilhar:** Integração com a **Web Share API** nativa para envio direto via WhatsApp, Telegram, e-mail, etc. (em dispositivos suportados).
- 🌓 **Design Moderno e Responsivo:**
  - Interface limpa com suporte automático a **Modo Claro (Light Mode)** e **Modo Escuro (Dark Mode)** via `prefers-color-scheme`.
  - Layout adaptável para telas móveis e desktop em tela dividida (*side-by-side*).

---

## 🔒 Privacidade e Segurança (Privacy by Design)

Diferente de geradores tradicionais na internet que enviam seus dados para servidores externos:

1. **Processamento 100% Local:** Todo o cálculo e desenho do QR Code ocorrem diretamente no seu navegador.
2. **Zero Coleta de Dados:** Nenhum texto, link, senha de Wi-Fi ou dado sensível é gravado ou transmitido para qualquer servidor ou banco de dados.
3. **Zero Rastreamento:** Sem cookies de rastreamento, sem anúncios e sem coleta de métricas invasivas.

Consulte a nossa [Política de Privacidade](privacy.html) e os [Termos de Uso](terms.html) para mais informações.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5:** Estruturação semântica e renderização gráfica via `Canvas API`.
- **CSS3:** Variáveis CSS (*Custom Properties*), Grid Layout, Flexbox, gradientes modernos e suporte a temas escuros.
- **JavaScript (Vanilla ES6+):** Manipulação de DOM, renderização assíncrona, conversão de SVG para Canvas e integração com a Web Share API.
- **[qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator):** Algoritmo de geração e codificação matricial dos dados QR.
- **[Simple Icons](https://simpleicons.org/):** Ícones vetoriais de marcas e redes sociais.

---

## 📂 Estrutura do Projeto

```text
qrcode-generator/
├── index.html       # Aplicação principal (Gerador interativo)
├── terms.html       # Página de Termos de Uso
├── privacy.html     # Página de Política de Privacidade
├── LICENSE          # Licença de uso de código aberto (MIT)
├── README.md        # Documentação completa do projeto
└── .gitignore       # Arquivos ignorados pelo controle de versão
```

---

## 🚀 Como Executar Localmente

Como o projeto é construído em Vanilla HTML/CSS/JavaScript puro, não é necessário instalar `Node.js`, `npm` ou configurar servidores complexos.

### Opção 1: Clonar e Abrir no Navegador
```bash
# 1. Clone o repositório
git clone https://github.com/dougretrogames/qrcode-generator.git

# 2. Acesse a pasta do projeto
cd qrcode-generator

# 3. Abra o arquivo index.html no seu navegador favorito (Chrome, Edge, Firefox, Safari)
```

### Opção 2: Usar uma Extensão de Live Server
Se estiver usando o **VS Code** ou outro editor:
1. Instale a extensão **Live Server** (ou execute `npx serve .` / `python -m http.server`).
2. Clique com o botão direito em `index.html` e selecione **Open with Live Server**.

---

## 🌐 Como Publicar no GitHub Pages

O projeto já está 100% pronto para publicação no **GitHub Pages**:

1. Acesse o seu repositório no GitHub: `https://github.com/dougretrogames/qrcode-generator`
2. Clique na aba **Settings** (Configurações).
3. No menu lateral esquerdo, clique em **Pages**.
4. Em **Build and deployment** > **Source**, selecione **Deploy from a branch**.
5. Em **Branch**, selecione a branch `main` e a pasta `/(root)`.
6. Clique em **Save**.
7. Em poucos segundos seu site estará no ar no endereço:  
   👉 `https://dougretrogames.github.io/qrcode-generator/`

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

<p align="center">
  Desenvolvido por <strong>Douglas (<a href="https://github.com/dougretrogames" target="_blank">@dougretrogames</a>)</strong>
</p>
