# Gasoline-Project
nothing special basic c switch practice

#include <stdlib.h>
#include <stdio.h>
#include <math.h>

int main()
{
    float shell_diesel=88.2,shell_unl=92.1,petron_die=87.2,petron_unl=88.5,phoenix_die=86.8,phoenix_unl=88.2,sea_oilDie=79.9,sea_oilUnl=83.9;
    float liter,total_price;
    int gas,diesel_unleaded;

    printf("\t\t\t\tWELCOME TO GASOLINE STORE!\t\t\t\t");
    printf("\n\nPlease choose the gas that you want to purchase in our list!");
    printf("\nSHELL   [1] \nPETRON  [2] \nPHOENIX [3] \nSEA OIL [4]");
    printf("\nEnter the Gas brand you like : ");
    scanf("%d",&gas);
  
system("cls");
    switch(gas)
{
    case 1 :  system("color 6");
    printf("Prices : \nDiesel =%.1f    [1] \nUnleaded = %.1f [2] \n",shell_diesel,shell_unl);
    printf("\nChoose Whether Diesel or Unleaded : ");
    scanf("%d",&diesel_unleaded);
    printf("\nEnter How much liter: ");
    scanf("%f",&liter);
    if(diesel_unleaded == 1){
       total_price = shell_diesel * liter;
       printf("%.1f",total_price);
    }else if(diesel_unleaded == 2){
        total_price = shell_unl * liter;
        printf("%.1f",total_price);
    }else {
        printf("Please Choose from [1] & [2] only Thank you.");
    }
    break;
    case 2 : system("color 3"); 
      printf("Prices : \nDiesel =%.1f    [1] \nUnleaded = %.1f [2] \n",petron_die,petron_unl);
    printf("\nChoose Whether Diesel or Unleaded : ");
    scanf("%d",&diesel_unleaded);
    printf("\nEnter How much liter: ");
    scanf("%f",&liter);
    if(diesel_unleaded == 1){
       total_price = petron_die * liter;
       printf("%.1f",total_price);
    }else if(diesel_unleaded == 2){
        total_price = petron_unl * liter;
        printf("%.1f",total_price);
    }else {
        printf("Please Choose from [1] & [2] only Thank you.");
    }
    break;
    case 3 : system("color 5"); 
      printf("Prices : \nDiesel =%.1f    [1] \nUnleaded = %.1f [2] \n",phoenix_die,phoenix_unl);
    printf("\nChoose Whether Diesel or Unleaded : ");
    scanf("%d",&diesel_unleaded);
    printf("\nEnter How much liter: ");
    scanf("%f",&liter);
    if(diesel_unleaded == 1){
       total_price = phoenix_die * liter;
       printf("%.1f",total_price);
    }else if(diesel_unleaded == 2){
        total_price = phoenix_unl * liter;
        printf("%.1f",total_price);
    }else {
        printf("Please Choose from [1] & [2] only Thank you.");
    }
    break;
    case 4 : system("color 1"); 
      printf("Prices : \nDiesel =%.1f    [1] \nUnleaded = %.1f [2] \n",sea_oilDie,sea_oilUnl);
    printf("\nChoose Whether Diesel or Unleaded : ");
    scanf("%d",&diesel_unleaded);
    printf("\nEnter How much liter: ");
    scanf("%f",&liter);
    if(diesel_unleaded == 1){
       total_price = sea_oilDie * liter;
       printf("%.1f",total_price);
    }else if(diesel_unleaded == 2){
        total_price = sea_oilUnl * liter;
        printf("%.1f",total_price);
    }else {
        printf("Please Choose from [1] & [2] only Thank you.");
    }
    break;
    default : printf("Enter From the Choices above :D !");
    break;
}



    printf("\n\n");
    system("PAUSE");
    system("cls");
    printf("\t\tThank you For your Purchase !\t\t");
    printf("\n");

}
