#include <stdio.h>
#include <time.h>
#include <stdlib.h>
#include <ctype.h>

typedef struct {
    
        int day;
        int month;
        int year;
        
        
}  Date;
int main()
{
    
   Date LPM;
   Date Today; 
   
   int day_diff, mon_diff, year_diff;
   int GE;
   int DUEday, DUEmonth, DUEyear;
   
     /*First date given by the user of the LMP */
   printf("Introduce the date of your first day of the Last Menstrual Period (LMP) in this format dd mm yyyy. \n");
    int check = scanf("%d %d %d",&LPM.day,&LPM.month,&LPM.year);
    
    
    /*Validation of the date given for LPM*/ 
    if (check != 3){
        printf("Please enter only numbers, signs and letters aren´t need.\n\n");
        return 0;
    }else if (LPM.month > 12 || LPM.day > 31){
        printf("Make sure the day and month are in the range.\n\n");
        exit (0);
        
    }
    /*Second date given*/ 
    printf("Introduce the current date in this format dd mm yyyy. \n");
    int checar= scanf ("%d %d %d",&Today.day,&Today.month,&Today.year);
     
     /*Validation of the date given for current day*/ 
    if (checar != 3){
        printf("Please enter only numbers, signs and letters aren´t need.\n\n");
        return 0;
    }else if (LPM.month > 12 || LPM.day > 31){
        printf("Make sure the day and month are in the range.\n\n");
        exit(0);
        
    }
    /*Second date (current date) function */
    time_t date = time(0);
        struct tm *tlocal = localtime(&date);
        char output[128];
        strftime(output,128,"%d %m %Y",tlocal);
        printf("%s\n\n",output);
        
    if (Today.day < LPM.day)
    {
        if (Today.month == 3)
        {
             /* In here it check if the year is a leap year */ 
             if ((Today.year % 4 == 0 && Today.year % 100 != 0) || (Today.year % 400 == 0))
             {
                Today.day += 29;
             }
             else 
             {
                 Today.day +=28;
             }
        }
        /* Days of the month from May, July, October, December */ 
        else if (Today.month == 5 || Today.month == 7 || Today.month == 10 || Today.month == 12)
        {
            Today.day +=30;
        }
        /* Days from January, March, June, November */
        else
        {
            Today.day += 31;
        }
        Today.month = Today.month - 1;
    }
    if (Today.month < LPM.month)
    {
        Today.month += 12;
        Today.year -= 1;
    }
        day_diff = Today.day - LPM.day;
        mon_diff = Today.month - LPM.month;
        year_diff = Today.year - LPM.year;
        
        
        printf("Time difference from Last Menstrual Period (LPM) to today: %d years, %02d months and %02d days.\n\n", year_diff, mon_diff, day_diff);
        
    /*Gestational Age */
      GE = (mon_diff *4);
       if (GE > 3) 
      {
         GE++;
      }
        printf("Gestational Age: %d weeks\n\n", GE);  
        
    /*Due Date*/
    DUEday = (LPM.day + 7);
    DUEmonth = (LPM.month +9);
     if (DUEmonth > 12)
     {
         LPM.year +=1;
     }
     DUEyear = LPM.year; 
     
     printf("Due Date: %d %d %d\n\n", DUEday, DUEmonth, DUEyear);
    
           
     
     return 0;
}


