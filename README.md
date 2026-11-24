# Protocolo Zero

Protótipo de jogo 2D em Python + Pygame para a disciplina de POO[cite: 1].

## Ideia do protótipo
Um engenheiro de IA sobrevive a um mundo dominado por máquinas, explora áreas, coleta componentes do computador e tenta executar o software para desativar as IAs (ou perde toda a vida no caminho)[cite: 1, 2].

## Equipe
- Rodolfo Zion Ruthes Brito[cite: 1]
- Pedro Ricardo Ferreira Moreira[cite: 1]
- Eduardo Moraes de Oliveira[cite: 1]
- Lucas Viana Gusmão[cite: 1]

## Conceitos de POO
- **Encapsulamento:** vida e inventário do jogador controlados por métodos[cite: 2].
- **Abstração:** classe `Entidade` base com `update()` e `draw()`[cite: 2].
- **Herança e Polimorfismo:** `Jogador` e `Inimigo` (`InimigoRobo`, `InimigoDrone`) com comportamentos e ataques próprios[cite: 2].
- **Associação, Agregação e Composição:** interação entre entidades, fase, inventário e computador[cite: 2, 4].

## Próximos passos (protótipo)
- [ ] Subir estrutura inicial do projeto
- [ ] Implementar movimentação básica e colisão
- [ ] Implementar coleta de peças e inventário
- [ ] Implementar inimigos e condição de vitória/derrota
