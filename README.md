#include<iostream>
using namespace std;
int main()
{
	int total_quantity=0;
	int quantity=0,bill=0;
	int choice=0;
	bool again;
	int price;
	cout << "==============================================" << endl;
	cout << "-----------Welcome to ALMADINA TRADERS--------" << endl;
start:
	cout << "==============================================" << endl;
	
	cout << "1.DAP" << endl;
	cout << "2.UREA" << endl;
	cout << "3.NP" << endl;
	cout << "4.PIONEER" << endl;
	cout << "5.DEKALB" << endl;
	cout << "6.CHECK OUT" << endl;
	cout << "Enter the number:";
	cin >> choice;
	switch (choice)
	{
	case 1:
		price = 17000;
		cout << "DAP"<<endl;
		break;
	case 2:
		price = 5000;
		cout << "UREA" << endl;
		break;
	case 3:
		price =10000 ;
		cout << "NP" << endl;
		break;
	case 4:
		go:
		cout << "1.1429"<<endl;
		cout << "2.1543" << endl;
		cout << "3.2088" << endl;
		cout << "4.1541" << endl;
		cout << "enter the choice" << endl;
		cin >> choice;
		switch (choice)
		{
		case 1:
			price = 20000;
			cout << "1429" << endl;
			break;
		case 2:
			price = 16000;
			cout << "1543" << endl;
			break;
		case 3:
			price = 21000;
			cout << "2088" << endl;
			break;
		case 4:
			price = 23000;
			cout << "1541" << endl;
			break;
		default:
			goto go;
		}
		break;
	case 5:
		goo:
		cout << "1.6321" << endl;
		cout << "2.6317" << endl;
		cout << "3.9108" << endl;
		cout << "4.6789" << endl;
		cout << "Enter the choice" << endl;
		cin >> choice;
		switch (choice)
		{
		case 1:
			price = 30000;
			cout << "6321" << endl;
			break;
		case 2:
			price = 20000;
			cout << "6317" << endl;
			break;
		case 3:
			price = 15000;
			cout << "9108" << endl;
			break;
		case 4:
			price = 17000;
			cout << "6789" << endl;
			break;
		default:
			goto goo;

		}
	
		break;
	case 6:
		cout << "check out" << endl;
		goto end;
		break;
	default:
		goto start;
	}
	cout << "Enter the quatity: ";
	cin >> quantity;
	end:
	bill = bill + (price * quantity);
	total_quantity = total_quantity + quantity;
	cout << "Do you want to purchase another another item (yes=1||No=0)" << endl;
	cin >> again;
	if (again == 1)
	{
		goto start;
	}
	cout << "Your bill is " << bill<<endl;
	cout << "Your quantity is " << total_quantity;
	return 0;
}
