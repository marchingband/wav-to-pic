# wav-to-pic

This python script can help to format a .wav file for use on a PIC MCU.
Here are the steps:

1 : open a sound file in Audacity (free software)

2 : convert the file to a single mono track

3 : export the sound, or a portion of it, using 16bit PCM .wav, and remember where you saved it

4 : open the .wav file in Sublime text editor, then <select all>, and <copy>
  
5 : paste the data into your clone of this file, save the file

6 : open a new terminal session, <cd> into the directory where you cloned this file, and launch python
  
7 : import wav2pic

8 : write this line of code into the python REPL, replacing "myfile.txt" with your own desired output file name, in quotes:
  wav2pic.convert(wav2pic.x,"my_file.txt")
  
9 : open "myfile.txt", it will be in the same directory as wav2pic.py, and copy everything

10 : paste into your c file, and use it in your PIC-based application.
