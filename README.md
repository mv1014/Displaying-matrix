//DISPLAYING A MATRIX TAKEN FROM THE USER
#include<stdio.h>
#include<string.h>
int main(){
    
    int i,j,r,c;
    printf("Write the number of rows : \n");
    scanf("%d",&r);
    printf("Write the number of columns : \n");
    scanf("%d",&c);
    int a[r][c];
    printf("Write the numbers of the matrix : \n");
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            printf("Enter the values for a[%d][%d] : \n",i+1,j+1);
            scanf("%d",&a[i][j]);
        }
        if(j==c){
            printf("\n");
        }
    }
    printf("The matrix entered by the user is : \n");
    for(i=0;i<r;i++){
        for(j=0;j<c;j++){
            printf("%d ", a[i][j]);
        }
        printf("\n");
    }
    return 0;
}

