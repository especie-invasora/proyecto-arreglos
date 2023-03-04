# proyecto-arreglos
this program is for  make the practice 2 of  EDA

#include <iostream>
using std :: cout ;
using std :: endl ;
using std :: cin ;


/*
 Programa que realiza la implementación de la escitala espartana
 Para cifrar y descifrar.
*/
void crearMensaje();
void descifrarMensaje();
int main(){
 short opcion=0;
    while (1){
 cout << "*** ESCÍTALA ESPARTANA ***" << endl;
 cout << " Que operacion  desea realizar"<< endl ;
 cout << "opcion1 crear un cifrado" << endl;
 cout << "opcion2 desifrar un mensaje "<< endl ;
 cout << "3 obcion no valida";
 cin >> opcion;
   switch(opcion){
   case 1:
     crearMensaje();
              break;
   case 2:
  descifrarMensaje();
              break;
 case 3:
           return 0;
            default:
 printf("Opción no válida.\n");
 } 
    }
 
 

void crearMensaje(){
 int ren, col, i, j, k=0;
 cout << "porfavor proporcione el tamaño de la matriz" << endl;
cout << "renglones (--)" << endl;
cin >> ren ;
 cout << "porfavor ahora selecione las columnas (||) << endl ";
 cin >> col;
 char escitala[ren][col];
 char texto[ren*col];
 cout << "proporcione el texto de favor" << endl;
 cin >> texto;
 for(i=0 ; i<ren ; i++)
 for (j=0 ; j<col ; j++)
 escitala[i][j] = texto[k++];
cout << "El texto de la escitala espartana queda si  " << endl ;
 for (i=0 ; i<col ; i++)
 for (j=0 ; j<ren ; j++)
cout<< escitala[i][j];
 endl;
}
void descifrarMensaje(){
 int ren, col, i, j, k=0;
cout << "ingresa el tamaño de la citacala" << endl;
cout << "renglones" << endl;
cin >> ren ;
 cout << "columnas" << endl;
 cin >> col;
 char escitala[ren][col];
 char texto[ren*col];
cout << "el texto  desifraso es ";
cin >> texto ;
 for (i=0 ; i<col ; i++)
 for (j=0 ; j<ren ; j++)
 escitala[j][i] = texto[k++];
 cout << "el texto cifrado es:" << endl;
 for (i=0 ; i<ren ; i++)
 for (j=0 ; j<col ; j++)
 cout << escitala[i][j]; 
 }
    
}
    
