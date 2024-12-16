# Frontend Mentor - Newsletter sign-up form with success message solution

This is a solution to the [Newsletter sign-up form with success message challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/newsletter-signup-form-with-success-message-3FC1AZbNrv). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- Add their email and submit the form
- See a success message with their email after successfully submitting the form
- See form validation messages if:
  - The field is left empty
  - The email address is not formatted correctly
- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![alt text](<Screenshot (55).png>)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Mobile-first workflow
- Vanilla javascript

### What I learned

I learnt that it's not all about learning the theories of designing a web app. A lot of practice is needed to fully accumulate the design practices. I made a single-page website with the styling and functionality all in a page, even the success is in same page. The code may not look clean but everything works the way they should and i'm satisfied with my work.
Below are some pieces of code that I want to highlight.

```html
<span id="error"></span> <span id="mess"></span>.
```

```css
#submit:focus {
  background-image: linear-gradient(
    to right,
    rgb(255, 129, 121),
    rgba(255, 98, 87, 0.678)
  );

  box-shadow: 0px 10px 50px rgb(255, 98, 87);
}
input:focus {
  outline: none;
  font-family: inherit;
  color: inherit;
}
```

```js
var img = document.querySelector(".illustration");
form.addEventListener("submit", (e) => {
  e.preventDefault();
  validate();
});
const errmsg = (message) => {
  err.innerText = message;
  email.style.borderColor = "rgb(255, 48, 35)";
  email.style.color = "red";
  email.style.backgroundColor = "rgb(255, 200, 200)";
};
const validate = () => {
  var mail = email.value.trim();
  if (mail) {
    success.style.display = "block";
    main.style.display = "none";
    span.textContent = mail;
  } else {
    errmsg("Input Email");
  }
};
```

### Continued development

I have mastered the grid system and from there want to move to javascript frameworks. I'm familiar with some frameworks like jQuery, react js but haven't really used any in projects. Hopefully in future challenges I'll use other frameworks.

## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@AdeniyiAbdulsa3](https://www.twitter.com/AdeniyiAbdulsa3)
- GitHub - [Abdul-ade](https://github.com/Abdul-ade)
