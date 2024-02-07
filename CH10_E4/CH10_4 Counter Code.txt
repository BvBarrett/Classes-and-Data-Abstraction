// Counter.cpp : This file contains the 'main' function. Program execution begins and ends there.
//Brandon Barrett 

#include <iostream>
#include "Counter.h"

using namespace std;

void Counter::initializeCounter()
{
	counter = 0;
}
void Counter::setCounter(int x)
{
	if (x >= 0)
		counter = x;
	else counter = 0;
}
void Counter::incrementCounter()
{
	counter++;
}
void Counter::decrementCounter()
{
	if (counter <= 0)
		cout << "Counter cannot be negative." << endl;
	else
		counter--;
}
int Counter::getCounter() const
{
	return counter;
}
void Counter::print() const
{
	cout << "Counter = " << counter << endl;
}
Counter::Counter(int x)
{
	setCounter(x);
}
