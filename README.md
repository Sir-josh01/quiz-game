# Quiz Game
This project is an interactive Quiz Application designed to test user knowledge on a specific topic (or a range of topics). Built with Vanilla JavaScript, HTML, and CSS, it manages the complete quiz lifecycle, including question presentation, answer validation, score tracking, and immediate feedback. It demonstrates key front-end skills in event handling and dynamic state management without relying on external libraries.
## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

Self-generating educational questions that shows you when you're right and when you're wrong.
It is repeated when the questions are exhausted.
Built with HTML, CSS and Vanilla JavaScript.

### The challenge

-Getting the app to indicate correct and wrong answers.
-Exploring the question banks to appear after compiled.

### Screenshot

![](./Screenshots/Screenshot%20(206).png)
![](./Screenshots/Screenshot%20(207).png)
![](./Screenshots/Screenshot%20(208).png)
![](./Screenshots/Screenshot%20(209).png)

### Links

- Solution URL: [@GitHub](https://github.com/Sir-josh01/quiz-game)
- Live Site URL: [@](https://)

## My process
- Structure with HTML.
- Designs and layout by CSS. 
- Handles the functionality and display with vanilla Javascript only.

### Built with
- Semantic HTML5 markup
- CSS custom properties
- Javascript for interactivity

### What I learned

```html
 <div id="question">Questions</div>
      <div id="answer-buttons" class="btn-grid">
         <button class="btn">Answer 1</button>
         <button class="btn">Answer 2</button>
         <button class="btn">Answer 3</button>
         <button class="btn">Answer 4</button>
      </div>
```

```css
*, ::after, ::before {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  font-size: 1rem;
}

:root {
  --hue-neutral: 200;
  --hue-wrong: 0;
  --hue-correct: 145;
}

```

```js
function selectAnswer(e) { 
  const selectedButton = e.target
  const correct = selectedButton.dataset.correct
  setStatusClass(document.body, correct)
  Array.from(answerButtonsElement.children).forEach(button => {
    setStatusClass(button, button.dataset.correct)
  })

  const questions = [{
  question: 'what is 2 + 2?',
  answers: [
    { text: '4', correct: true },
    { text: '22', correct: false }
  ]
},
```

### Continued development

-To add an API and integrate the application to generate question from an extertal source
-Make the questio dynamic and more educational and inspiring.
-Add a button which will end and exit application
-Store the score and display to users.  

### Useful resources

- [google.com](https://www.google.com) - Acquired some resources from stackoverflow.
- [w3school.com](https://www.w3school) - An amazing site which helped with giving understanding deeper concepts.


## Author

- Website - [@myPorfolio](https://my-portfolio-f43qpo3lz-sir-josh01-projects.vercel.app/)
- Frontend Mentor - [@sir_josh01](https://www.frontendmentor.io/profile/sir_josh01)
- Twitter - [@sir_josh01](https://www.twitter.com/Sir_josh01)
- LinkedIn - [@sir_josh01](https://www.linkedin.com/in/sir-josh01)

