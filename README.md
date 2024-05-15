# FOR-CHILDREN-PINO
![Screenshot 2024-05-15 193622](https://github.com/Jatin9826/FOR-CHILDREN-PINO/assets/167497208/d885db0d-db6b-4a1c-a874-0b12fd42b08a)

I MADE THIS PROJECT AS A FUN USING HTML , CSS , JAVA-SCRIPT (PINO)

"Ever dreamed of becoming a maestro without the hassle of learning to play an actual instrument? Introducing the 'Click-to-Play Piano' – your virtual gateway to musical stardom with just a click! Simply tap your way to harmonic bliss as each key unleashes a symphony of sound. Whether you're a virtuoso or just here to tickle the ivories for fun, this interactive piano will have you feeling like Beethoven in no time. Warning: Side effects may include uncontrollable toe-tapping and spontaneous outbreaks of joyous laughter!"



1. **Select DOM Elements**: Use `document.querySelectorAll()` to select all elements with the class "key" and store them in the variable `keys`. Similarly, select elements with classes "key.white" and "key.black" and store them in variables `whiteKeys` and `blackKeys`, respectively.

2. **Attach Event Listeners**: Iterate over each element in `keys` using `forEach()` and attach a click event listener to each one, calling the `handleKeyClick()` function when clicked.

3. **Handle Key Click**: Define the `handleKeyClick()` function, which is called when a key is clicked. It passes the clicked key element (`this`) to the `playKey()` function.

4. **Play Key Function**: Define the `playKey()` function, which takes a key element as a parameter.

5. **Retrieve Audio Element**: Use the `dataset.note` attribute of the key element to get the ID of the corresponding audio element and store it in the variable `keyAudio`.

6. **Reset Audio**: Set the `currentTime` property of `keyAudio` to 0, ensuring that the audio starts from the beginning each time it's played.

7. **Play Audio**: Call the `play()` method on `keyAudio` to play the associated audio file.

8. **Add Active Class**: Add the "active" class to the clicked key element, visually indicating that it's being played.

9. **Remove Active Class on Audio End**: Add an event listener to `keyAudio` for the "ended" event. When the audio ends, remove the "active" class from the key element.

10. **Function End**: Logic execution completes.
