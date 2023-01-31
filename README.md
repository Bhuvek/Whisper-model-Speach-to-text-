# Whisper-model-Speach-to-text-
Audio Processing : This model is used to convert any Speach into text into few line of code 

To use this model :

Step 1: You have to instal lib:
! pip install git+https://github.com/openai/whisper.git -q

Step 2:LOAD THE LIB

import whisper 
model = whisper.load_model('medium')  #769M para/record

!wget -O audio.mp3 

Step 3:

from IPython.display import Audio, display

display(Audio('//content//Hope(PaglaSongs) (2).mp3', autoplay=True))

Step 4:

result = model.transcribe("//content//Hope(PaglaSongs) (2).mp3")
print(result["text"])


For Simple use :

import whisper
model = whisper.load_model('medium')
model.transcribe("audio.mp3")['text']

