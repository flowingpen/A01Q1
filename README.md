A01Q1
=====
#include <stdio.h>
#include <stdlib.h>
struct node 
{
int data;
struct node *next;
};
struct node *start=NULL, *current, *newnode;
void main()
{
int n;
do
{
struct node *newnode=(struct node *)malloc(sizeof(struct node));
printf("enter the data to be entered");
scanf("%d",&newnode->data);
if(start==NULL)
{
start=newnode;
current=newnode;
}
else
{
current->next=newnode;
current=newnode;
}
printf("do you want to add another");
ch=getchar();
}
while(ch!='n');
getnode(&head,3);
getch();
}
void getnode(struct node *head, int index)
{
temp=head;
int count=0;
while(temp)
{
if(index==count)
printf("%d",temp->data);
temp=temp->next;
count++;
}
}
