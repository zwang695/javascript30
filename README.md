# 30 Day Javascript Challenge

## Day 1: Drumkit
Each keypress has a specific keycode - elements can have class data-key that represents which keypress they relate to. We can add the keydown eventListener to the window - if a key is pressed, we want to then play the audio and also play the animation. To play the audio, there are events related to audio html elements such as play. To reset the audio so we don't have to wait for the audio to end (play won't play if it is already playing the audio), we can set the currentTime of the audio to the start, 0. To play the animation, we can just change the CSS class of the respective div elements. 

## Day 2: Clock
Each hand is an element, can rotate them by changing their transform attribute - set it to rotate(degree). Get the time with Javascript's Date class, and divide by total units * 360 + 90 to get the number of degrees you are supposed to rotate. Keep in mind that the regular origin of transform is 50%, so the middle of the element, so you have to set transform-origin to 100% in order to rotate from the very right of the element. 

## Day 3: CSS Variables
Learned how to create CSS variables, and manipulate them using javascript. You can edit variables with documentElement.style.setProperty

## Day 4: Array stuff
Played around with array functions including reduce, map, sort. 

## Day 5: CSS Flexbox
Played around with flex containers and flex objects, can have flex in flex in flex.

## Day 6: Ajax Type Ahead
Here we created an app where you can filter cities by their name or by state. We had to first fetch the data from the endpoint, which returns a promise (so we have to use then keyword), and then convert the raw data into json (which also returns a promise so thus then keyword), and then push the data into a cities array (extended the json data with ... keyword). We then created a findMatches function, where we filter the cities array we created. We filter it by matching each city against a regex expression of the word currently inserted. We can then create eventlisteners on our html elements, and then turn each element of the array returned by findmatches into a span. We then replace our current suggestions with that html element we created. Key thing i learned from this is how to employ regex expressions in data manipulation with strings. 
