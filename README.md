# 8-Feb
int tim1;
int tim2;
int tim3;
int verde = 13;
int amarillo = 7;
int rojo = 2;

void setup() {
pinMode(verde, OUTPUT);
pinMode(amarillo, OUTPUT);
 pinMode(rojo, OUTPUT);
 Serial.begin (9600);
 Serial.println("¿Cuántos segundos quieres para el led verde?");
  delay(4000);
  tim1 = Serial.parseInt ();
 Serial.println("¿Cuántos segundos quieres para el led amarillo?");
  delay(4000);
  tim2 = Serial.parseInt ();
 Serial.println("¿Cuántos segundos quieres para el led rojo?");
  delay(4000);
  tim3 = Serial.parseInt ();
}

 void loop()
{
 digitalWrite (verde, HIGH);
 delay (tim1*1000);
 digitalWrite (verde, LOW);
 delay (tim1*1000);

 digitalWrite (amarillo, HIGH);
 delay (tim2*1000);
 digitalWrite (amarillo, LOW);
 delay (tim2*1000);

 digitalWrite (rojo, HIGH);
 delay (tim3*1000);
 digitalWrite (rojo, LOW);
 delay (tim3*1000);
}
