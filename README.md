# 12 DIAS: ROTA DE FUGA 🧟‍♂️🎲
Um jogo de sobrevivência zumbi e alocação de dados (Roll & Write) nas versões **Print & Play** (Imprima e Jogue) e **Digital** (Web App).

## 🎲 Sobre o Jogo
Você é um sobrevivente ilhado em uma cidade dominada por mortos-vivos. O resgate nunca virá. Sua única chance é consertar um carro velho abandonado na oficina e **FUGIR**. Mas você tem pouco tempo: a horda chegará no dia 12. 
Gerencie suprimentos, enfrente perigos, colete recursos rolando dados e defenda sua barricada contra a horda!

## 📦 Estrutura do Projeto
A organização do projeto foi ajustada para melhor legibilidade:

- `index.html` - **O Jogo Digital!** (antigo `folha_de_jogo_v2.html`). Abra no navegador para jogar.
- `12_Dias_Rota_de_Fuga_PnP.pdf` - **A Versão Física!** Arquivo em PDF formatado para impressão perfeita em folha A4.
- `docs/` - Contém o manual de regras em HTML e arquivos de texto como o post do Discord.
- `audio/` - Pasta para a trilha sonora em MP3 da versão digital.
- `img/` - Imagens, texturas e logos usados diretamente na interface do jogo.
- `pnp-source/` - Códigos HTML base e PDFs de testes usados para gerar a versão Print & Play final.
- `assets/` - Imagens soltas antigas, tilesets brutos e arquivos originais que serviram de base.
- `tools/` - Ferramentas de desenvolvimento (ex: `sprite_viewer.html`).

## 🕹️ Como Jogar

### Opção 1: Versão Digital (Web)
1. Baixe os arquivos do projeto.
2. Dê um clique duplo em `index.html` para abri-lo no seu navegador favorito.
3. Clique em **"Iniciar Jogo"**. O tutorial interativo irá te guiar pelos primeiros passos.
4. O sistema cuida da rolagem de dados e eventos, mas **você deve clicar manualmente nos medidores** no topo da tela para alterar Vida, Suprimentos, Munição, etc., simulando a folha de papel.

### Opção 2: Versão Print & Play
1. Imprima o arquivo `12_Dias_Rota_de_Fuga_PnP.pdf` em uma folha A4 (foi otimizado para não gastar muita tinta).
2. O manual de regras está dentro do arquivo `docs/manual_de_regras.html`.
3. Você precisará de **7 dados normais (D6)** (sendo 2 deles de cores diferentes para servir como dado de clima e dado de eventos).
4. Utilize lápis e borracha para marcar os quadradinhos da folha!

## 🛠️ Tecnologias Utilizadas
- HTML5, CSS3 Vanilla, JavaScript
- Geração procedural de imagens por IA
- Interface fluida baseada em *Glassmorphism* no jogo web.
