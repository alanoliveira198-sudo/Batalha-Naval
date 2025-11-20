# Batalha-Naval
# Desafio Batalha Naval - Posicionamento de Navios

Bem-vindo ao desafio "Batalha Naval - Posicionamento de Navios"! Neste jogo clássico, os jogadores posicionam secretamente seus navios em um tabuleiro e tentam acertar as posições dos navios adversários.

A empresa MateCheck contratou você para desenvolver a parte inicial do jogo, que consiste no posicionamento dos navios em um tabuleiro simplificado.

O desafio é dividido em três níveis: Novato, Aventureiro e Mestre, com cada nível adicionando mais complexidade ao anterior. Você deve escolher qual desafio quer realizar.

### 🚨 Atenção:

O nível Novato do desafio é focado em utilizar vetores (arrays unidimensionais) e matrizes (arrays bidimensionais) em C para representar o tabuleiro e posicionar dois navios com tamanhos e orientações fixas, exibindo o resultado final.

### 🎮 Nível Novato: Posicionando Navios no Tabuleiro 

Neste primeiro desafio, você dará o primeiro passo na construção do seu jogo de Batalha Naval. Você utilizará seus conhecimentos de vetores e matrizes em C para representar um tabuleiro   $10\times 10$  e posicionar dois navios: um na vertical e outro na horizontal.

### 🚩 Objetivo:

Representar um tabuleiro de Batalha Naval  $10\times 10$  e posicionar dois navios de tamanho 3 (um vertical e um horizontal), garantindo que estejam dentro dos limites e não se sobreponham, e em seguida, exibir o tabuleiro no console.

### ⚙️ Funcionalidades do Sistema:

Representação do Tabuleiro: Utilizar uma matriz (array bidimensional) de tamanho $10\times 10$ para o tabuleiro.
Inicializar todas as posições com o valor $0$ (água).

# Representação e Posicionamento dos Navios:
Declarar navios com tamanho fixo 3.

Representar as posições dos navios na matriz do tabuleiro com o valor  3.

Um navio será posicionado horizontalmente e o outro verticalmente.

As coordenadas iniciais de cada navio serão definidas no código (sem input do usuário).

Exibição do Tabuleiro: Exibir a matriz completa no console com loops aninhados e printf, mostrando 0 para água e 3  para as partes dos navios.

### 📥 Entrada (Definida no Código) e 📤 Saída de Dados:

Entrada: As coordenadas iniciais (linha e coluna) de cada navio são definidas diretamente no código.

Saída: O sistema exibirá o tabuleiro $10\times 10$ completo no console, de forma clara e organizada, com os navios posicionados.

## 🧩 Como compilar e executar

No terminal (CMD ou PowerShell), dentro da pasta do projeto:

```bash
gcc novato.c -o novato -Wall -Wextra -std=c11

```



### 🛡️ Nível Aventureiro: Adicionando Interatividade e Validação Robusta

No nível Aventureiro, você expandirá o sistema para permitir que o usuário escolha as posições dos navios e implementará validações mais robustas para garantir um posicionamento correto.

### 🆕 Diferença em relação ao Nível Novato:


Entrada de Coordenadas pelo Usuário: O programa solicitará ao usuário as coordenadas iniciais (linha e coluna) e a orientação (Horizontal/Vertical) de cada navio.

Validação de Limites: Implementação de uma função de validação que verifica se o navio, em sua orientação e tamanho, está completamente dentro dos limites do tabuleiro   $10\times 10$.

Validação de Sobreposição: Implementação de uma função que verifica se o novo navio a ser posicionado não se sobrepõe a navios já existentes (posições com valor  3).


### ⚙️ Funcionalidades do Sistema:

O sistema solicitará interativamente as coordenadas iniciais para o posicionamento dos dois navios.

O sistema repetirá a solicitação caso as coordenadas resultem em um navio fora dos limites ou sobreposto.

### 📥 Entrada e 📤 Saída de Dados:

Entrada: O usuário insere as coordenadas iniciais e orientação de cada navio via terminal.

Saída: O sistema exibe mensagens de erro em caso de validação falha e o tabuleiro final após o posicionamento correto.

## 🧩 Como compilar e executar

No terminal (CMD ou PowerShell), dentro da pasta do projeto:

```bash
gcc aventureiro.c -o aventureiro -Wall -Wextra -std=c11

```





### 🏆 Nível Mestre: Múltiplos Navios e Estruturas de Dados

No nível Mestre, você aumentará a complexidade do posicionamento, utilizando estruturas (struct) para gerenciar os navios e permitindo o posicionamento de múltiplos tipos de navios.

### 🆕 Diferença em relação ao Nível Aventureiro:

Estruturas de Dados: Utilização de struct em C para representar um Navio, contendo propriedades como:

Tamanho

Coordenada Inicial (Linha, Coluna)

Orientação (Horizontal, Vertical)

Múltiplos Navios: O sistema permitirá o posicionamento de uma frota:

1 Porta-Aviões (Tamanho 5)

2 Encouraçados (Tamanho 4)

3 Submarinos (Tamanho 3)

Tipos de Navio no Tabuleiro: Cada tipo de navio será representado por um valor diferente no tabuleiro (ex: Porta-Aviões = $5$, Encouraçado = $4$, Submarino = $3$).

### ⚙️ Funcionalidades do Sistema:

O programa utilizará a estrutura struct para manipular os dados de cada navio.

O sistema irá gerenciar e validar o posicionamento de um total de 6 navios (1 de tamanho 5, 2 de tamanho 4, 3 de tamanho 3).

A exibição do tabuleiro mostrará os diferentes valores para os diferentes tipos de navios.

### 📥 Entrada e 📤 Saída de Dados:

Entrada: O usuário insere as coordenadas e orientação para cada um dos 6 navios da frota.

Saída: O sistema exibe o tabuleiro final com a frota completa posicionada e utiliza diferentes números para representar os diferentes tipos de navios.

## 🧩 Como compilar e executar

No terminal (CMD ou PowerShell), dentro da pasta do projeto:

```bash
gcc mestre.c -o mestre -Wall -Wextra -std=c11

```
































