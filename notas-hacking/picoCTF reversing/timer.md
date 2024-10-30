# Solucion

```
┌──(kali㉿kali)-[~/Documents/picoCTF/reversing/timer]
└─$ ls
AndroidManifest.xml  classes2.dex  classes3.dex  classes.dex  kotlin  META-INF  res  resources.arsc  timer.apk
                                                                                                                                                              
┌──(kali㉿kali)-[~/Documents/picoCTF/reversing/timer]
└─$ strings classes3.dex | grep pico       
*picoCTF{t1m3r_r3v3rs3d_succ355fully_17496}

```