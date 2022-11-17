# Figura_cuadrado
Estructura de datos

#include <cstdlib>
#include <iostream>

using namespace std;

class Cuadrado
{
	private:
		float lado,base,Area,perimetro;
		
		
	public:
		Triangulo() { base=0; lado=0; Area=0; perimetro=0; }
		void visualizar();
		void calcularArea();
		void calcularperimetro();
		void setBas(float ba);
		void setLa (float la);
};

void Cuadrado::visualizar()
{
	cout<<"Area y perimetro:"<<endl;
	cout<<"base:"<<base<<endl;
	cout<<"lado:"<<lado<<endl;
	cout<<"Area:"<<Area<<endl;
	cout<<"perimetro:"<<perimetro<<endl;
}

void Cuadrado::calcularArea ()		
{
	Area = lado*lado;
}
void Cuadrado::calcularperimetro()
{
    perimetro= lado+lado;	
}
void Cuadrado::setBas(float ba)
{
	base = ba;
}
void Cuadrado::setLa(float la)
{
	lado = la;
}

  
  
 principal cuadrado
  
  #include "Cuadrado.h"0
#include <cstdlib>
#include <iostream>

using namespace std;

int main (int argc, char * arg[])
{
	float la,ba,area;
	string c;


cout<<"Bienvenido"<<endl;
cout<<"\tPrograma que calcula el area y perimetro"<<endl;

cout<<"Escribe la figura:"<<endl;
cin>>c;
cout<<"Escribe el lado:"<<endl;
cin>>la;
cout<<"Escribe la base :"<<endl;
cin>>ba;

Cuadrado C;
C.setLa(la);
C.setBas(ba);
C.calcularArea();
C.calcularperimetro();
C.visualizar();

getchar();
system("pause");
return 0;
}
