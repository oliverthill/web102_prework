# WEB102 Prework - *Sea Monster Website*

Submitted by: **Oliver Toshiki Hill**

**Sea Monster Website** is a website for the company Sea Monster Crowdfunding that displays information about the games they have funded.

Time spent: **10** hours spent in total

## Required Features

The following **required** functionality is completed:

* [ ] The introduction section explains the background of the company and how many games remain unfunded.
* [ ] The Stats section includes information about the total contributions and dollars raised as well as the top two most funded games.
* [ ] The Our Games section initially displays all games funded by Sea Monster Crowdfunding
* [ ] The Our Games section has three buttons that allow the user to display only unfunded games, only funded games, or all games.

The following **optional** features are implemented:

* [ ] The header includes a button that scrolls to the "Our Games" section.
* [ ] The website's visual appeal has been improved through custom edits in the html and CSS files.

## Video Walkthrough

Here's a walkthrough of implemented features:

![web102_prework](https://github.com/oliverthill/web102_prework/blob/main/web102_walkthrough.gif?raw=true)

GIF created with LICEcap

## Notes

Describe any challenges encountered while building the app:


Problem 1: Lack of familiarity with html and CSS functionality specifically in JavaScript.

I once consulted with a student who was struggling academically to capture requirements for a personalized tracking tool. Based on those needs, I used Java with Selenium to automate interaction with the school portal by inspecting the portal’s DOM in Chrome DevTools. I identified anchor names and file paths, then leveraged CSS and XPath selectors to programmatically extract assignment grades and due dates. While this provided great experience necessary for completing this project, I lack experience with using Javascript specifically. While concepts were familiar, specifics of syntax were not, and methods such as filter() and reduce() were new to me.

Solution: Extensive research through the materials provided and independent resouces.


Problem 2: Finding the variable to be passed to addGamesToPage.

I was originally unable to differentiate between GAMES_JSON and gamesContainer, misunderstanding the key difference in their data structures and how they were formed. I thought that gamesContainer itself was a JavaScript array of objects, and did not properly think about the statement:

    const gamesContainer = document.getElementById("games-container");

When reading over this statement again, it can of course be seen that this searches for an element in the html file, meaning that it is an html element and not an array. I overlooked this because it was already provided in the skeleton, but I should have thoroughly scanned all of the given code before moving onto my own implementation.

Solution: Walking through the code step-by-step, and understanding what every object and variable's function is within the code.


Problem 3: Various syntax errors, leading to errors in button functionality.

While there were many small cases of syntax errors that I quickly caught, the most notable example was in challenge 6, where my string that explained the number of unfunded games using the ternary operator was not being displayed correctly. I unfortunately spent over 45 minutes trying to debug this one issue only to find that this declaration:

    numOfUnfunded = listOfUnfundedGames.length;

had failed to have been assigned a data type.

Solution: I eventually began to research general debugging methods that could be used for WebDev, and came across the console.log() method. I then inserted in my code: console.log(numOfUnfunded); right after the parsing of the string, and looked at the result in the console tab in Chrome DevTools. I found the error: "Uncaught ReferenceError: numOfUnfunded is not defined" which eventally led me to realize that the underlying issue was the numOfUnfunded variable itself.


Problem 4: The scroll button, and making other general CSS edits

In the selenium webscraper program I developed for my client, I was much less concerned with CSS formatting which led me to have less experience with it. Additionally, I had a lot of trouble developing the method for scrolling to a desired section on the web page when assigned to an event listener for a button.

Solution: Extensive research through the materials provided and independent resouces.


## License

    Copyright [2025] [Oliver Toshiki Hill]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
