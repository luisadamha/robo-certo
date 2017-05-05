#include <stdio.h>
#include <stdlib.h>

int main()
{
    int s1, s2, s3, m1, m2;
    s1=s2=s3=m1=m2=0;
    label:{
    scanf ("%d %d %d", &s1, &s2, &s3);


    if (s1==1 && s2==1 && s3==1){
        m1=0;
        m2=0;
        printf("%d %d", m1, m2);
        printf("\n pare");
        goto label;
    }
    if (s1==1 && s2==0 && s3==1){
        m1=1;
        m2=1;
        printf("%d %d", m1, m2);
        printf("\n siga em frente");
        goto label;
    }
    if (s1==1 && s2==1 && s3==0){
        m1=1;
        m2=0;
        printf("%d %d", m1, m2);
        printf("\n vire a direita");
        goto label;
    }
    if (s1==0 && s2==1 && s3==1){
        m1=0;
        m2=1;
        printf("%d %d", m1, m2);
        printf("\n vire a esquerda");
        goto label;
    }
    if (s1==0 && s2==0 && s3==1){
        m1=1;
        m2=1;
        printf("%d %d", m1, m2);
        printf("\n siga em frente");
        goto label;
    }
    if (s1== 0 && s2==1 && s3==0){
        m1=0;
        m2=1;
        printf("%d %d", m1, m2);
        printf("\n vire a esquerda");
        goto label;
    }
    if (s1==1 & s2==0 && s3==0){
        m1=1;
        m2=1;
        printf("%d %d", m1, m2);
        printf("\n siga em frente");
        goto label;
    }
    if (s1==0 && s2==0 && s3==0){
        m1=1;
        m2=1;
        printf("%d %d", m1, m2);
        printf("\n siga em frente");
        goto label;
    }
    goto label;

    }
    return 0;
}
