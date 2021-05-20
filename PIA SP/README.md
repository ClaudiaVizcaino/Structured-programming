# Final Project (PIA): "Gestational Age and Due-Date Calculator"



**Program:** https://www.onlinegdb.com/lsAVn0XYK

**Video:** https://youtu.be/MI7qVzZl3FI

## Objective
- The main objective of this PIA is to calculate the Gestational Age and Estimate Due Date (EDD) for any pregnancy, the gestational age would give the weeks of the pregnancy and the EDD would give the date of the expected deliver day.

## Program  
- This program gives a proper control of the prenatal care for any person, it is more focus on the pregnant woman because it ask the Last Menstrual Period (LMP) which is a date usually known by the women or doctor. 
- The program fulfill the objective and also gives the user the time difference between the two dates.

## Information needed
- The program would ask the last menstrual period (LMP) date. 

## Code 
- The code works with the LPM date and the current date, it uses Naegele's rule that it is based on a normal 28-day menstrual cycle, for obtain the gestational age in which the pregnant is.
1. The code starts by validating the two dates (LMP and the current date) it makes a difference between them counting the leap years and different total days of every month. 
1. After obtaining the difference (of the years, months, and days) it starts calculating the Gestational Age which is given by the following rule:
**EG=(N° Months x 4)+(1 week every 3 months)**
1. Finally, the code obtain the Due-Date with the Naegele's rule, the code verify the month if it is higher than 12 and the day if it is higher than 31.
**Due-Date=LPM-3 Months+1 week**
## Auto-evaluation 
 1.  Complejidad: 2
 2. Funcionalidad: 2
 3.  Código: 3 
 4. Almacenaje: 1 
 5. Documentación: 2
**CF** = 10
##  References
1. Calculating a Due Date. Johns Hopkins Medicine. (n.d.). https://www.hopkinsmedicine.org/health/wellness-and-prevention/calculating-a-due-date. 
1. Gestational Age. (n.d.). https://manual.jointcommission.org/releases/TJC2016B1/DataElem0265.html#:~:text=Gestational%20age%20(written%20with%20both,Obstetricians%20and%20Gynecologists%20reVITALize%20Initiative). 
