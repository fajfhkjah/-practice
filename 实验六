#include <stdio.h>

struct Country
{
	char name[100];
	int jp;
	int yp;
	int tp;
	int zj;
};

typedef struct Country Country;

void sort(Country a[],int n)
{
	for(int i=0;i<n-1;i++)
	{
		for(int j=0;j<n-1;j++)
		{
			if(a[j].jp<a[j+1].jp)
			{
				Country temp=a[j];
				a[j]=a[j+1];
				a[j+1]=temp;
			}
		}
	}
}

int main()
{
	Country c[8];
	FILE* fp=fopen("D:\\text.txt","r");
	int i;
	for(i=0;i<8;i++)
	{
		fscanf(fp,"%s %d %d %d %d",c[i].name,&c[i].jp,&c[i].yp,&c[i].tp,&c[i].zj);
	}
	fclose(fp);
	sort(c,8);
	FILE* outfp=fopen("D:\\newnew.txt","w");
	for(i=0;i<8;i++)
	{
		fprintf(fp,"%s\t%d\t%d\t%d\t%d\n",c[i].name,c[i].jp,c[i].yp,c[i].tp,c[i].zj);
	}
	fclose(outfp);
	return 0;
}
