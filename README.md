#include "stdafx.h"
#include "stdio.h"
#include "stdlib.h"
#include "time.h"

int main ()
{
     int tal = 0;
     int antal_variabler;
     int nytt_tal;
     
     srand((unsigned)time(NULL));
     nytt_tal = rand() % 100 + 1;
     printf("Datorn tänker på ett tal mellan 1 och 100. Varsågod att gissa:");
     antal_variabler = scanf_s("%d", &tal);
     getchar(); //töm radslutet efter scanf
     if (tal == nytt_tal)
          printf("Talet är för stort.");
     else if (tal > nytt_tal)
          printf("Talet är för stort.");
     else printf("Talet är för litet.");
     getchar(); /* utan denna rad hoppar programmet ur consolefönstret när du kör
                   programmet, och du hinner inte se resultatet */
     return 0;
}     
