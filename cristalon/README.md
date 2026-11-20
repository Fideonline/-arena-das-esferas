# Cristalon

**Alpha 0.1 — O Despertar dos Cristais** · RPG de captura e batalha por turnos para navegador, com mundo e criaturas próprias, visual anime nas batalhas e mapa em pixel art.

O jogo está todo em [index.html](./index.html) (HTML, CSS e JavaScript, sem dependências). As artes dos iniciais ficam em [assets/](./assets).

## Como jogar
| Ação | Teclado | Celular |
|---|---|---|
| Andar / navegar | Setas ou WASD | Direcional |
| Confirmar (A) | Z ou Espaço | A |
| Voltar (B) | X ou Esc | B |
| Menu | Enter | MENU |

1. Na tela de título, comece um **Novo jogo** e escolha seu nome.
2. Vá ao **Laboratório da Profa. Lírio** (sul da Vila Aurora) e escolha seu parceiro.
3. Enfrente o rival **Kael**, que escolhe o elemento vantajoso contra o seu.
4. Siga para a **Rota 1** (norte). No mato alto aparecem cristalons selvagens: enfraqueça-os e use um **Cristal de Captura**.
5. Cure a equipe no **Centro de Cura** (que também vende itens) ou em casa.

O progresso fica salvo no navegador (menu → Salvar; o jogo também salva sozinho ao entrar em prédios).

## Conteúdo da Alpha 0.1
- **Iniciais:** Axolume (Água), Lavascudo (Fogo), Folhix (Planta).
- **Selvagens da Rota 1:** Piuvento (Normal), Brotim (Planta), Gotin (Água), Faiscol (Elétrico), Pedrisco (Pedra) e o raro Lumicris (Cristal).
- **Elementos:** Normal, Fogo, Água, Planta, Pedra, Elétrico e Cristal, com tabela de vantagens.
- **Sistemas:** batalha por turnos com golpes elementais, críticos, bônus de mesmo elemento, alterações de atributo, experiência, subida de nível, aprendizado de golpes, captura, equipe de até 6, mochila, loja, Cristaldex e salvamento.
- **Mapa:** Vila Aurora (casa, casa do rival, laboratório, Centro de Cura) e Rota 1 com treinador, NPCs, placas e itens no chão.

## Onde mexer
- Criaturas, golpes e elementos: objetos `SPECIES`, `MOVES`, `TYPES` e `CHART` no início do script.
- Encontros da Rota 1: `ROUTE1` (espécie e peso).
- Mapa: função `buildMap`, `BUILDINGS`, `NPCS` e `OBJS`.
- Para trocar a arte de uma criatura, coloque a imagem em `assets/` e aponte `img` (retrato quadrado) e `art` (arte completa) na espécie.
