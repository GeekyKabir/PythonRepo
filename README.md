# EasyAcces- A program which can use to access programs easily.

import pyttsx3
import os

print("\nWelcome to EasyAccess.")
pyttsx3.speak("Welcome to EasyAccess.")
print("\nType 'help' or '?' for help (without inverted commas/quotations).")
pyttsx3.speak("\nType your choice of program.")
print()

while True:
	print("Type your choice of program:" , end='') #Here we can also use p = input("Type your choice of program:")
	p = input()
	if (("run" in p) or ("execute" in p) or ("open" in p)) and (("cmd" in p) or ("command prompt" in p) or ("terminal" in p)):
		os.system("start cmd") #Here I used 'start' with 'cmd' because it open the new window of cmd prompt. If I use only 'cmd' it opens the command prompt in the same terminal on the new line.
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and (("powershell" in p) or ("windows powershell" in p)):
		os.system("start powershell") #Here it is same as cmd. 'start' keyword used to open another window.
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and (("chrome" in p) or ("google chrome" in p) or ("google" in p)) :
		os.system("chrome")
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and (("notepad" in p) or ("editor" in p)):
		os.system("notepad")
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and (("player" in p) or ("media player" in p) or ("windows media player" in p)):
		os.system("wmplayer")
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and (("vlc" in p) or ("vlc player" in p) or ("vlc media player" in p)):
		os.system("vlc")	
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and (("firefox" in p) or ("firefox browser" in p) or ("mozilla" in p)):
		os.system("firefox https://google.com")	#Here we can give link of the website with browser to access the given URL directly.
	elif (("run" in p) or ("execute" in p) or ("open" in p) or ("show" in p)) and ("time" in p) :
		os.system("time /t")
	elif (("run" in p) or ("execute" in p) or ("open" in p) or ("show" in p)) and  ("date" in p):
		os.system("date /t")
	elif (("date & time" in p) or ("time & date" in p)):
		os.system("time /t & date /t")
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and ("calendar" in p):
		os.system("start outlookcal:")
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and ("calculator" in p):
		os.system("start calculator:")	
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and (("clock" in p) or ("alarm" in p)):
		os.system("start ms-clock:")	
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and ("camera" in p):
		os.system("start microsoft.windows.camera:")
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and (("wifi" in p) or ("available networks" in p)):
		os.system("start ms-availablenetworks:")	
	elif (("run" in p) or ("execute" in p) or ("open" in p)) and (("file explorer" in p) or ("file manager" in p) or ("this pc") or ("explorer")):
		os.system("explorer")
	elif (("help" in p) or ("?" in p)):
		print("\nThis program supports to easily open -\n 1.Command Prompt\n 2.PowerShell\n 3.Chrome\n 4.Notepad\n 5.Windows Media Player\n 6.VLC Media Player\n 7.Firefox\n 8.Time\n 9.Date\n 10.Calendar\n 11.Calculator\n 12.Alarm\n 13.Camera\n 14.Available Networks\n 15.File Explorer\n")
		print("\nType 'q', 'exit' or 'quit' to close EasyAccess.")
		print("\nNote: Use words like 'run', 'execute' or 'open' with the above mentioned program name. Only in small letters.")
		print("\nThis program is created by Mohammad_Kabir Sheikh.\n Contact: kabirsheikh30@gmail.com\n")
	elif (("exit" in p) or ("quit" in p) or ("q" in p)):
		break		
	else:
		print("Input keywords not supported. Type 'help' or '?' for help.")	
	
