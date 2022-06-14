The objective of the final project is to familiarize ourselves with steganography and how it works through designing and implementing an LSB steganography application. We’ve created an executable application with a GUI that allows you to encrypt as well as decrypt images through the actual GUI or through a command line.

User Manual
GUI:
To use GUI there are two options:
1.	Open GUI using the executable file:
Windows Environment:
	Navigate to the executable folder, Double Click stegano.exe
	Choose either the embed or detach image mode:
 
	If embed image mode is chosen:
o	Choose the Security Image (Secret Image)
o	Choose the Media Image
o	Enter the Password to use
o	Click Embed
 
o	The Embedded (Media) Image will pop up
o	Close the popped-up image, and check the output folder
o	The Embedded (Media) Image should be saved to there
	If Detach Image mode is chosen:
o	Choose the Embedded (Media) Image
o	Enter the right password
 
o	Click Detach
o	The Secret Image will pop up, if the password is incorrect nothing will be shown
o	Close the popped-up image, and check the output folder
o	The Secret Image with original filename and extension should be saved to there
Linux Environment:
	Navigate to the program folder
	Use command “wine stegano.exe”
 
	The rest will be same with the windows steps

2.	Open GUI with the source code
Any environment
	Open Command Prompt (Or terminal)
	Navigate to the source code folder using Command Prompt (Or terminal)
	Run “python gui.py” (Make sure use python here, otherwise some libraries may not load correctly)
	The rest of the steps will be same with the Open GUI using the executable file

 

 
CLI
To use CLI in any environment:
	Open Command Prompt (Or terminal)
	Navigate to the source code folder
	Check all the options with main.py -h
 
	To embed a Secret image to the Media image, use -s, -m and -p flags
Command: main.py -s < secret image> -m < media image> -p <passphrase>
 
o	The Embedded (Media) Image will pop up
o	Close the popped-up image, and check the output folder
o	The Embedded (Media) Image should be saved to there
	To detach a Secret image from the Embedded (Media) Image, use -e, -p flags
Command: main.py -e < embedded image> -p <passphrase>
 
o	The Secret Image will pop up, if the password is incorrect nothing will be shown
o	Close the popped-up image, and check the output folder
o	The Secret Image with original filename and extension should be saved to there


