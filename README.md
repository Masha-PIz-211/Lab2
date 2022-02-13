/* ********************** *
* Власова Мария 
* Программирование циклов с пред- и постусловием
* Вариант 2
* ***********************/

#include <iostream>
#include <cmath>

using namespace std;

int main()
{
  setlocale(0, "");
  float m, c=298792, m0=1.675, v=50000;
  cout << "Таблица зависимости массы от скорости нейтрона \n";
  while (v<=290000) 
  { 
  	m=m0/sqrt(1-pow(v/c,2));
  	printf(" v = %8.1f   m = %.3f \n",v,m);
  	if (v<250000)
  	  v=v+50000;
  	else
  	  v=v+10000;
  }
  system("pause");
  return 0;
}
