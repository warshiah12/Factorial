# Factorial
# for loop
#include<iostream>
using namespace std;
int main()
{
	int num = 0, y, fact = 1;  //declaring variables with datatype integers
	cout << "Enter a number: " << endl;
	cin >> num;
	while (cin.fail() != 0)
	{
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Incorrect command. Enter the number again" << endl;
		cin >> num;
	}
	for (y = 1; y <= num; y++)
	{
		fact = fact * y;
	}
	cout << "Factorial = " << fact << endl;
	return 0;
}
