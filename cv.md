# Bondar Yaroslav

![avatar](./assets/images/avatar.png)  
### Junior Frontend Developer
---

### Contact information:
  - **E-mail:** `yarobondmail@gmail.com`<br>
  - **Telegram:** `@bonYaroslav`<br>
  - **Discord (rs-school):** `yarobond (@Yaroslav-Bondar)`<br>
  - [Linkedin](https://www.linkedin.com/in/yaroslav-bondar-7014a021b/)<br>
  - [GitHub](https://github.com/Yaroslav-Bondar)

### Profile: 

I have experience in self-development of pet projects in `JavaScript` and `React.js`. At the moment I am improving my professional skills by developing pet-projects. My peculiarity as a professional is that I like to delve into the subtleties and technical details of a programming language or any system. I see my goal as a developer in constant progress and development of my skills and knowledge. At the moment, I study web development mainly from the `front-end` side. Going forward, I see myself as a `full-stack` developer with a shift in focus towards `back-end` development. I like difficult challenges and interesting projects. Projects with a focus on performance and modern technologies. I like to be engaged in one product, make it great and be a part of a motivated, focused and professional team.

### Technical Skills:

- `Programming languages:`
  - JavaScript
- `Web fundamentals:` 
  - HTML5
  - CSS3
    - Naming classes according to the BEM methodology
  - Sass
  - Adaptive/responsive, valid, cross-browser layout
  - Pixel perfect markup
  - Figma
- `Libraries:`
  - React.js
    - Redux (react-redux)
    - React-router (react-router-dom)
- `Common front-end development tools:`
  - Git
  - Node.js
    - Npm
  - Gulp.js
  - Firefox/chrome dev tools 
- `Databases: MariaDB, MySql` 
- `Software architecture patterns:`
  - MVC
- `IDE:` 
  - Visual Studio Code, Sublime Text

### Code example:

**Which color is the brightest ?. [Kata from Codewars](https://www.codewars.com/kata/62eb800ba29959001c07dfee):**
> *One of the common ways of representing color is the RGB color model, in which the Red, Green, and Blue primary colors of light are added together in various ways to reproduce a broad array of colors. One of the ways to determine brightness of a color is to find the value V of the alternative HSV (Hue, Saturation, Value) color model. Value is defined as the largest component of a color:<br> 
`V = max(R,G,B)`<br> 
You are given a list of colors in 6-digit hexidecimal notation #RRGGBB. Return the brightest of these colors!. For example:<br> 
`brightest(["#001000", "#000000"]) == "#001000"`<br>
`brightest(["#ABCDEF", "#123456"]) == "#ABCDEF"`<br>
If there are multiple brightest colors, return the first one:<b>
`brightest(["#00FF00", "#FFFF00", "#01130F"]) == "#00FF00"`<br>
**Note that both input and output should use upper case for characters A, B, C, D, E, F.**<br>
`#Algorithms` `#Strings`* 
``` javascript
/**
 * Creates an array of elements that are the red green blue value of the RGB model
 * @param {string} hex - Color in 6-digit hexidecimal notation. For example: "#ABCDEF".
 * @returns {Array} An array of elements in hexadecimal representation 
 * that are the red green blue value of the RGB model. For example: ['AB','CD','EF'] 
 */
function splitHex (hex) {
  const step = 2
  const result = new Array()
  for (let i = 1; i < hex.length; i += step) {
    result.push(hex.substr(i, step))
  }
  return result
}
/**
 * Returns the maximum value of an array of elements that are the red green blue value of the RGB model.
 * @param {Array} rgb - An array of elements in hexadecimal representation that are the red green blue value of the RGB model. For example: ['AB','CD','EF'].
 * @returns {number} The maximum value in decimal representation 
 * of an array of elements that are the red green blue value of the RGB model in hexadecimal notation. For example: 255  
 */
function maxRgb (rgb) {
  // const intRgb = rgb.map(item => parseInt(item, 16))
  const hexRgb = rgb.map(item => '0x' + item)
  return Math.max(...hexRgb)
}
/**
 * Returns the brightest of colors.
 * @param {Array} colors - List of colors in 6-digit hexidecimal notation (["#ABCDEF", "#FFFF00"]).
 * @returns {string} The brightest color.
 */
function brightest(colors) {
  const rgb = colors.map(splitHex)
  rgb.sort((a, b) => maxRgb(b) - maxRgb(a))
  return '#' + rgb[0].join('')
}
```
### Study projects:
**English irregular verb trainer**
> Web application for better memorization of irregular English verbs. The program prompts the user to enter the correct version of one of the forms of the verb. It then validates the entered data and displays the result. It is possible to expand the list of verbs by editing the json file.

  - [View the demo](https://yaroslav-bondar.github.io/irregular-verb-trainer-MVC-/)<br>
  - [source](https://github.com/Yaroslav-Bondar/irregular-verb-trainer-MVC-)

**Responsive/adaptive layout of the online store. CSS3, Flex, Grid, Swiper Slider.**

  - [View the demo](https://yaroslav-bondar.github.io/pirosmany/)<br>
  - [source](https://github.com/Yaroslav-Bondar/pirosmany)

**Landing page adaptive layout HTML5, CSS3, SCSS, Java Script.**

  - [View the demo](https://yaroslav-bondar.github.io/X-ONE-adaptive-layout-Landing-Page-/)<br>
  - [source](https://github.com/Yaroslav-Bondar/X-ONE-adaptive-layout-Landing-Page-)

