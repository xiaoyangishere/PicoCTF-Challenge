# Python Wrangling
# Description
Python scripts are invoked kind of like programs in the Terminal... Can you run this [Python script](https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/ende.py) using this [password](https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/pw.txt) to get the [flag](https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/flag.txt.en)?

# Solution
1. Open webshell terminal
2. Enter these in the Terminal prompt: $ wget https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/ende.py
                                       && wget https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/pw.txt
                                       && wget https://mercury.picoctf.net/static/8e33ede04d02f3765b8c6a6e24d72733/flag.txt.en
3. Enter $ cat ende.py to read the python scripts
4. Enter $ cat pw.txt to read the passwd
4. Inside the python script, we could see that it builds with a file called "pole.txt". It supports two arguments (-e/-d)
5. Since we need to decrypt it, use -d 
6. Enter $ python3 ende.py -d pole.txt
7. Enter the passwd found in pw.txt

# Flag
picoCTF{4p0110_1n_7h3_h0us3_aa821c16}
   
