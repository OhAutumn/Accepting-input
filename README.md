//Baekjoon oline 11718
//You should correct the numbers(4, 5) if you upload this code on online judge.

#include <stdio.h>

int main() {
	char input[5][5] = { 0, };
    int i;
    int n;

    for (i=0; i<5; i++)  gets(input[i]);

    for (i=4; i>=0; i--) {
        if (input[i][0] != 0) {
            n = i;
            break;
        }
    }

    for (i=0; i<n; i++) {
		puts(input[i]);
    }
    printf(input[n]);
 }

 //C언어에는 True, False가 없다. 1, 0으로 쓰면 된다.
 //gets는 엔터를 치기 전까지 입력받는다.
 //puts는 엔터를 함께 출력한다.

