Android Gesture Detector Application with SpeechToText Conversion

Android supports the Gesture API since version 1.6. The API can be located in the package android.gesture, and lets you store, load, draw and recognize gestures. 

We will present gestures: “A” to “Z”. When a corresponding gesture will be recognized, a toast message will be shown and the output of this would be given as input to SpeechToText Conversion module 

SpeechToText Conversion module Further translates the detected text to Speech

Motivation of this Android Application is to use for education purpose



Constructor of TextToSpeech class:  TextToSpeech(Context context, TextToSpeech.OnInitListener)
Methods of TextToSpeech class : 
  1) int speak (String text, int queueMode, HashMap params):
  converts the text into speech. Queue Mode may be QUEUE_ADD or QUEUE_FLUSH. 
  Request parameters can be null, KEY_PARAM_STREAM, KEY_PARAM_VALUME etc.
  
  2)int setSpeechRate(float speed):	it sets the speed for the speech.
  3)int setPitch(float speed):	it sets the pitch for the speech.
  4)int setLanguage (Locale loc):	it sets the locale specific language for the speech.
  5)void shutdown():	it releases the resource set by TextToSpeech Engine.
  6)int stop():	it interrupts the current utterance (whether played or rendered to file) and discards other utterances in the queue.

 
TextToSpeech.OnInitListener Interface:You need to implement TextToSpeech.OnInitListener interface, for performing event handling on TextToSpeech engine.

Method of TextToSpeech.OnInitListener Interface:There is only one method in this interface.
Method	Description:
void onInit (int status)	Called to signal the completion of the TextToSpeech engine initialization. T
he status can be SUCCESS or ERROR.
  
