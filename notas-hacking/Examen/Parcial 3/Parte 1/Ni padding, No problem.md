
# Solucion

```
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial3/no_padding]
└─$ nc mercury.picoctf.net 33780
Welcome to the Padding Oracle Challenge
This oracle will take anything you give it and decrypt using RSA. It will not accept the ciphertext with the secret message... Good Luck!


n: 136908661492147564613293130741847553156140070014620222301286105586284998816167411625693302179324093185112690944957590306387216183246225066322947664249467778259494681038977563430173657334419528564514452102222559244296061765965422102756187099431736994090270316312884387188317593486527210175922259951933433188567
e: 65537
ciphertext: 68543208789124397119341321824688985467748253032373963540673496869883177984443048689004055147135275657100631348851415925448375577094389414462251043290369799111026699824358801414392612224354569597987407046151491396592070528553976417650089210886603879243505588374903023163315804750717126586413346461301080758880


Give me ciphertext to decrypt: ^C
                                                                                                                                                              
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial3/no_padding]
└─$ nano solve.py               
                                                                                                                                                              
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial3/no_padding]
└─$ python3 solve.py 
[+] Opening connection to mercury.picoctf.net on port 33780: Done
/home/kali/Documents/picoCTF/parcial3/no_padding/solve.py:17: BytesWarning: Text is not bytes; assuming ASCII, no guarantees. See https://docs.pwntools.com/#bytes
  r.sendlineafter(b'Give me ciphertext to decrypt: ', str(payload))
Doubled Plain: 580550060391700078946913236734911770139931497702556153513487440893406629034802718534645538074938502890768709712035489670906
Plain Text Hex: 7069636f4354467b6d347962335f54683073655f6d337335346733735f3472335f646966757272656e745f303830313937337d
Plain Text: picoCTF{m4yb3_Th0se_m3s54g3s_4r3_difurrent_0801973}
[*] Closed connection to mercury.picoctf.net port 33780

```