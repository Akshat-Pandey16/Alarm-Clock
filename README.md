# Alarm-Clock
An alarm clock is a reminder to start working on our dream by waking up from our dreams.
#python code
from datetime import datetime   
from playsound import playsound
import time
inputtime = int(input("Enter the time of alarm to be set:HH:MM:SS\n"))
now = datetime.now()

justtime=int(now.strftime("%H%M"))

print("Setting up alarm..")
while True:
    justtime=int(now.strftime("%H%M"))
    if(inputtime==justtime):
        print("Wake Up!")
        playsound('song.mp3')
        time.sleep(2)
        break
