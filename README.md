# tinkercad
movimiento de un servomotor con ayuda de un software de programación
Movimiento de Servomotor

Este proyecto de tinkercad se basa en hacer girar un servomotor con intervalos de movimiento de 1000 milisegundos, donde
en los primeros 100 milisegundos entra en estado alto y el servomotor se mueve durante ese intervalo de tiempo hasta que
llega el tiempo posterior donde entra en estado bajo y se detiene el servomotor hasta el proximo cambio de estado logico.
Haciendo conexiones del pin negativo y el pin positivo del servomotor al arduino #1 y un tercer pin o cable de datos 
(pin 13) al cual le entran las señales HIGH y LOW.

void setup()
{
  pinMode(13, OUTPUT);
}

void loop()
{
  digitalWrite(13, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(13, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
}
