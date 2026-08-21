# Project Embedded Bomb

Projeto de sistema embarcado desenvolvido com Arduino Uno, teclado matricial 4x4, display LCD 16x2 e buzzer.

## Tecnologias

- Arduino Uno
- PlatformIO
- C++ / Arduino Framework
- Keypad
- LiquidCrystal

## Estrutura

```text
project-embedded-bomb/
├── platformio.ini
├── src/
│   └── main.cpp
└── README.md
```

## Funcionamento

O sistema solicita uma senha pelo teclado matricial. Quando a senha configurada é inserida corretamente, inicia-se uma contagem regressiva no LCD acompanhada por sinal sonoro. Ao final, o display apresenta a mensagem `BOOOM!!!!!!`.

> Este projeto é uma simulação acadêmica de um dispositivo temporizado e não deve ser utilizado para criar ou acionar explosivos reais.
