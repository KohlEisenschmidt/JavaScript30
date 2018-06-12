this file was a test experiment in note takeing


http://keycode.info/   is a little website that shows the keyCode of a key when pressed 

data attribute 
data-key is not standard. In this example the data-key="65" is used like a class to link the audio attribute to the div attribute 
 <div data-key="65" class="key">
      <kbd>A</kbd>
      <span class="sound">clap</span>
    </div>

and

  <audio data-key="65" src="sounds/clap.wav"></audio>

----------------------

 we want to listen to the keydown event and when this happens we are going 
 to run this function (e) ((the event))

(in the script tag)
 window.addEventListener('keydown', function (e) {
   console.log(e);
 
 when we run this event and press say A we will see in the console the keyboard event and then its object 
 with all its information. 
 if we clicked "A" and open the console and open the object we will see the keyCode for A to be 65. 

 (now if we change the script to find the keyCode)
 window.addEventListener('keydown', function (e) {
   console.log(e.keyCode);
   Now when we press a key, only the keyCode will be displayed in the console. 
