# Frontend Mentor - REST Countries API with color theme switcher solution

This is a solution to the [REST Countries API with color theme switcher challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/rest-countries-api-with-color-theme-switcher-5cacc469fec04111f7b848ca). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview
This is an application project that will be fetching all world-wide's countries and display them with other information related to them. it can be a right-hand tool that can help when one needs to know informations related to a specific country. I created this app while i was learning from andela kick-start program that had equiped me with the javascript and css-grid and flex designing. 

### The challenge

Users should be able to:

- See all countries from the API on the homepage
- Search for a country using an `input` field
- Filter countries by region
- Click on a country to see more detailed information on a separate page
- Click through to the border countries on the detail page
- Toggle the color scheme between light and dark mode *(optional)*

### Screenshot

![](src\imgs\Screenshot.png)


### Links
-  [ View a Live Demo](https://jado-jeady.github.io/countriesApp/)


### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Javascript


### What I learned

during this project, i mainly learned to use event handling, consuming data from Json file and display them. i even leaned more about html DOM manipulation with Javascript. and i combined them to form a Dark/Light mode feature. as a matter of fact it is the thing that mostly challenged me but thanks to [Hemsa from Youtube](https://youtube.com) for his reference and giving me the logic behind that. 


```html
<h1>Some HTML code I'm proud of</h1>
```
```
const switchMode =  (newMode)=>{
const root = document.documentElement;
const mode = localStorage.getItem("mode");
localStorage.setItem("mode",`${newMode}`);
if(newMode=="light"){
        root.style.setProperty('--bgColor', 'hsl(0, 0%, 98%)');
        root.style.setProperty('--eltsBgColor', 'hsl(0, 0%, 100%)');
        root.style.setProperty('--color', 'hsl(200, 15%, 8%)');
        localStorage.setItem("mode",`light`);
        modeBtn.innerHTML=`
        <div id="mode-icon" data-mode="light"><span class="material-symbols-outlined">
            light_mode
            </span>
        `
    }}
```

### Useful resources

- [Free CodeCamp](https://www.freecodecamp.org/news/how-to-read-json-file-in-javascript/) - This helped me for Handling the leading Json file  . I really liked this pattern and will use it going forward.
- [Mozia Developer's event Handling reference ](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events) - This is an amazing article which helped me finally understand Event Handling in Javascript and html for web development . I'd recommend it to anyone still learning this concept.


## Author

- Website - [LetDo](https://www.your-site.com)
- Frontend Mentor - [@jado-jeady](https://www.frontendmentor.io/profile/jado-jeady)
- Twitter - [@jado](https://www.twitter.com/jado)

