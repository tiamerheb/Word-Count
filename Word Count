#include <stdio.h>
int main(int argc, char *argv[])
{
        FILE * stdin;
        char currentLetter;
        int charCount = 0;
        int wordCount = 0;
        int lineCount = 0;
        int count = 1;
        int a_word = 0;
        FILE * file = fopen(argv[count], "r");
             
        while((currentLetter = fgetc(file)) != EOF)
        {
                if (isspace(currentLetter))
                {
                        if (a_word == 1)
                        {
                                wordCount++;
                                a_word = 0;
                        }
                }
                else
                {
                        a_word = 1;
                }
                if (currentLetter == '\n')
                {
                        lineCount++;
                }
                charCount++;
        }
        printf("%d lines \n", lineCount);
        printf("%d characters \n", charCount);
        printf("%d words \n", wordCount);
}
