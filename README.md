# COMP-206-Assignment-1solution

Download Here: [COMP 206 Assignment 1solution](https://jarviscodinghub.com/assignment/comp-206-assignment-1solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793
Question 1: Using the Linux Terminal to Browse Animals (20 points)
The Q1 folder contains several files that we want you to examine using only the Linux terminal. You are
not supposed to use any other operating system features, especially not file browsers and windowbased editors, for this question only.
Using BASH shell commands, answer these questions about the animals in the Q1 folder and explain the
shell commands you executed to find the answer. While most questions can be answered simply by
viewing the files and computing things in your head, try to automate as much as you can: more points
for more complete automation. Write your responses in q1_written_answers.txt.
For example, the question “How many animals are there?” would be answered “8: I discovered this by
running ls *.dat | wc which counts the number of animal data files.”
a) List all the weights, in increasing order (ignore names here).
b) List all the lengths, in decreasing order (ignore names here).
c) Which is heavier, the hippo or the elephant?
d) An unfortunate fish swam into the crocodile pen, please increase its weight by 2 kg.
e) The giraffe is annoyingly tall, please remove all traces of it from our zoo.
Question 2: Sending Secret Messages (30 points)
The first “computers” were human beings with the job of
encrypting (scrambling messages to hide their contents)
and decrypting (reversing the process to read the message).
One of the simplest encryptions is called “Codebook”, and
it simply means replacing the letters of the alphabet using a
pattern that’s written down in a codebook. The Q2 folder
contains a sample codebook.txt file, shown here:
It has one line for the pattern of small letters and a second for the pattern of capitals. Each line is 26
characters long and indicates a re-mapping of each input letter based on it’s position in the standard
alphabet.
Ex1: An “a” in the input is the first letter in the alphabet, so encrypting replaces it by the first letter in
the first line of the codebook.txt file, which is “c”. While decrypting, “c” goes back to “a”.
Ex2: An “H” in the input is the 8th letter in the alphabet, so encrypting replaces it by the 8th letter in the
second line of the codebook.txt file, which is “Q”. While decrypting, “Q” goes back to “H”.
You must write two BASH programs:
a. q2_encrypt.bash: Reads the codebook file provided as its first argument, reads the original
message file provided as the second argument and prints the encrypted message on standard
output.
b. q2_decrypt.bash: Reads the codebook provided as the first argument, applies the decryption on
the encrypted file provided as the second argument and prints the recovered original message
on standard output.
Sample Program Output:
Question 3: Sorting Vacation Photos (50 points)
As Computer Science has evolved, it now covers many more useful and enlightening applications, such
as helping us view photos of cats on the Internet and organize our tourist photos. Suppose you return
from a trip having spread your images across multiple directories within the Q3 folder and you want to
re-create the timeline in chronological order.
Write a BASH program, called q3_image_sorter.bash that creates a timeline image that summarizes all
photos within the directory (and recursive sub-directories) of the first and only command-line argument.
• You can assume all input files have “.jpg” extension.
• The time-line must be sorted with the oldest on top to newest at the bottom, using the
modification date of each file (to match our example output, ensure you do not modify the
images yourself after you’ve unzipped)
• Call the Linux program “convert -append” to create the timeline image, which takes a list of N
image name arguments. The first N-1 are treated as inputs, to be read and stacked vertically in
the same order that the files are listed, and the final (Nth) argument is the output filename.
o If you do not have convert on your home system and want to develop there, you need
to install it, with a command such as “$ sudo apt-get install imagemagick”
• The time-line image must be created in the shell’s present working directory and should match
the path given as the first argument, but with “_” (underscore) characters replacing any slashes.
For example, the command “$ bash q3_image_sorter.bash Q3/SimpleTest” needs to output the
file “Q3_SimpleTest.jpg”.
• We recommend using shell command “eog” to view the files, but many other methods work
too. If you are doing your work remotely on mimi, transfer the image to yourself to view it using
scp.
