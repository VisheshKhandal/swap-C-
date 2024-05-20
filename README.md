# swap-C-
swaping two numbers :  : : : : :

#include<stdio.h>
void wrong_swap(int a,int b);
void swap(int *a,int *b);

int main() {
    int x = 3,y =4;
    printf("the value of x,y befoe swap IS %d and %d\n",x,y );
    // wrong_swap(x,y); TODO: THIS IS NOT WORK due to CALL BY VALUE ;
    swap(&x,&y);
    printf("the value of x,y after swap id %d and %d\n",x,y );  
    return 0;
}
void wrong_swap(int a,int b) {
    int temp;
    temp = a;
    a = b;
    b = temp;
}
void swap(int *a,int *b) {
    int temp;
    temp = *a; //FIXME: THE MEANING OF *a and *b IS DENOTED THE ACTUAL VALUES OF  A AND B 
    *a = *b;
    *b = temp;
}    

    
     

