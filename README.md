# uzduotis
pd3
#include <stdio.h>
#include <stdlib.h>

void ivedimas();
void kitaFig();
void patikrinimas();
int ke, ks;
int fe, fs;
int k11;
int *ptr = &k11;
int kl2;


int main()
{

    do
        ivedimas();
    while(*ptr == 2);

    do
        kitaFig();
    while (kl2 == 2);

    patikrinimas();

    return 0;
}

void ivedimas()
{
    printf("iveskite karalienes stulpelio ir eilutes kordinates\n");
    scanf("%d%d",&ke,&ks);
    if (ke>8 || ks>8)
    {
        printf("blogos kordinates\n");
        k11 = 2;
    }
    else k11 = 1;

}

void kitaFig()
{
    printf("iveskite kitos figuros stulpelio ir eilutes kordinates\n");
    scanf("%d%d",&fe,&fs);
    if (fe>8 || fs>8)

    {
        printf("blogos kordinates\n");
        kl2 = 2;
    }
    else kl2 = 1;


}

void patikrinimas()
{
    if (ke==fe || ks==fs)
    {
        printf("kertasi");
    }

    else if((fs-ks)/(fe-ke)==1 || (ks-fs)/(ke-fe)==-1)
    {
        printf("kertasi");
    }

    else printf("nesikerta");


}
