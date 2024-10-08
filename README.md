<h1 align="center">STOP WATCH</h1>

<p align="center">
  <img src="https://github.com/BhavdeepSinghNijhawan/Stop-Watch/assets/143419096/3fe6f522-bdb6-4650-846d-3554b92cc9a6" />
</p>

A stopwatch is a handheld timekeeping device used to measure the amount of time elapsed between a starting point and an ending point. It typically features a set of buttons for starting, stopping, and resetting the timer. Stopwatches are commonly used in various activities where precise timing is important, such as sports, science experiments, and other time-sensitive applications.

## LIVE URL

https://bhavdeepsinghnijhawan.github.io/Stop-Watch/

## TECHNOLOGY STACK

### HTML

```
<!DOCTYPE html>
```
- **Document Type Declaration:** This line declares the **document type** and **version of HTML** being used. **1<!DOCTYPE html>`** specifies that this is an **HTML5** document.
```
<html lang="en">
```
- **HTML Element:** This is the root element of the HTML document. The **`lang="en"`** attribute specifies that the language of the document is English.
```
<head>
```
- **Head Element:** This section contains **meta-information** about the document such as its **title**, **character set**, **styles**, and **scripts** that should be loaded.
```
<meta charset="UTF-8">
```
- **Meta Character Set:** This specifies the **character encoding** for the HTML document. **`UTF-8`** is a standard character encoding capable of encoding all possible characters.
```
<meta http-equiv="X-UA-Compatible" content="IE=edge">
```
- **Meta Compatibility:** This tag ensures that the document is displayed in the **highest mode available** in Internet Explorer.
```
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
- **Viewport Meta Tag:** This controls the viewport's size and scale, ensuring that the web page is responsive and properly scaled on different devices. **`width=device-width`** sets the width to be equal to the width of the device screen. **`initial-scale=1.0`** sets the initial zoom level when the page is first loaded by the browser.
```
<title>Stop Watch</title>
```
- **Title Element:** This sets the title of the web page, which is displayed in the browser's title bar or tab.
```
<link rel="stylesheet" href="style.css">
```
- **Link Element:** This links an external CSS file **`(style.css)`** to the HTML document. This file contains the styles for the web page.
```
</head>
```
- **End of Head Element**
```
<body>
```
- **Body Element:** This section contains the content of the HTML document that is visible to users.
```
<div class="container">
```
- **Div Element:** This creates a division or a container on the web page. The **`class="container"`** attribute assigns a class name **`"container"`** to this div, which can be used for CSS styling.
```
<h1>Bhavdeep Singh Nijhawan<br> 
    Stop Watch</h1>
```
- **Heading Element:** This defines a **top-level heading (H1)** for the web page. It displays the text "Bhavdeep Singh Nijhawan" followed by a line break **`(<br>)`** and then "Stop Watch".
```
<div id="time">
```
- **Div Element:** This creates another division with the **`id "time"`**, which will be used to display the stopwatch time.
```
<span class="digit" id="hr">00</span> 
<span class="txt">Hr</span> 
<span class="digit" id="min">00</span> 
<span class="txt">Min</span> 
<span class="digit" id="sec">00</span> 
<span class="txt">Sec</span> 
<span class="digit" id="count">00</span>
```
- **Span Elements:** These elements display the digits and labels for the stopwatch.
  - **`<span class="digit" id="hr">00</span>:`** Displays hours with the id "hr" and class "digit".
  - **`<span class="txt">Hr</span>:`** Displays the label "Hr".
  - **`<span class="digit" id="min">00</span>:`** Displays minutes with the id "min" and class "digit".
  - **`<span class="txt">Min</span>:`** Displays the label "Min".
  - **`<span class="digit" id="sec">00</span>:`** Displays seconds with the id "sec" and class "digit".
  - **`<span class="txt">Sec</span>:`** Displays the label "Sec".
  - **`<span class="digit" id="count">00</span>:`** Displays the count (likely hundredths of a second) with the id "count" and class "digit".
```
</div>
```
- **End of Div Element (time)**
```
<div id="buttons">
```
- **Button Elements:** These create three buttons with the class "btn" and respective ids "start", "stop", and "reset". The text inside the buttons ("Start", "Stop", "Reset") indicates their functionality.
```
<button class="btn" id="start">Start</button> 
<button class="btn" id="stop">Stop</button> 
<button class="btn" id="reset">Reset</button>
```
- **Button Elements:** These create three buttons with the class "btn" and respective ids "start", "stop", and "reset". The text inside the buttons ("Start", "Stop", "Reset") indicates their functionality.
```
    </div>
</div>
```
- **End of Div Elements (buttons and container)**
```
<script src="script.js"></script>
```
- **Script Element:** This includes an external JavaScript file (script.js) which will contain the logic for the stopwatch.
```
</body>
</html>
```
- **End of Body and HTML Elements:** This marks the end of the body and the entire HTML document.

### CSS

```
body { 
    padding: 0; 
    margin: 0; 
    font-family: verdana; 
} 
```
- Removes all padding and margin from the body.

```
.container { 
    display: flex; 
    flex-direction: column; 
    justify-content: center; 
    align-items: center; 
    width: 100%; 
    height: 100vh; 
    background-color: rgb(0, 0, 0); 
} 
```
- Uses Flexbox to center the content both vertically and horizontally.
- Sets the width to 100% and height to 100vh (viewport height).
- Sets the background color to black.
```
h1 { 
    color: rgb(255, 115, 0); 
    text-align: center; 
} 
```
- Sets the color of the heading to a bright orange.
- Centers the text.
```
.digit { 
    font-size: 150px; 
    color: #fff; 
} 
```
- Sets the font size for the digits to be very large (150px).
- Sets the color to white.
```
.txt { 
    font-size: 30px; 
    color: #fffcd6; 
} 
```
- Sets the font size for the text to 30px.
- Uses a light yellow color.
```
#buttons { 
    margin-top: 50px; 
} 
```

- Adds a margin at the top of the buttons container.

```
.btn { 
    width: 100px; 
    padding: 10px 15px; 
    margin: 0px 20px; 
    border-top-right-radius: 10px; 
    border-bottom-left-radius: 10px; 
    border-bottom-right-radius: 4px; 
    border-top-left-radius: 4px; 
    cursor: pointer; 
    font-size: 20px; 
    transition: 0.5s; 
    color: white; 
    font-weight: 500; 
} 
```

- Sets the **width**, **padding**, and **margin** for the buttons.
- Adds **various border-radius values** for rounded corners.
- Changes the cursor to a pointer when hovering over the button.
- Sets the **font size**, **transition time**, **text color**, and **font weight**.

```
#start { 
    background-color: rgb(255, 115, 0); 
} 
```

- Sets the background color for the start button to bright orange.

```
#stop { 
    background-color: rgb(255, 115, 0); 
} 
```

- Sets the background color for the stop button to bright orange.

```
#reset { 
    background-color: rgb(255, 115, 0); 
} 
```

- Sets the background color for the reset button to bright orange.

### JavaScript

```
let startBtn = document.getElementById('start'); 
let stopBtn = document.getElementById('stop'); 
let resetBtn = document.getElementById('reset'); 

let hour = 0; 
let minute = 0; 
let second = 0; 
let count = 0; 
```

- Retrieves the start, stop, and reset buttons from the HTML.
- Initializes variables for hours, minutes, seconds, and count to 0.

```
startBtn.addEventListener('click', function () { 
    timer = true; 
    stopWatch(); 
}); 

stopBtn.addEventListener('click', function () { 
    timer = false; 
}); 

resetBtn.addEventListener('click', function () { 
    timer = false; 
    hour = 0; 
    minute = 0; 
    second = 0; 
    count = 0; 
    document.getElementById('hr').innerHTML = "00"; 
    document.getElementById('min').innerHTML = "00"; 
    document.getElementById('sec').innerHTML = "00"; 
    document.getElementById('count').innerHTML = "00"; 
}); 
```

- Adds click event listeners to the **start**, **stop**, and **reset** buttons.
- The **start button **sets timer to true** and **calls the stopWatch function**.
- The **stop button sets timer to false**.
- The **reset button sets timer to false** and **resets the time variables** and **the displayed time**.

```
function stopWatch() { 
    if (timer) { 
        count++; 

        if (count == 100) { 
            second++; 
            count = 0; 
        } 

        if (second == 60) { 
            minute++; 
            second = 0; 
        } 

        if (minute == 60) { 
            hour++; 
            minute = 0; 
            second = 0; 
        } 

        let hrString = hour; 
        let minString = minute; 
        let secString = second; 
        let countString = count; 

        if (hour < 10) { 
            hrString = "0" + hrString; 
        } 

        if (minute < 10) { 
            minString = "0" + minString; 
        } 

        if (second < 10) { 
            secString = "0" + secString; 
        } 

        if (count < 10) { 
            countString = "0" + countString; 
        } 

        document.getElementById('hr').innerHTML = hrString; 
        document.getElementById('min').innerHTML = minString; 
        document.getElementById('sec').innerHTML = secString; 
        document.getElementById('count').innerHTML = countString; 
        setTimeout(stopWatch, 10); 
    } 
}
```
- Defines the stopWatch function that runs the stopwatch logic.
- If timer is true, increments the count.
- When count reaches 100, increments second and resets count to 0.
- When second reaches 60, increments minute and resets second to 0.
- When minute reaches 60, increments hour and resets minute and second to 0.
- Formats the time values to ensure two-digit display.
- Updates the HTML elements with the current time values.
- Calls the stopWatch function again after 10 milliseconds using **`setTimeout`**.

## CONTRIBUTOR

- [Bhavdeep Singh Nijhawan](https://www.linkedin.com/in/bhavdeep-singh-nijhawan-739634280)
