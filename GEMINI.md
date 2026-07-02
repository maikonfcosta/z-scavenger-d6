# Z-Scavenger: Destino D6 - Contexto e Memória do Projeto

Este arquivo serve como repositório de memória, regras de design e aprendizados contínuos para guiar agentes de IA e desenvolvedores que venham a trabalhar no projeto *Z-Scavenger: Destino D6*.

---

## 🧭 Visão Geral do Jogo
*   **Título:** Z-Scavenger: Destino D6
*   **Gênero:** Print & Play (PnP) Solo de Alocação de Dados (Dice Placement) e Sobrevivência Pós-Apocalíptica.
*   **Objetivo de Vitória:** Consertar o carro na Oficina (Trilha de Conserto) e em seguida passar no Teste de Fuga (Soma > 8).
*   **Condições de Derrota:**
    1.  Vida reduzida a 0.
    2.  Infecção aumentada a 6.
    3.  Marcador de Horda alcançar o espaço final (12).

---

## 📜 Regras Atualizadas

### 1. Barricada (Defesa Obrigatória)
O jogador pode alocar 0, 1 ou no máximo 2 dados na Barricada. 
A soma dos dados deve ser **maior ou igual** ao valor atual da Ameaça (definida pelo Clima).
**Penalidade:** Se a soma for *menor* que a Ameaça (ou se 0 dados forem alocados), o jogador perde **1 de Vida E 1 de Suprimento**.

### 2. Oficina & Combos
Pode-se alocar até 3 dados na Oficina. Existem 3 combos especiais que só podem ser usados **1 vez por partida**:
*   **PAR (ex: 2 e 2):** Gambiarra -> Ganha +1 Sucata.
*   **TRINCA (ex: 4, 4 e 4):** Peça Intacta -> Avança 1 espaço no Conserto de graça.
*   **SEQUÊNCIA DE 3 (ex: 2, 3 e 4):** Pólvora e Chumbo -> Recupera 1 de Munição.

### 3. Tabela de Encontros (Rolar 1D6 após explorar um local)
*   **1** - *Zumbis Bloqueiam a Saída:* Perde o recurso do local **OU** gasta 1 Munição para mantê-lo.
*   **2** - *Risco de Infecção:* Aumente 1 de Infecção.
*   **3** - *Caminho Seguro:* Nada extra.
*   **4** - *Achado Útil:* Ganhe +2 Sucatas extras.
*   **5** - *Mochila Abandonada:* Ganhe +1 Suprimento extra.
*   **6** - *Estoque Militar:* Ganhe +1 Munição extra.

### 4. Clima e Ameaça (Rolar 1D6 no início do dia)
*   **1** - Céu Limpo (Ameaça 4)
*   **2** - Sol Forte (Ameaça 5)
*   **3** - Nublado (Ameaça 6)
*   **4** - Chuva Fina (Ameaça 7) -> *Abrigo: 3 e 4 não curam Vida nesta rodada.*
*   **5** - Chuva Forte (Ameaça 8) -> *Oficina: Consertar o carro custa 1 Sucata extra.*
*   **6** - Névoa Densa (Ameaça 10) -> *Visibilidade Zero: Não pode gastar Munição nesta rodada.*

### 5. Fuga Final (O Clímax)
Após preencher toda a trilha do Carro, você deve fazer o Teste de Fuga.
Role 2 dados de teste. Se a soma for **Maior que 8**, você VENCE.
Munição: Pode gastar munição (+1 no total da soma por munição gasta).
Se falhar: Sofre 1 de Dano (Vida). Você pode tentar novamente no próximo turno. Para tentar *imediatamente* no mesmo turno, deve gastar 1 Suprimento.

---

## 📂 Estrutura do Repositório
*   `C:/Users/maiki/Documents/PESSOAL/z-scavenger-d6/`
    *   `docs/`
    *   `img/` — Assets de imagem Low Ink gerados por IA.
    *   `folha_de_jogo.html` — Tabuleiro interativo e gerador de impressão atualizado.
    *   `folha_de_jogo.pdf` — PDF legado.

## 🎨 Decisões de Design & Arquitetura Visiva
1.  **Estilo Low Ink Estrito:** Fundo branco/creme (#faf8f5), contornos e linhas pretas fortes (#111111), otimizado para impressão doméstica A4.
2.  **Encaixe A4 Perfeito:** Zera margens no print CSS (`@page { margin: 0; }`).
3.  **Hibridismo Físico/Digital:** HTML interativo, checkbox de combos e rolador de dados Javascript nativo.
