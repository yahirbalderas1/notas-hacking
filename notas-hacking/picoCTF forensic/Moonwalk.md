## Objetivo
Decode this [message](https://jupiter.challenges.picoctf.org/static/14393e18d98fedbaedbc28896d7ef31a/message.wav) from the moon
## Solucion
Paso 1: Buscar un decodificador sstv para el archivo e instalamos
Paso 2: Decodificar
┌──(kali㉿kali)-[~/Downloads]
└─$ sstv -d message.wav -o flag.jpg           
[sstv] Searching for calibration header... Found!    
[sstv] Detected SSTV mode Scottie 1
[sstv] Decoding image...                                                                [####################################################################################################] 100%
[sstv] Drawing image data...
[sstv] ...Done!
                    

## Notas adicionales

## Referencias