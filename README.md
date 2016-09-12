# rfpwnon v-0.7
<br>
Most update to date code available from: http://exploit.agency/sploit/rfpwnon<br>
Demo at: https://www.legacysecuritygroup.com/index.php/categories/13-sdr/22-rfpwnon-py-the-ultimate-rfcat-ask-ook-brute-force-tool<br>
<br>
<pre>
python rfpwnon.py --help
usage: rfpwnon.py [-h] [-v] [-f BASEFREQ] [-b BAUDRATE] [-l BINLENGTH]
                  [-r REPEATTIMES] [--keys] [-p PPAD] [-t TPAD] [--raw]
                  [--tri]

Application to use a rfcat compatible device to brute force a particular AM
OOK or raw binary signal.

optional arguments:
  -h, --help      show this help message and exit
  -v, --version   show program's version number and exit
  -f BASEFREQ     Specify the target frequency to transmit on, default is
                  915000000.)
  -b BAUDRATE     Specify the baudrate of the signal, default is 2000.
  -l BINLENGTH    Specify the binary length of the signal to brute force. By
                  default this is the binary length before pwm encoding. When
                  the flag --raw is set this is the binary length of the pwm
                  encoded signal.
  -r REPEATTIMES  Specify the number of times to repeat the signal. By default
                  this is set to 1 and uses the de bruijn sequence for speed.
                  When set greater than one the script sends each possible
                  permutation of the signal individually and takes much longer
                  to complete. For some applications the signal is required to
                  be sent multiple times.
  --keys          Displays the values being transmitted in binary, hex, and
                  decimal both before and after pwm encoding.
  -p PPAD         Specify your own binary padding to be attached before the
                  brute forced binary.
  -t TPAD         Specify your own binary padding to be attached after the
                  brute forced binary.
  --raw           This flag disables the script from performing the pwm
                  encoding of the binary signal. When set you must specify the
                  full pwm encoded binary length using -l.
  --tri           This flag sets up the script to brute force a trinary
                  signal.

</pre>
