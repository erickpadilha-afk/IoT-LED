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
