# C-Programs
#include <stdio.h>
#include <time.h>
#include <unistd.h>
#include <stdlib.h>
#include <conio.h>
int main()
{
	int hour,minute,second;
	hour=minute=second=0;
	while(1)
	{
		
		printf("%2d:%2d:%2d",hour,minute,second);
		
		second++;
		if(second==60)
		{
			minute+=1;
			second=0;
		}
			
			if(minute==60)
			{
			hour+=1;
			minute=0;
			}
			
			if(hour==24)
			{
				hour=0;
				minute=0;
				second=0;
			}
			sleep(1);
			clrscr();
		}	//	while close
				return 0;
}	//min close
