---
layout: single
title: "조건문"
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"
---
### 01. 사주보기
![saju](/assets/images/if1.jpg)
~~~c
#include <stdio.h>
int main() {
  int year, month, day;
  int rmd;
printf("enter the year, month and day you were born: ");
  scanf("%d%d%d", &year, &month, &day);
  rmd=(year-month+day)%10;
    if(rmd==0)
  printf("AWESOME LUCK");
  else
  printf("SOSO LUCK");
    return 0;
}
~~~
---
### 02. 3개의 터널 통과
![tunnel](/assets/images/if2.jpg)

~~~c
#include <stdio.h>
int main() {
   int h=170;
  int h1, h2, h3;
  printf("enter the height of 3 tunnels: ");
  scanf("%d%d%d", &h1, &h2, &h3);  
  if((h<h1) && (h<h2) && (h<h3))
        printf("successful");
  else
    printf("unsuccessful");
  
    return 0;
}
~~~
---
### 03. 이 달은 며칠까지 있을까?
![calenderl](/assets/images/if3.jpg)
~~~c
#include <stdio.h>
int main(void)
{ int year, month;
printf("연도와 월을 입력하세요 : ");
scanf("%d%d", &year, &month);
printf("%d년 %d월의 마지막날은 ", year, month);
if(month==1||month==3||month==5||month==7||month==8||month==10||month==12)
printf("31일");
else if(month==4||month==6||month==9||month==11)
printf("30일");
else
{if((year%4==0 && year%100!=0) || year%400==0)
printf("29일");
else
printf("28일");}
printf("입니다.\n");
return 0;}
~~~
