# My_Repository
@ubuntu:~/project/test$ cat makefile 
# helloworld is a binary file
helloworld: test.o
	echo "good"
	gcc -o helloworld test.o

test.o: test.c
	gcc -c -o test.o test.c
@ubuntu:~/project/test$ cat test.c 
#include <stdio.h>

/*
 * By Vamei
 * test.c for makefile demo
 */
int main() 
{
    printf("Hello world!\n");
    printf("%s\n", __TIME__);
    printf("%s\n", __DATE__);
    return 0;
}
