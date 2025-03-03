Interactive Piano Lesson

https://github.com/Lenka-88/Project-2---Interactive-Piano-Play.git


Interactive Piano Lesson:

An interactive game with DOM events in JavaScript, which helps beginner-level piano students’ study. 

Comment: 
There is plenty of notes within the main.js JavaScript making it very clear and organized, however please see below additional thought process summarizing the completed work. 
There are no comments within HTML and CSS as the project is very simple in nature.


Explanation of the Process (main.js):


At the beginning of the code, I have variable name assignments for the keys array and the notes array. There is also a function looping through the elements of the keys array and pushing them to the notes array.
I created a function named keyPlay that changes the background color of the keys when they are pressed down. I used the .target property, because the target was modified.
Created a function named keyReturn that returns the background color of the keys to their default with an empty string '' when the mouse is released on the element. Again, I simply used the .target property.
Created an event handler that runs the keyPlay as an event handler when a mousedown event fires on any note.
Inside the function, created a second event handler property that runs the keyReturn when a mouseup event fires on any note.

At the beginning of the code, I have variable name assignments for the keys array and the empty notes array. There is also a function looping through the keys array and pushing the keys elements to the notes array to be assigned a variable name.
I created a .forEach loop that passes the elements in the notes array through your event function, so now the program knows what to do when each piano key has a mousedown or mouseup event fired on it. 
There are variables that represent the progress buttons in the song box below that allow students to progress the piano.
The nextOne, nextTwo, nextThree, and startOver change the lyrics and musical notes of the song to help the student play along.
In the beginning of the song the only button the student needs is nextOne. Because of this the .hidden properties of the other buttons are assigned the value of true.
Then I created events on all the progress buttons, by firstly creating an event handler property with a click event on the nextOne element.
To begin modifying the song box, I had to switch the progress buttons first.
Using an anonymous event handler function, I made the following changes to the button that appears after nextOne is clicked:
1.	Reveal the nextTwo button by changing the .hidden property to make the nextTwo button appear.
2.	Hide the nextOne button by changing the .hidden property to hide the nextOne button

Next, a click event firing on the nextOne changes the music notes that guide the piano student through the song.
Added the following changes to the nextOne event handler function so the musical notes change when the button is clicked.
1.	Changed the element with an ID of letter-note-five to D.
2.	Changed the element with an ID of letter-note-six to C.

Created another event handler property with a click event on the button element called nextTwo. 
Made the following changes to the button that appears when nextTwo is clicked:
1.	Reveal the nextThree button by changing the .hidden property to make the nextThree button appear.
2.	
3.	Hide the nextTwo button by changing the .hidden property to hide the nextTwo button.


13.
Once the student has reached the of the Happy Birthday song the lyrics change from HAP-PY BIRTH-DAY TO YOU to HAP-PY BIRTH-DAY DEAR FRI-END.
Following changes to the lyrics in the function when the button is clicked:
1.	Changed the content of the element with an ID of word-five to DEAR.
2.	Changed the content of the element with an ID of word-six to FRI-.

Above creates the lyrics HAP-PY BIRTH-DAY DEAR FRI-. To finish the line, you must add the -END to the song box. The -END element is stored in the lastLyric variable.
Added a statement to the event handler function for nextTwo that changes the display property of lastLyric to 'inline-block'.

A click event firing on the second button also change the music notes to guide the piano student through the song by making following changes to the nextTwo event handler function so the musical notes change when the button is clicked:
1.	Changed the content of letter-note-three to G.
2.	Changed the content of letter-note-four to E.
3.	Changed the content of letter-note-five to C.
4.	Changed the content of letter-note-six to B.

Next, I created an event handler property with a click event on the nextThree element.
By using an anonymous event handler function, I made the following changes to the button that appears when nextThree is clicked:
1.	Reveal the startOver button by changing the .hidden property to make the startOver button appear.

2.	Hide the nextThree button by changing the .hidden property to hide the nextThree button

Added the following changes to the nextThree event handler function so the lyrics change when this button is clicked.
1.	Changed the word-one to HAP-.
2.	Changed the word-two to PY.
3.	Changed the word-three to BIRTH.
4.	Changed the word-four to DAY
5.	Changed the -five to TO.
6.	Changed the word-six to YOU!.

Added the following changes to the nextThree event handler function so the musical notes change when the button is clicked.
1.	Changed the letter-note-one to F.
2.	Changed the letter-note-two to F.
3.	Changed the letter-note-three to E.
4.	Changed the letter-note-four to C.
5.	Changed the letter-note-five to D.
6.	Changed the letter-note-six to C.

Now I have the lyricsHAP-PY BIRTH-DAY TO YOU! -END! 

To finish the line, I got  rid of the “-end” in the song box by adding a statement to the event function for nextThree that changes the display property of lastLyric back to 'none'.


