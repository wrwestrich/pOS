# CSC4100

Programming Assignment #1-2 for CSC4100

## OS design

I made this OS using the FAT12 file system. The boot loader uses this file system to load the second stage of the OS, which is written in C/protected mode. The OS implements a very simple IDT to use the keyboard inpterrupt to record input for the login screen. The IDT is very unfinished, but I had many issue getting it to work properly is the first place, so I had to cut corners. The login screen checks only the password and checks against "password." The keyboard only supports lowercase letters, numbers, and various symbols.

I've tested the login screen with various inputs. Any input that's not a letter or number will cause it password to be incorrect, as it puts that character into the input buffer.

In conclusion, it is very watered down, it's rough, and it desperately needs improving, but it gets the job done. Scheduling, more interrupts, and cleaner code would be the first things on the list of improvements.
