
<a id=top></a>

# Building a Calorie Counter

<details>
      <summary>
        <h4>Follow Links Steps</h4>
      </summary>
       
<table>
  <thead>
    <tr><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__00__title_" target="_self">Step 0</a></th><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__01__step__" target="_self">Step 1</a></th><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__02__step__" target="_self">Step 2</a></th><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__03__step__" target="_self">Step 3</a></th><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__04__step__" target="_self">Step 4</a></th><tr><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__05__step__" target="_self">Step 5</a></th><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__06__step__" target="_self">Step 6</a></th><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__07__step__" target="_self">Step 7</a></th><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__08__step__" target="_self">Step 8</a></th><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__09__step__" target="_self">Step 9</a></th><tr><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__10__step__" target="_self">Step 10</a></th><th><a href="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp//tree/main/steps/__11__step__" target="_self">Step 11</a></th></tr>
  </thead>
  <tbody>
  </tbody>
</table>
</details>


<details>
      <summary>
        <h4>Description of the Task</h4>
      </summary>
       <h3>Step  11</h3>

<section>
<p>Create another <code>div</code> element. Within it, nest a <code>button</code> to <code>submit</code> the form. This button should have the text <code>Calculate Remaining Calories</code>.</p>
<p>Then add a <code>button</code> with the <code>id</code> set to <code>clear</code> to clear the form (don't forget to give it a <code>type</code> attribute that prevents it from submitting the form). This button needs the text <code>Clear</code>.</p>
</section>
</details>

<h4>preview</h4>
    <img src="https://github.com/AndriiKot/JS__Validation_by_Building_a_Calorie_Counter__freeCodeCamp/blob/main/images/previews/preview_step11.png" alt="preview_step11">
  

[back to top](#top)


<table>
  <thead>
      <tr><th height=33 width=100>JavaScript</th><th height=33 width=100>CSS</th><th height=33 width=100>HTML5</th></tr>
  </thead>
  <tbody>
      <tr><td height=100 width=100><a href=https://ecma-international.org/publications-and-standards/standards/ target="_self"><img src=https://github.com/AndriiKot/iconsSVG_and_linksDocs/blob/main/svg/javascript-1.svg alt=JavaScript></a></td><td height=100 width=100><a href=https://www.w3.org/Style/CSS/ target="_self"><img src=https://github.com/AndriiKot/iconsSVG_and_linksDocs/blob/main/svg/css.svg alt=CSS></a></td><td height=100 width=100><a href=https://html.spec.whatwg.org/multipage/ target="_self"><img src=https://github.com/AndriiKot/iconsSVG_and_linksDocs/blob/main/svg/html.svg alt=HTML5></a></td></tr>
  </tbody>
</table>

[back to top](#top)



<details open>
  <summary>
    <h4>index.html</h4>
  </summary>



```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="styles.css" />
    <title>Calorie Counter</title>
  </head>
  <body>
    <main>
      <h1>Calorie Counter</h1>
      <div class="container">
        <form id="calorie-counter">
          <label for="budget">Budget</label>
          <input
            type="number"
            min="0"
            id="budget"
            placeholder="Daily calorie budget"
            required
          />
          <fieldset id="breakfast">
            <legend>Breakfast</legend>
            <div class="input-container"></div>
          </fieldset>
          <fieldset id="lunch">
            <legend>Lunch</legend>
            <div class="input-container"></div>
          </fieldset>
          <fieldset id="dinner">
            <legend>Dinner</legend>
            <div class="input-container"></div>
          </fieldset>
          <fieldset id="snacks">
            <legend>Snacks</legend>
            <div class="input-container"></div>
          </fieldset>
          <fieldset id="exercise">
            <legend>Exercise</legend>
            <div class="input-container"></div>
          </fieldset>
          <div class="controls">
            <span>
              <label for="entry-dropdown">Add food or exercise:</label>
              <select id="entry-dropdown" name="options">
                <option value="breakfast" selected>Breakfast</option>
                <option value="lunch">Lunch</option>
                <option value="dinner">Dinner</option>
                <option value="snacks">Snacks</option>
                <option value="exercise">Exercise</option>
              </select>
              <button type="button" id="add-entry">Add Entry</button>
            </span>
          </div>
          <div>
            <button type="submit">Calculate Remaining Calories</button>
            <button type="button" id="clear">Clear</button>
          </div>
        </form>
      </div>
    </main>
  </body>
</html>

```



[back to top](#top)


</details>

<details open>
  <summary>
    <h4>script.js</h4>
  </summary>



```js
'use strict';


```



[back to top](#top)


</details>

<details open>
  <summary>
    <h4>styles.css</h4>
  </summary>



```css
:root {
  --light-grey: #f5f6f7;
  --dark-blue: #0a0a23;
  --fcc-blue: #1b1b32;
  --light-yellow: #fecc4c;
  --dark-yellow: #feac32;
  --light-pink: #ffadad;
  --dark-red: #850000;
  --light-green: #acd157;
}

body {
  font-family: "Lato", Helvetica, Arial, sans-serif;
  font-size: 18px;
  background-color: var(--fcc-blue);
  color: var(--light-grey);
}

h1 {
  text-align: center;
}

.container {
  width: 90%;
  max-width: 680px;
}

h1,
.container,
.output {
  margin: 20px auto;
}

label,
legend {
  font-weight: bold;
}

.input-container {
  display: flex;
  flex-direction: column;
}

button {
  cursor: pointer;
  text-decoration: none;
  background-color: var(--light-yellow);
  border: 2px solid var(--dark-yellow);
}

button,
input,
select {
  min-height: 24px;
  color: var(--dark-blue);
}

fieldset,
label,
button,
input,
select {
  margin-bottom: 10px;
}

.output {
  border: 2px solid var(--light-grey);
  padding: 10px;
  text-align: center;
}

.hide {
  display: none;
}

.output span {
  font-weight: bold;
  font-size: 1.2em;
}

.surplus {
  color: var(--light-pink);
}

.deficit {
  color: var(--light-green);
}

```



[back to top](#top)


</details>