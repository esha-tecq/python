from gtts import gTTS
import gtts
v=gtts.lang.tts_langs()
for i,j in v.items():
 print(i,j)
 import os
 def text_to_speech(txt,lang):
 obj=gTTS(text=txt,lang=lang)
 obj.save("file1.mp3")
 os.system("file1.mp3")
"""
Press 1: To convert text into speech
Press 0: Exit
"""
while True:
 choice=input("Enter your choice: ")
 if choice=='1':
    text_to_speech(input("Enter your text: "),input("Enter Language: "))
 elif choice=='0':
  break
 else:
  print("Invalid choice")
