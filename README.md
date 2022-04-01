# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Emily Yao**

Time spent: 6 hours spent in total

Link to project: https://glitch.com/edit/#!/moored-ambiguous-flamingo

## Required Functionality

The following **required** functionality is complete:

* [X] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [X] "Start" button toggles between "Start" and "Stop" when clicked. 
* [X] Game buttons each light up and play a sound when clicked. 
* [X] Computer plays back sequence of clues including sound and visual cue for each button
* [X] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [X] User wins the game after guessing a complete pattern
* [X] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [X] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [X] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [X] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [X] Game will keep increasing the sequence pattern until the player fails (technically caps at 100)
- [X] Game keeps track of player's highest number of correct guesses

## Video Walkthrough (GIF)

When choosing an incorrect button:
![](https://i.imgur.com/tVlkx3i.gif)

After completing a full sequence (demo stops after 5 but full game continues for 100 clues):
![](https://i.imgur.com/fWgSnIM.gif)


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
None really. All the resources provided in this handy manual was all I needed. I especially liked the additional relevant reading while following this guide. I learned a lot of CSS tricks that I hadn't known before. 

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
In my first test run of this game, I was consistently failing at the third guess. It seemed very strange to me, and I had a gut feeling that this wasn't because of my wrong input. The first two guesses were both the blue button, and I could pass the first two guesses with no issue, so I had a hunch the defect lied in the third button, which was the yellow button. Even though I was sure I was pressing the yellow button on my third guess, the game would give me the lose message. I was so thankful that the code came with console messages to debug, because when I immediately checked the console log, it said that the game was registering button 4 as button 1 instead. This led me to check my html tags on button 4. What was even stranger was that "onlick = "guess(4)"" was properly implemented. In the end, it was a matter of letting Glitch completely upload my changes to the code. So what I did was just retype the onlick tag for button 4 so that Glitch could recognize my change and reflect on the page. Maybe what had happened was that I forgot to move my cursor onto a different line after wiring the yellow button to guess(4). After making this adjustment, I could pass the game in its entirety.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
I now sort of understand the basic frameworks that go into creating a webpage. Now I'm wondering how I can customize these web elements using my own graphics. All of the button, dropdown, and etc. elements have a default appearance. I understand you can use CSS to change certain characterstics of the buttons but what if I wanted a button of a non polygonal shape? How do I add dynamic animations to a webpage? Would it also involve Javascript? Are there other tools on the Internet that make web development more user friendly like Glitch?

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
Since I love playing rhythm games, I had an idea where I could take this light and sound memory game and add a time component to it. Basically, not only would the player have to match the order of the sounds, they'd also have to match the duration that each pitch is played for. This would involve adding a rhythm pattern for the clue sequence. This feature would also require a protocol for determining if the player pressed a button for the exact length of time. Of course, you'd need to be superhuman to count by milliseconds so for this game pressing the button within a reasonable range around the desired duration would suffice. I'd also take the time to wire the button up to key presses instead of just mouse clicks. Maybe the player can play using the arrow keys or the number keys.



## Interview Recording URL Link

[My 5-minute Interview Recording](https://ucla.zoom.us/rec/play/5pLai9bHMWpGDS91G2sDrWxZELQa7n-EvM0yj6UBuMD_oiF-XsAorOCw9IFlkgKmBd7RJb9D_cXanlSm.Wuvfj02rnn-MQ0qC (Passcode: h#bCe@q6))
(Passcode: h#bCe@q6)


## License

    Copyright Emily Yao

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.