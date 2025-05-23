#include <stdio.h>
int main() {
    int choice, answer, score;

    while (1) {
        printf("\n===== QUIZ GAME MENU =====\n");
        printf("1. Start Quiz\n");
        printf("2. Exit\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);

        if (choice == 1) {
            score = 0;

            // Question 1
            printf("\nQ1. What is the capital of France?\n");
            printf("1. Rome\n2. Madrid\n3. Paris\n4. Berlin\n");
            printf("Your answer: ");
            scanf("%d", &answer);
            if (answer == 3) {
                score++;
            }

            // Question 2
            printf("\nQ2. Who wrote 'Romeo and Juliet'?\n");
            printf("1. Charles Dickens\n2. William Shakespeare\n3. Mark Twain\n4. Jane Austen\n");
            printf("Your answer: ");
            scanf("%d", &answer);
            if (answer == 2) {
                score++;
            }

            // Question 3
            printf("\nQ3. Which planet is known as the Red Planet?\n");
            printf("1. Venus\n2. Saturn\n3. Mars\n4. Jupiter\n");
            printf("Your answer: ");
            scanf("%d", &answer);
            if (answer == 3) {
                score++;
            }

            // Question 4
            printf("\nQ4. What is the square root of 64?\n");
            printf("1. 6\n2. 8\n3. 7\n4. 9\n");
            printf("Your answer: ");
            scanf("%d", &answer);
            if (answer == 2) {
                score++;
            }

            // Question 5
            printf("\nQ5. In which year did the Titanic sink?\n");
            printf("1. 1912\n2. 1920\n3. 1905\n4. 1915\n");
            printf("Your answer: ");
            scanf("%d", &answer);
            if (answer == 1) {
                score++;
            }

            // Display score
            printf("\n===== QUIZ COMPLETE =====\n");
            printf("Your score: %d out of 5\n", score);

            if (score == 5) {
                printf("Excellent work!\n");
            } else if (score >= 3) {
                printf("Good job!\n");
            } else {
                printf("Better luck next time.\n");
            }

        } else if (choice == 2) {
            printf("Thanks for playing!\n");
            break;
        } else {
            printf("Invalid choice. Try again.\n");
        }
    }

    return 0;
}
