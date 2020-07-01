/*
 * CAPÍTULO II: PUERTOS DIGITALES
 * CÓDIGO 8: Manejo de LCD y puertos entrada
 * Objetivo: Contador de un pulsador visualizado en la LCD
 * Funciones : librería LiquidCrystial.h
 *             LiquidCrystal ( )       Inicializa la interfaz de la pantalla LCD
 *             begin(columnas, filas)  Configura uso de LCD
 *             print(data)             Imprime texto en la LCD   
 *             setCursor(columa, fila) Posiciona el cursos en la LCD
 */
#include<LiquidCrystal.h> 

LiquidCrystal lcd(13,12,11,10,9,8); // inicia lcd

const int btn=7; // variable para pin como salida
int cont=0; //variable de conteo
void setup() {
 lcd.begin(16,2); //inicia lcd con filas y columnas a emplear
 pinMode(btn,INPUT); // define pin 7 como entrada
 lcd.setCursor(0,0);  // ubicación en lcd
 lcd.print("ARDUINO"); // imprime palabra
 lcd.setCursor(0,1);  //ubicación lcd
 lcd.print("CONT:"); // imprime palabra
}

void loop() {
  if(digitalRead(btn)==LOW){  // condición de presionar botón
      delay(250); // delay antirebotes
      if(cont<20){ // condición de contador
        cont++; // incremento de variable
        lcd.setCursor(7,1); // ubicación en lcd
        lcd.print(cont); // imprime variable
      }
      else{
          lcd.setCursor(6,1); // ubicación en lcd
          lcd.print("    ");  // imprime mensaje en blanco (borrar)
          cont=0; // reinicia contador
        }
    }
}
