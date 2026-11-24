## Protocolo Zero POO 🤖

Protótipo de jogo 2D desenvolvido em Python com a biblioteca Pygame para a disciplina de Programação Orientada a Objetos (POO).

# 🎮 Sobre o Jogo

Protocolo Zero é ambientado em um cenário pós-apocalíptico dominado por inteligências artificiais rebeldes. O jogador controla um engenheiro de IA sobrevivente que precisa explorar instalações abandonadas, desviar e combater máquinas hostis e coletar peças fundamentais para montar um computador funcional. O objetivo final é carregar e executar um software capaz de neutralizar o controle das IAs sobre o mundo.

# Mecânicas Principais

-Exploração: Movimentação em ambiente 2D com obstáculos e áreas bloqueadas.

-Sobrevivência: Gerenciamento de pontos de vida diante de máquinas hostis.

-Coleta e Inventário: Busca pelos 5 componentes essenciais:

Placa-mãe

Processador

Memória RAM

Armazenamento

Fonte de alimentação

Condições de Fim de Jogo:

Vitória: Reunir as peças, montar o computador e executar o software.

Derrota: Os pontos de vida do personagem chegarem a zero.

👥 Equipe de Desenvolvimento
Rodolfo Zion Ruthes Brito

Pedro Ricardo Ferreira Moreira

Eduardo Moraes de Oliveira

Lucas Viana Gusmão

# 🧩 Aplicação dos Conceitos de POO

O projeto foi estruturado com foco na aplicação prática dos pilares da Orientação a Objetos:

-Encapsulamento: Atributos críticos (como vida do jogador) são protegidos e manipulados apenas via métodos específicos (take_damage(), heal()).

-Abstração: Classes-base como Entidade definem a interface comum (update(), draw(), take_damage()) sem expor detalhes de implementação.

-Herança: Jogador e Inimigo herdam da base Entidade. Tipos específicos de inimigos (InimigoRobo, InimigoDrone) herdam de Inimigo.

-Polimorfismo e Sobrescrita: Inimigos compartilham a interface attack() e update(), mas executam comportamentos distintos (combate corpo a corpo vs. disparo de projéteis à distância).

-Composição: A classe principal Jogo contém a Fase atual e a InterfaceJogo. O Jogador contém o seu Inventario.

-Agregação: A Fase mantém referências ao Jogador, inimigos, componentes e obstáculos, permitindo que entidades persistam entre transições.

-Associação: Relações de interação direta, como combate entre Jogador e Inimigo, ou uso dos itens coletados no Computador.

# 🛠️ Tecnologias Utilizadas

Linguagem: Python 3.10+

Biblioteca gráfica: Pygame

# 🚀 Como Executar o Protótipo

Pré-requisitos

Certifique-se de ter o Python instalado na sua máquina.

Passo a passo

Clone o repositório:

git clone https://github.com/SEU_USUARIO/protocolo-zero.git
cd protocolo-zero


Crie e ative um ambiente virtual (recomendado):

Linux / macOS:

python3 -m venv .venv
source .venv/bin/activate


Windows:

python -m venv .venv
.venv\Scripts\activate


Instale as dependências:

pip install -r requirements.txt


Inicie o jogo:

python main.py


📋 Status do Protótipo

[ ] Criação da estrutura de pastas e classes base

[ ] Movimentação e colisão básica do Jogador

[ ] Sistema de componentes e inventário

[ ] Inimigos básicos (Robô e Drone)

[ ] Interface (HUD de vida e inventário)

[ ] Montagem do computador e condição de vitória/derrota
