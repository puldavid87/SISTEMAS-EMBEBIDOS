//llamar a la matriz de datos
#include"matriz_entrenamiento.h"
//extern-> otra forma de llamar a matriz
//extern matriz[fil][col]
#define col 5
#define fil 120


//5  3,5 1,3 0,3




//6  3 4,8 1,8

float datos_prueba[5]={6,3,4.8,1.8,3};
int j=0; // moverse en filas
int i=0; //moverse en columnas
float potencia; // potencia de atributos
float raiz;  // distancia de dos puntos
float dist_menor=3000; // almacenar la menor distanci
float etiqueta;
void setup() {
Serial.begin(9600);
/*
 *programa para imprimir los datos de entrenamiento
 *
for(int j=0;j<fil;j++){ // moverse en filas
  for(int i=0;i<col;i++){ //moverse en columnas
     Serial.print(matriz[j][i]); // imprime valores de matriz
     Serial.print(','); // separador de datos
    }
    Serial.println(' '); // separador de filas
  }
*/
}

void loop() {
  for(j=0;j<fil;j++){ // moverse en filas
     for(i=0;i<col-1;i++){ // moverse en columnas
       potencia=potencia+pow(matriz[j][i]-datos_prueba[i],2); // potencia dentre columnas
      }
      raiz=sqrt(potencia); // raiz de potencias (distancia entre dos puntos)
      //Serial.println(raiz);
      potencia=0; //reinicio variable
      if(raiz<dist_menor){ //comparo a distancia menor
        dist_menor=raiz; // cambio de valor
        etiqueta=matriz[j][4]; // asigno predicción de etiqueta
       }
    }
    Serial.println(etiqueta); // imprimo etiqueta
    if(etiqueta==datos_prueba[4]) // comparo predicción.
      Serial.println("PREDICCION CORRECTA");
     else
      Serial.println("PREDICCION ERRONEA");
   delay(5000);   
}
