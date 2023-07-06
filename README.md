# dacongming
小白刚开始学C用的
//用结构体编写一部电影类的信息
#include <stdio.h>
struct Movie
{
char name[20];
double price;
double start_time;
double end_time;
char position[20];
double lasting_time;
short ticket;
float version;
};
int main()
{
struct Movie M1 = { "泰坦尼克号",45.99,8.30,10.30,"第4排6座位",60.00,2};
printf("电影名字：%s", M1.name);
printf("价格:%f元\n", M1.price);
printf("开始时间：%lf\n", M1.start_time);
printf("结束时间：%lf\n", M1.end_time);
printf("座位号：%s\n", M1.position);
printf("观影时长：%lf\n", M1.lasting_time);
printf("电影票数：%d张\n", M1.ticket);
printf("电影版本：%f\n",M1.version);
M1.price = 38;
printf("打折后的价格：%lf元\n", M1.price);

return 0;
}
