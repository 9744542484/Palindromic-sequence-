//# Palindromic-sequence-
#include <stdio.h>

int main() {

    int n, originalNum, reversedNum = 0, remainder;

    printf("Enter an integer: ");

    scanf("%d", &n);

    originalNum = n;

    // reverse the number

    while (n != 0) {

        remainder = n % 10;

        reversedNum = reversedNum * 10 + remainder;

        n /= 10;

    }

    // check if the reversed number is equal to the original number

    if (originalNum == reversedNum)

        printf("%d is a palindrome.", originalNum);

    else

        printf("%d is not a palindrome.", originalNum);

    return 0;

}

