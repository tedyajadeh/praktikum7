# praktikum7


##soal1.cpp
**Alur Argoritma**
1. Mulai program tersebut 
2. input interger fungsi (int, int)
4. input interger a dan b dan deskripsikan a=0, dan b=1.
5. jika nilai suku satu (b) adalah =1 dan jika nilai suku dua (a) adalah =0.
6. maka cetak rumus fungsi iteratif menggunakan for intruksikan fungsi fibionici di awali dengan 2 dan di akhiri dengan indexs suku
7. deskripsikan variable untuk mencetak fuungsi selanjutnya.
8. cetak suku fibionici menggunakan pemanggilan fungsi itertif.

**Pseudecode**
1. int typedatar (a, b)
2. if (bill=1) return a
3. if (bill=0) return b
4. for (int i=2; i<=bil; i++)
5. c= a+b, a=b, b=c
6. end 

**CODE PROGRAM**
```
#include <iostream>

using namespace std;

int iteratif (int bil, int a, int b, int c)
{
a=0, b=1;
if (bil == 1) return b;
if (bil == 0) return a;

else{
for(int i=2; i<=bil; i++){

c = a + b;
a = b;
b = c;
}
return c;
}
}

int main()
{
int bil, a, b,c;

cout<<"Masukkan bilangan deret ke-: ";
cin>>bil;
cout<<"\nBilangan fibonaccinya untuk "<<bil<<" adalah ";
cout<< iteratif ( bil,  a,  b,  c);

return 0;
}
```
**Hasil**
![hasil](https://raw.githubusercontent.com/Amirul29/praktikum7/master/soal1.png)


##Soal2.cpp

**Alur Argoritma**
1. Mulai program tersebut 
2. input interger fungsi (int a, intb).
3. jika nilai interger (b==0) return 0.
4. jika nilai (b>0) intruksikan return a + type data (a, b - 1).
5. Sebaliknya return (-a) + type Data (a, b+1)
6. masukan variabel a,b untuk menginput nilai awal dan dibagi degan nilai selanjutny.
7. cetak nilai perkalian dengan memanggil funsi rekrusif menggunkan type datany.

**Pseudecode**
```
deskripsi a x b =
1. 0, untuk b = 0
2. a + (a x (b-1)), untuk b > 0
3. -a + (a x (b + 1)), untuk b < 0
4. end
```

**CODE PROGRAM**
```
#include <iostream>
using namespace std;


int kali_rekursif(int a, int b)
{
 if (b==0)
  return 0;
 else if (b > 0)
  return a + kali_rekursif(a, b - 1);
 else
  return (-a) + kali_rekursif(a, b+1);
}


main()
{
 int a, b;
 cout << "Masukan Bilangan : ";
 cin >> a;
 cout << "Dikli Dengan :";
 cin >> b;
 cout << " AxB = " << kali_rekursif(a, b) << endl;
}
```
**Hasiil**
![Hasil](https://raw.githubusercontent.com/Amirul29/praktikum7/master/soal2.png)

##soal3.cpp
**Alur Argoritma**
1. Mulai program tersebut 
2. input menggunakan initruksi void dan menggunakan pointer untuk menetapakan void typedata (char *s)
3. jika nilai **s!=0**--> menggunakan Pointer(*) maka masukan intruksi membalik (&s[1])
4. masuan char untuk intruksi kata yang ingin kita ubah dan intruksi balik
5. cetak pemblikan kata dengan memanggil funsi rekrusif menggunkan type datany.

**Pseudecoede**
```
#include
#include
void balik(char *k){
if(*k!=�){
balik(&k[1]);
cout<
}
}main(){
char *kata=�....�;--> //untuk masukan kata
balik(kata);
cout<
return 0;
```
**CODE PROGRAM**
```
#include<iostream>
#include<string.h>

using namespace std;
void balik(char *s)
{ if (*s != '\0'){
balik(&s[1]);
cout << s[0];
}
}
int main()
{
      char* kata = (char*) "amirul";
    balik(kata); cout << endl;
    return 0;

}
```
**Hasil**
![hasil](https://raw.githubusercontent.com/Amirul29/praktikum7/master/soal3.png)