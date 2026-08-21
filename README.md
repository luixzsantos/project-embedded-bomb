<h1>💣 Embedded Bomb — Arduino Uno</h1>

<h2>📌 Sobre o projeto</h2>

<p>
Este projeto consiste em uma <strong>simulação de bomba utilizando Arduino Uno</strong>,
desenvolvida para demonstrar conceitos de sistemas embarcados, programação em C++
e integração entre hardware e software. O sistema utiliza um teclado matricial para
entrada da senha, um display LCD para apresentar as informações e um buzzer para
emitir os sons durante a contagem regressiva.
</p>

<h2>🔧 Componentes</h2>

<ul>
    <li>Arduino Uno</li>
    <li>Teclado matricial 4x4</li>
    <li>Display LCD 16x2</li>
    <li>Buzzer/Piezo</li>
    <li>Protoboard</li>
    <li>Jumpers</li>
</ul>

<h2>⚙️ Como funciona</h2>

<p>
Ao ligar o Arduino, o display LCD apresenta:
</p>

<pre>Enter password</pre>

<p>
O usuário deve digitar a senha utilizando o teclado matricial.
</p>

<h3>🔐 Senha</h3>

<p>A senha configurada atualmente no projeto é:</p>

<pre>7553608</pre>

<p>
Depois de inserir os 7 caracteres, o Arduino compara a senha digitada
com a senha armazenada no código.
</p>

<p>
Se a senha estiver <strong>errada</strong>, o display apresenta:
</p>

<pre>Password wrong</pre>

<p>
Se a senha estiver <strong>correta</strong>, começa uma contagem regressiva
de <strong>20 segundos</strong>. Durante a contagem, o buzzer emite sinais
sonoros e o LCD mostra o tempo restante.
</p>

<p>
Quando a contagem chega a <code>0</code>, o LCD apresenta:
</p>

<pre>BOOOM!!!!!!</pre>

<p>
O buzzer permanece acionado por alguns segundos, representando o final
da simulação.
</p>

<h2>🎛️ Teclado</h2>

<p>
A tecla <code>*</code> pode ser utilizada para <strong>limpar a entrada
da senha</strong>.
</p>

<table>
    <thead>
        <tr>
            <th>Teclado</th>
            <th>Arduino Uno</th>
        </tr>
    </thead>
    <tbody>
        <tr><td>Linha 1</td><td>A0</td></tr>
        <tr><td>Linha 2</td><td>A1</td></tr>
        <tr><td>Linha 3</td><td>D11</td></tr>
        <tr><td>Linha 4</td><td>D10</td></tr>
        <tr><td>Coluna 1</td><td>D9</td></tr>
        <tr><td>Coluna 2</td><td>D8</td></tr>
        <tr><td>Coluna 3</td><td>D7</td></tr>
        <tr><td>Coluna 4</td><td>D6</td></tr>
    </tbody>
</table>

<h2>🖥️ Display LCD</h2>

<table>
    <thead>
        <tr>
            <th>LCD</th>
            <th>Arduino Uno</th>
        </tr>
    </thead>
    <tbody>
        <tr><td>RS</td><td>D5</td></tr>
        <tr><td>E</td><td>D4</td></tr>
        <tr><td>D4</td><td>D3</td></tr>
        <tr><td>D5</td><td>D2</td></tr>
        <tr><td>D6</td><td>A4</td></tr>
        <tr><td>D7</td><td>A5</td></tr>
    </tbody>
</table>

<h2>🔊 Buzzer</h2>

<p>
O buzzer está conectado ao pino <strong>D13</strong>.
Ele é utilizado para fornecer feedback sonoro durante a contagem
regressiva e no final da simulação.
</p>

<h2>🤔 Por que Arduino Uno?</h2>

<p>
O <strong>Arduino Uno</strong> foi escolhido por ser uma plataforma simples,
acessível e adequada para projetos acadêmicos e de introdução a sistemas
embarcados. Ele possui entradas e saídas suficientes para conectar o teclado,
o LCD e o buzzer, além de possuir ampla compatibilidade com bibliotecas
e ferramentas de desenvolvimento.
</p>

<p>
Neste projeto, o Arduino é responsável por <strong>receber a entrada do teclado,
processar a senha, controlar o display e comandar o buzzer</strong>.
</p>

<h2>💻 Tecnologias utilizadas</h2>

<ul>
    <li>C++</li>
    <li>Arduino Framework</li>
    <li>PlatformIO</li>
    <li>Biblioteca Keypad</li>
    <li>Biblioteca LiquidCrystal</li>
</ul>

<h2>🚀 Como executar</h2>

<ol>
    <li>Instale o Visual Studio Code.</li>
    <li>Instale a extensão PlatformIO.</li>
    <li>Clone este repositório.</li>
    <li>Abra o projeto no PlatformIO.</li>
    <li>Conecte o Arduino Uno ao computador.</li>
    <li>Compile o projeto.</li>
    <li>Faça o upload para o Arduino.</li>
    <li>Monte o circuito seguindo a configuração dos pinos.</li>
    <li>Ligue o sistema.</li>
    <li>Digite a senha <code>7553608</code>.</li>
    <li>Observe a contagem regressiva no LCD.</li>
</ol>

<h2>📁 Estrutura do projeto</h2>

<pre>
project-embedded-bomb/
├── platformio.ini
├── README.md
└── src/
    └── main.cpp
</pre>

<h2>⚠️ Aviso</h2>

<p>
Este projeto é <strong>exclusivamente educacional</strong> e representa uma
simulação eletrônica. Não utiliza explosivos, materiais pirotécnicos ou
mecanismos destinados a causar danos.
</p>

<h2>👨‍💻 Autor</h2>

<p>
<strong>Luiz Fernando Araujo Santos</strong>
</p>
