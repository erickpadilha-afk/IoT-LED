# IoT-LED
<p>Circuito feito no site Tinkercad, no qual faz com que um botão seja pressionado e acenda uma pequena luz de LED.</p>

<h1><strong>Código para o funcionamento do LED</strong></h1>

int buttonPin = 7; <br>
int ledPin = 10; <br>
bool estadoLed = false; <br>
void setup() <br>
{ <br>
  pinMode(ledPin, OUTPUT); <br>
  pinMode(buttonPin, INPUT); <br>
}<br> 

void loop() <br>
{ <br>
  if (digitalRead(buttonPin) == HIGH){ <br>
estadoLed = !estadoLed; <br>
    digitalWrite(ledPin,estadoLed); <br>
    delay(100); <br>
} <br>
} <br>

<h2><strong>Materiais que foram usados</strong></h2>

| Qtd | Componente |
|-----|------------|
| 1 | Placa Arduino UNO |
| 1 | Cabo USB |
| 1 | Protoboard |
| 1 | Resistor de 200 Ω ou 220 Ω |
| 1 | Resistor de 10 kΩ |
| 1 | Botão tipo push button |
| 1 | LED vermelho difuso de 5 mm |
| — | Fios de jumper macho-macho |
