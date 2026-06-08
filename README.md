# codigo-do-andre
codigos da esteira
int motor = 9;
int sensor = 2;


void setup() {
  pinMode(motor, OUTPUT);
  pinMode(sensor, INPUT);
  Serial.begin(9600);
}


void loop() {


  // Liga a esteira
  analogWrite(motor, 180);


  // Verifica o sensor
    if (digitalRead(sensor) == HIGH) {
    analogWrite(motor, 0); // Para a esteira
    Serial.println("Carrinho detectado");
  }
}

  delay(100);
}


  delay(100);
}
