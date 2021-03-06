# JSON

Guide for custom questions and the related JSON.  

Start:

```json
{"response_code":0,"results":
  [
```

Then follow up with this statement for each question:

```json
{"category":"MyCategory","type":"boolean","difficulty":"mydifficulty","question":"Example Question","correct_answer":"TrueOrFalse","incorrect_answers":["mybooleanvalue"]},
```

Add one of those for each question you want.  
Note you need to switch out the following values:
> `category` - put in the category of the question (Example: `"History"`).
> `type` - type must be the string `boolean` or the quiz site will not render the question. **REQUIRED**  
> `difficulty` - the difficulty of the question (Example: `"easy"`)  
> `question` - the question to ask the user (Example: `"Why are donuts so tasty?"`) **REQUIRED**  
> `correct_answer` - boolean of which answer correct (Example: `"True"` or `"False"`) **REQUIRED**  
> `incorrect_answers` - array of boolean values (array must *only have a single value*) (Example: `["True"]`)  

Ending of JSON file:

```json
 ]
}
```

Thanks for reading!  
