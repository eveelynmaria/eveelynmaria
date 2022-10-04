#include <DHTesp.h>
DHTesp dhtSensor;
void setup() {
// put your setup code here, to run once:
Serial.begin(115200);
Serial.println("Iniciando Setup");
dhtSensor.setup(13,DHTesp::DHT22);
Serial.printIn("Finalizando Setup");
Serial.println("Finalizando Setup");
}
void loop() {
// put your main code here, to run repeatedly:
foat temperatura = dhtSensor.getTemperature();
float humidade = dhtSensor.getHumidity();
Serial.printIn(T"Temperatura :" + String(temperatura + "C");
Serial.printIn("Humidade : "+ String(humidade) + "%");
delay(3000);
digitalWrite(23, HIGH);
digitalWrite(23, HIGH);
delay(1000);
digitalWrite(23, LOW);
digitalWrite(23, L
