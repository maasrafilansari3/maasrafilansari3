#include<stdio.h>
int count_bjp;
int count_tmc;
int count_cong;
int count_cpm;
int count_isf;

int main(){
    int i=0,choise2;
    char choise1;
    while (i<1)
    {   
        printf("\npress 'E' for voting\npress 'R' for result if voting is complete\n");
        scanf("%c",&choise1);
        switch (choise1)
        {
            case 'e':
                printf("\nwelcome to voteing\n\n");
                printf("press '1' to vote for BJP\npress '2' to vote for TMC\npress '3' to vote for CONG\npress '4' to vote for CPIM\npress '5' to vote for ISF\npress '6' if voteing is complete\n");
                scanf("%d",&choise2);
                switch(choise2){
                    case 1:
                        printf("you vote for BJP\n");
                        count_bjp++;
                        break;
                    case 2:
                        printf("you vote for TMC\n");
                        count_tmc++;
                        break;
                    case 3:
                        printf("you vote for CONG\n");
                        count_cong++;
                        break;
                    case 4:
                        printf("you vote for CPIM\n");
                        count_cpm++;
                        break;
                    case 5:
                        printf("you vote for ISF\n");
                        count_isf++;
                        break;
                    default:
                        printf("your choise is incorrect\n");
                        break;
                }
                break;
            case 'r':
                printf("\nthe total vote of BJP is %d \n",count_bjp);
                printf("the total vote of TMC is %d \n",count_tmc);
                printf("the total vote of CONG is %d \n",count_cong);
                printf("the total vote of CPIM is %d \n",count_cpm);
                printf("the total vote of ISF is %d \n",count_isf);
                i=1;
                break;
            default:
                break;
        }
    }
    return 0;
}
