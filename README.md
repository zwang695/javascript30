# 30 Day Javascript Challenge

## Day 1: Drumkit
Each keypress has a specific keycode - elements can have class data-key that represents which keypress they relate to. We can add the keydown eventListener to the window - if a key is pressed, we want to then play the audio and also play the animation. To play the audio, there are events related to audio html elements such as play. To reset the audio so we don't have to wait for the audio to end (play won't play if it is already playing the audio), we can set the currentTime of the audio to the start, 0. To play the animation, we can just change the CSS class of the respective div elements. 
