#include <stdio.h>
#include <stdlib.h>

int main(){
int array[50];
int i,j,k,temp;
        for(j=0; j<50; j++){
        array[j]=rand()%50+1;
        }
        for(k=0; k<50; k++){
        printf("%d ",array[k]);}
        printf("\n\n");

        for(j=0;j<50;j++){
        for(i=1; i<49; i++){
            if(array[i-1]>array[i]){
              temp=array[i];
            array[i]=array[i-1];
            array[i-1]=temp;}}}

         for(j=0; j<50; j++){
        printf("%d ",array[j]);}


    return 0;
}
