#include<iostream>
#include<conio.h>
class complex {
private:
	int R1;
	int R2;
	int I1;
	int I2;
public:
	void set(int, int, int, int);
	void addition();
	void subtraction();
	void print();
};
using namespace std;
void main()
{
	int r1, r2, i1, i2;
	complex c;
	cout << "Eneter the first Real number";
	cin >> r1;
	cout << "Enter the 1st imaginary number";
	cin >> i1;
	cout << "Enter the 2nd Real number";
	cin >> r2;
	cout << "Enter the 2nd imaginary number";
	cin >> i2;
	c.set(r1, r2, i1, i2);
	c.addition();
	c.subtraction();
	_getch();
}
void complex::set(int r1, int r2, int i1, int i2) {
	R1 = r1;
	R2 = r2;
	I1 = i1;
	I2 = i2;
}
void complex::addition() {
	cout << "Addition of Complex Numbers" << endl;
	cout << "The complex number is after addition is given as (" << R1 + R2 << "," << I1 + I2 << ")" << endl;
}
void complex::subtraction() {
	cout << "Subtraction of Complex Numbers" << endl;
	cout << "The complex number is after subtraction is given as (" << R1 - R2 << "," << I1 - I2 << ")" << endl;
}
void complex::print() {
	cout << "The two numbers you have given are as under :" << endl;
	cout << "(" << R1 << "," << I1 << ")" << endl;
	cout << "(" << R2 << "," << I2 << ")" << endl;
}
