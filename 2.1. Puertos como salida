/*
 * CAPÍTULO II: PUERTOS DIGITALES
 * CÓDIGO 1: Manejo de puertos configurados como salida
 * Objetivo: Enceder y apagar leds desde Arduino con diferentes 
 *           formas de uso de variables
 *           No necesita librerías
 * Funciones de programación:           
 *           pinMode(pin, MODO) 
 *                        MODO-> INPUT/OUTPUT
 *           digitalWrite(pin, ESTADO)             
 *                        ESTADO-> HIGH, LOW
 *           delay(ms)
 *                 ms-> tiempo en milisegundos
 */
#define led1 8  // uso de #define que no su puede alterar su valor
int led2=9;    // variable normal, no recomendable
const int led3=10; //variable constante, recomendable
void setup() {
pinMode(led1,OUTPUT); // pin8 declarado como salida
pinMode(led2,OUTPUT); // pin9 declarado como salida
pinMode(led3,OUTPUT); // pin10 declarado como salida
}

void loop() {
  // Enciede led1 y apaga en un segundo
digitalWrite(led1,HIGH); //Envía 5 voltios a pin 8
delay(1000); // se detiene microncontrolador por 1 segundo
digitalWrite(led1,LOW); //Envía 0 voltios a pin 8
delay(1000); // se detiene microncontrolador por 1 segundo
//mientras el led2 se encuentra encendido el led3 está apagado y viceversa
// cada medio segundo
digitalWrite(led2,HIGH); //Envía 5 voltios a pin 9
digitalWrite(led3,LOW); //Envía 0 voltios a pin 10
delay(500); // se detiene microncontrolador por medio segundo
digitalWrite(led2,LOW); //Envía 0 voltios a pin 9
digitalWrite(led3,HIGH); //Envía 5 voltios a pin 10
delay(500); // se detiene microncontrolador por medio segundo
}
