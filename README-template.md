# Frontend Mentor - Base Apparel coming soon page solution

This is a solution to the [Base Apparel coming soon page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/base-apparel-coming-soon-page-5d46b47f8db8a7063f9331a0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview
This is one of the best intresting challange where I implemented JavaScript which helped to validate the form email element. Plus designing the layout of the website with the Basic of CSS FlexBox.

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page
- Receive an error message when the `form` is submitted if:
  - The `input` field is empty
  - The email address is not formatted correctly

### Screenshot

![](./screenshot.jpg)

![image](https://user-images.githubusercontent.com/42742924/126803527-26dc1c1b-9a47-46b3-8208-d5351cc527df.png)
![image](https://user-images.githubusercontent.com/42742924/126804120-f5475d7e-67e0-4870-be70-114128d03df7.png)


### Links

- Solution URL: [Add solution URL here](https://github.com/Skyz03/Base-coming-soon)
- Live Site URL: [Add live site URL here](https://github.com/Skyz03/Base-coming-soon)

## My process
The process includes, implementation of design using CSS FlexBox for the layout plus later the input element was implemented with basic ```input validation of type = Email```. After that JS file was added where form validation was implemented which is available in W3 school. 


### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- JS From Validation

### What I learned

There are many things I leanred which is the understading of Client-side form validation where, understood the basic of input validation or Custom validation which is implemented using JS and its custom functions. Also, implementing things in ```ID``` rather than ```CLASS``` is a better option when in DOM elements.  
```html
<input class="email-entry" type="email" name="mail" id="mail" placeholder="Email Address" required
            minlength="8">
```
```css
#errorImg {
  content: "";
  background: url(images/icon-error.svg) no-repeat;
  position: absolute;
  z-index: 2;
  top: 0.7rem;
  height: 100%;
  width: 100%;
  left: 17rem;
  visibility: hidden;
}
}
```
```js
cfunction showError() {
  if (email.validity.valueMissing) {
    // If the field is empty,
    // display the following error message.
    emailError.textContent = 'You need to enter an e-mail address.';
    emailImg.style.visibility = "visible"
  } else if (email.validity.typeMismatch) {
    // If the field doesn't contain an email address,
    // display the following error message.
    emailError.textContent = 'Entered value needs to be an e-mail address.';
    emailImg.style.visibility = "visible"
  } else if (email.validity.tooShort) {
    // If the data is too short,
    // display the following error message.
    emailError.textContent = `Email should be at least ${email.minLength} characters; you entered ${email.value.length}.`;
    emailImg.style.visibility = "visible"
  }
}
```

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
