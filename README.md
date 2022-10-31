#define _CRT_SECURE_NO_WARNINGS  1
#include <iostream>
#include <math.h>
#include <limits.h>
using namespace std;

int main()
{
	char arr[100] = { 0 };
	int i = 0;int n, m, a = 0;
	while ( arr[i]=getchar())
	{
		if (arr[i] == '\n')
		{
			break;
		}
		i++;
	}
	int count = 0;
	a = i;
	for (n = 65;n < 91; n++)
	{
		for (m = 0; m < a; m++)
		{
			if (arr[m] == (char)n)
			{
				count++;
			}
		}
		if (count > 0)
		{
			cout << (char)n << count << endl;
		}
		count = 0;
	}
	
	return 0;
}
