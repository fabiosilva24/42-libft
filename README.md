# Libft - My C Library Implementation

*Recreating essential C standard library functions from scratch*

## 🎯 About

Libft is my implementation of basic C library functions as part of the 42 school curriculum. This project taught me fundamental programming concepts and low-level memory management while building a personal library for future projects.

**Note**: This is educational work completed independently following 42 coding standards.

## 🧠 What I Learned

- **Memory Management**: malloc, free, and preventing memory leaks
- **Pointer Manipulation**: Understanding how pointers work and move through memory
- **String Processing**: How strings are stored and manipulated at the byte level
- **Low-level Programming**: Working directly with memory and file descriptors
- **Data Structures**: Building and managing linked lists
- **Error Handling**: Protecting against NULL pointers and edge cases

## 📂 Functions Implemented

### Standard Library Functions (libc)

**Character Functions:**
- `ft_isalpha`, `ft_isdigit`, `ft_isalnum`, `ft_isascii`, `ft_isprint`
- `ft_toupper`, `ft_tolower`

**String Functions:**
- `ft_strlen`, `ft_strchr`, `ft_strrchr`, `ft_strncmp`
- `ft_strlcpy`, `ft_strlcat`, `ft_strnstr`, `ft_strdup`

**Memory Functions:**  
- `ft_memset`, `ft_bzero`, `ft_memcpy`, `ft_memmove`
- `ft_memchr`, `ft_memcmp`, `ft_calloc`

**Conversion:**
- `ft_atoi` - string to integer

### Additional Functions

**String Creation:**
- `ft_substr`, `ft_strjoin`, `ft_strtrim`, `ft_split`
- `ft_itoa` - integer to string
- `ft_strmapi`, `ft_striteri`

**File Output:**
- `ft_putchar_fd`, `ft_putstr_fd`, `ft_putendl_fd`, `ft_putnbr_fd`

### Bonus: Linked Lists
- `ft_lstnew`, `ft_lstadd_front`, `ft_lstadd_back`
- `ft_lstsize`, `ft_lstlast`, `ft_lstdelone`, `ft_lstclear`
- `ft_lstiter`, `ft_lstmap`

## ⚙️ Compilation

```bash
make        # Create libft.a
make bonus  # Include bonus functions
make clean  # Remove object files
make fclean # Remove all compiled files
make re     # Recompile everything
```

## 🚀 Usage

```c
#include "libft.h"

int main(void)
{
    char *str = ft_strdup("Hello 42!");
    if (str)
    {
        ft_putendl_fd(str, 1);
        free(str);
    }
    return (0);
}
```

## 💡 Key Challenges

- **ft_split**: Parsing strings and managing memory for arrays
- **Linked Lists**: Understanding pointer to pointer concepts
- **Memory Management**: Preventing leaks and handling edge cases
- **ft_itoa**: Converting numbers to strings efficiently

## � Skills Gained

- Low-level C programming
- Manual memory management  
- Understanding of how standard library works
- Debugging with valgrind and gdb
- Following strict coding standards (42 Norm)

---

*This library serves as the foundation for all future 42 projects.*
