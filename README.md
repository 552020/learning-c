# C

## ft_putchar

ft_putchar.c

```c
#include<unistd.h>

void ft_putchar(char c)
{

    write(1, &c, 1);
}

int main(void)
{
	ft_putchar('m');
};
```

ft_putchar.b

## ft_print_alphabet

Create a function that displays the alphabet in lowercase, on a single line, by ascending order, starting from the letter 'a'.

The only allowed function is _write_.

```c
#include <unistd.h>

void ft_putchar(char c) {

    write(STDOUT_FILENO, &c, 1);

    }

void ft_print_alphabet(void) {
  char letter;

  letter = 'a';
  while (letter <= 'z') {
    ft_putchar(letter);
    letter++;
  }
}

int main(void) {
  ft_print_alphabet();
  return 0;
}
```

https://stackoverflow.com/questions/51426227/displaying-characters-in-ascending-order-in-c

## Varia

### Header

To insert the header open a file in VIM and press F1.

## Command line arguments in C/C++

_argc_ (argument count) is an integer that indicates how many arguments were entered on the command line when the program was started.
_argv_ (argument vector) is an array of pointers to arrays of character objects.

https://stackoverflow.com/questions/3024197/what-does-int-argc-char-argv-mean

https://www.geeksforgeeks.org/command-line-arguments-in-c-cpp/
