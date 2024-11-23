```
#include <stdio.h>

int main(void)

{
  int local_10;
  int local_c;
  
  local_c = 0x1e0da;
  for (local_10 = 0; local_10 < 0x25f; local_10 = local_10 + 1) {
    local_c = local_c + local_10;
  }
  printf("%i", local_c);
}
```

```
┌──(kali㉿kali)-[~/picoCTFretos/e3/GDB2]
└─$ gcc sol.c -o sol
                                              
┌──(kali㉿kali)-[~/picoCTFretos/e3/GDB2]
└─$ ls
debugger0_b  sol  sol.c
                                              
┌──(kali㉿kali)-[~/picoCTFretos/e3/GDB2]
└─$ ./sol  
307019 
```
