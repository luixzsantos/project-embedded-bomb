💣 Embedded Bomb — Arduino Uno
📌 Sobre o projeto

Este projeto consiste em uma simulação de bomba utilizando Arduino Uno, desenvolvida para demonstrar conceitos de sistemas embarcados, programação em C++ e integração entre hardware e software. O sistema utiliza um teclado matricial para entrada da senha, um display LCD para apresentar as informações e um buzzer para emitir os sons durante a contagem regressiva.

🔧 Componentes
Arduino Uno
Teclado matricial 4x4
Display LCD 16x2
Buzzer/Piezo
Protoboard
Jumpers
⚙️ Como funciona

Ao ligar o Arduino, o display LCD apresenta:

Enter password

O usuário deve digitar a senha utilizando o teclado matricial.

A senha atual do projeto é:

7553608

Depois de inserir os 7 caracteres, o Arduino compara a senha digitada com a senha armazenada no código.

Se a senha estiver errada, o display apresenta:

Password wrong

Se a senha estiver correta, começa uma contagem regressiva de 20 segundos. Durante a contagem, o buzzer emite sinais sonoros e o LCD mostra o tempo restante.

Quando a contagem chega a 0, o LCD apresenta:

BOOOM!!!!!!

e o buzzer permanece acionado por alguns segundos, representando o final da simulação.

🎛️ Teclado

A tecla * pode ser utilizada para limpar a entrada da senha.

O teclado está conectado ao Arduino da seguinte maneira:

Teclado	Arduino
Linha 1	A0
Linha 2	A1
Linha 3	D11
Linha 4	D10
Coluna 1	D9
Coluna 2	D8
Coluna 3	D7
Coluna 4	D6
🖥️ Display LCD

O LCD utiliza a seguinte configuração:

LCD	Arduino
RS	D5
E	D4
D4	D3
D5	D2
D6	A4
D7	A5
🔊 Buzzer

O buzzer está conectado ao:

D13

Ele é utilizado para fornecer o feedback sonoro durante a contagem regressiva e no final da simulação.

🤔 Por que Arduino Uno?

O Arduino Uno foi escolhido porque é uma plataforma simples e adequada para projetos acadêmicos e de introdução a sistemas embarcados. Ele possui entradas e saídas digitais e analógicas suficientes para conectar o teclado, LCD e buzzer, além de possuir ampla compatibilidade com bibliotecas e ferramentas de desenvolvimento.

Neste projeto, o Arduino é responsável por receber a entrada do teclado, processar a senha, controlar o display e comandar o buzzer.

💻 Tecnologias utilizadas
C++
Arduino Framework
PlatformIO
Biblioteca Keypad
Biblioteca LiquidCrystal
🚀 Como executar
Instale o Visual Studio Code.
Instale a extensão PlatformIO.
Clone este repositório.
Abra o projeto no PlatformIO.
Conecte o Arduino Uno ao computador.
Compile o projeto.
Faça o upload para o Arduino.
Monte o circuito seguindo a configuração dos pinos.
Ligue o sistema e digite:
7553608
Observe a contagem regressiva no LCD.
📁 Estrutura
project-embedded-bomb/
├── platformio.ini
├── README.md
└── src/
    └── main.cpp
⚠️ Aviso

Este projeto é exclusivamente educacional e representa uma simulação eletrônica. Não utiliza explosivos, materiais pirotécnicos ou mecanismos destinados a causar danos.

👨‍💻 Autor

Luiz Fernando Araujo Santos
