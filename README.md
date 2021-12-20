//Input / Output Array

#include <iostream>
#include <string>
#include <iomanip>
#include <array>

using namespace std;


int main()
{
	int Numbers[5];

	for (int i = 0; i < 5; i++) {

		cout << "Enter number " << i + 1 << ": ";
		cin >> Numbers[i];
		while (cin.fail())
		{
			cin.clear();
			cin.ignore(1000, '\n');
			cout << "\nInvalid Input! Try again\nEnter number " << i + 1 << ": ";
			cin >> Numbers[i];
		}
	}
	cout << endl;
	for (auto Number : Numbers) {
		cout << Number << endl;
	}
}
//Array art
  
#include <iostream>
#include <string>
#include <iomanip>
#include <array>

using namespace std;


int main()
{

	string theFace[5][5]{
		{"-","-","-","-","-"}, //First row
		{"-","O","-","O","-"}, //second row
		{"-","@","@","@","-"}, //third row
		{"-","^","^","^","-"}, //fourth row
		{"-","v","v","v","-"} //fifth row
	};
	for (int i = 0; i < 5; i++) {
		for (int j = 0; j < 5; j++)
		{
			cout << theFace[i][j];
		}
		cout << endl;
	}
}
