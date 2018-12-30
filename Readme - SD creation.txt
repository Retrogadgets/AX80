To create the AX81 file system on SD card

The programs reside in a 132 MBytes image file, which must start within the first 60 MB of the SD card. 
Each tape has a unique identifier in it, which is used to determine the beginning of the image file when the system starts up. 
A program consists of a header block (512 bytes) and the data block of 16 KBytes. 
In the header block are the program name (10 characters in the ZX81 character set) and then 2 bytes file length For the sake of clarity,
32 files each are combined with one tape. In the ZX81 you can then use POKE 99, x Command can be toggled between each tapes. 
By calculation, a maximum of 8192 files can be stored on an SD card and occupy about 132 MByte there. SDHC cards are also supported. 
In addition, there are 256 subfolders that represent the tapes and over which the "data exchange" takes place with the image file. 

1 Initialize the file system
For this, the SD card should be freshly formatted. First the installer is copied to the SD card. 
Then simply at the command prompt type install_fs.exe and creation of the image will be started. Then it takes up to 5 minutes for the file system to be created. 
In addition to the image file there is a subfolder TAPES in which the directories for the individual tapes are located. 
After installation, the installation program should be deleted again, as an accidental call creates a new, empty image file and deletes existing data there. 

2 Write files to SD card
The program 000_write_to_tape.exe writes all .P files located in the current directory to the free spaces of the corresponding subdirectory tapes. 
If the available space is insufficient, a corresponding error message will be displayed. Before writing, the tape is formatted (all programs deleted in it). 
The three zeros before the file name of the programs / scripts should ensure that they are always at the top of the directory. 

3 Read files from SD card
The program 000_read_from_tape.exe reads all the existing programs in the subdirectory. 
Existing programs will be overwritten without notice. 
