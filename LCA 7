#include <stdio.h>

void swapSpeeds(int *motor1, int *motor2)
{
    int temp = *motor1;
    *motor1 = *motor2;
    *motor2 = temp;
}

int main(void)
{
    int speed1, speed2;

    printf("Enter the speeds of Motor 1 and Motor 2: ");
    if (scanf("%d %d", &speed1, &speed2) != 2) {
        printf("Please enter two integer speeds.\n");
        return 1;
    }

    int originalSpeed1 = speed1;
    int originalSpeed2 = speed2;

    printf("\nBefore swapping\n");
    printf("Motor 1 speed: %d, Address: %p\n", speed1, (void *)&speed1);
    printf("Motor 2 speed: %d, Address: %p\n", speed2, (void *)&speed2);

    swapSpeeds(&speed1, &speed2);

    printf("\nAfter swapping\n");
    printf("Motor 1 speed: %d, Address: %p\n", speed1, (void *)&speed1);
    printf("Motor 2 speed: %d, Address: %p\n", speed2, (void *)&speed2);

    if (speed1 == originalSpeed2 && speed2 == originalSpeed1) {
        printf("\nSwap verified successfully.\n");
    } else {
        printf("\nSwap verification failed.\n");
    }

    return 0;
}
