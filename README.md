# Summativecode



#include <iostream>
#include <string>
using namespace std;

	
int main() {
	string name;
	string lname;
	int age;
	char question;

	cout << "Type your full name! " << endl;
	cin >> name;
	getline (cin, name);
	if (name.size() <= 6) {
		cout << "Error!" << endl;
	}
	else if (name.size() >= 7) {
		cout << "Hello " << name << ", Type your age! (16-30)" << endl;
		cin >> age;

		//age 16-18
		if (age >= 16 && age <= 18) {
			cout << name << " Your age is " << age << ". Wanna go to the mall?" << endl;
			cout << "(y/n)" << endl;
			cin >> question;
			switch (question) {
				{
			case 'y':
			case 'Y':
				cout << "Enjoy!" << endl;
				break;
				}
				{
			case 'N':
			case 'n':
				cout << "Cancelled!" << endl;
				break;
				}
			default:
				(cin.fail());
				cin.ignore();
				cout << "Error!" << endl;
			}
		}
		//age 19-20
		else if (age >= 19 && age <= 20) {
			cout << name << " Your age is " << age << ". Wanna go to the theme park?" << endl;
			cout << "(y/n)" << endl;
			cin >> question;
			switch (question) {
				{
			case 'y':
			case 'Y':
				cout << "Enjoy!" << endl;
				break;
				}
				{
			case 'N':
			case 'n':
				cout << "Cancelled!" << endl;
				break;
				}
			default:
				(cin.fail());
				cin.ignore();
				cout << "Error!" << endl;
			}
		}
		//age 21-25
		else if (age >= 21 && age <= 25) {
			cout << name << " Your age is " << age << ". Wanna go to a trip to Istanbul?" << endl;
			cout << "(y/n)" << endl;
			cin >> question;
			switch (question) {
				{
			case 'y':
			case 'Y':
				cout << "Enjoy!" << endl;
				break;
				}
				{
			case 'N':
			case 'n':
				cout << "Cancelled!" << endl;
				break;
				}
			default:
				(cin.fail());
				cin.ignore();
				cout << "Error!" << endl;
			}
		}
		//age 26-30
		else if (age >= 26 && age <= 30) {
			cout << name << " Your age is " << age << ". Wanna go to trip to Hawaii?" << endl;
			cout << "(y/n)" << endl;
			cin >> question;
			switch (question) {
				{
			case 'y':
			case 'Y':
				cout << "Enjoy!" << endl;
				break;
				}
				{
			case 'N':
			case 'n':
				cout << "Cancelled!" << endl;
				break;
				}
			default:
				(cin.fail());
				cin.ignore();
				cout << "Error!" << endl;
			}
		}
		else {
			(cin.fail());
			cin.ignore();
			cout << "Error!" << endl;
		}
	}

	return 0;
}
