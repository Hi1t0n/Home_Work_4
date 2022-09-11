# Home_Work_4
/*Разработать программу, которая выводит на экран линию из символов. 
Число символов, какой использовать символ, 
и какая будет линия - вертикальная, или горизонтальная - указывает пользователь.*/
#include <iostream>
using namespace std;
int main()
{
	setlocale(LC_ALL, "Russian");
	int a, b, c;
	char symbol;
	cout << "Введите символ: ";
	cin >> symbol;
	cout << "Введите кол-во символов: " << endl;
	cin >> a;
	cout << "Выберите тип линии: \n" << "1 - По горизонтали \n" << "2 - По вертикали" << endl;
	cin >> b;
	c = 0;
	switch (b)
	{
	case 1:
		while (c < a) 
		{
			cout << symbol << " ";
			c++;
		}
		break;
	case 2:
		while (c < a)
		{
			cout << symbol << endl;
			c++;
		}
		break;
	default:
		{
			cout << "Ошибка! Вы ввели не корректный тип линии";
		}
		break;
	}
}
