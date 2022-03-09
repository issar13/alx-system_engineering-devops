## Shell Variables and Expansions

**Task 0:** **alias ls="rm *":** Script that creates an alias with ls and rm.

**Task 1:** **echo hello $USER:**  script that prints hello user.

**Task 2:** **export PATH=$PATH:/action:** script that adds /action to the PATH. /action/

**Task 3:** **echo $PATH| tr ":" "\n" | wc -l:** script that counts the number of directories in the PATH.

**Task 4:** **printenv:** Creates a script that lists environment variables.

**Task 5:** **set:** script that lists all local variables and environment variables, and functions.

**Task 6:** **export BEST=School:**  script that creates a local variable.

**Task 7:** **export BEST=School:** script that creates a global variable.

**Task 8:** **echo $((128 + TRUEKNOWLEDGE)):** writes the addition of 128 with trueknowledge.

**Task 9:** **echo $((POWER / DIVIDE)):** Arithemetic calculation of power by divide.

**Task 10:** **echo $((BREATH ** LOVE)):** another arithmetic calculation of the result of breath to the power of love.

**Task 11:** **echo $((2#$BINARY)):** converts number from base 2 to base 10..

**Task 12:** **printf "%s\n" {a..z}{a..z} | grep -v oo:** a script that prints all possible combinations of two letters, except oo,letters are lower cases, from a to z,one combination per line,the output should be alpha ordered, starting with aa.

**Task 13:** **printf '%.2f\n' $NUM:** script that prints a number with two decimal places, followed by a new line.

**Task 14:** **printf '%x\n' $DECIMAL:**a script that converts a number from base 10 to base 16

**Task 15:** **tr 'A-Za-z' 'N-ZA-Mn-za-m':** a script that encodes and decodes text using the rot13 encryption. Assume ASCII.

**Task 16:** **cat -n | grep [13579][[:space:]] | tr -s ' ' | cut -f2:** a script that prints every other line from the input, starting with the first line.

**Task 17:** **printf "%o\n" $((5#`echo $WATER | tr 'water' '01234'` + 5#`echo $STIR | tr 'stir.' '01234'`)) | tr '01234567' 'bestchol':** a shell script that adds the two numbers stored in the environment variables WATER and STIR and prints the result.