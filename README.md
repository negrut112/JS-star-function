# JS-star-function
<p>A function that generate a perfect 5 corner star.</p>
<p>You can check the live preview on: <a href="https://negrut112.github.io/JS-star-function/">https://negrut112.github.io/JS-star-function/</a><br>
<img src="https://i.imgur.com/zOl3RMl.jpg"><br>
<b>HTML</b>
<p>I have used the HTML to define the area where I’m working defining the height, width and the border style:</p>
<p>&lt;canvas id=“myCanvas” height=“310” width=“500” style=“border: 1px solid black”&gt;&lt;/canvas&gt;</p>
<b>JavaScript</b>
<p>To make the star I used 3 parameters, two for starting point - left corner and one for side length.<br>
I had troubles to determine the other angles coordinate so I used math formulas whereas sinus and cosinus.</p>
<p>Example:</p>
<p>function filledStar(x,y,a){<br>
context.fillStyle=‘red’<br>
context.beginPath();<br>
context.moveTo(x+a/2-(Math.sin(72Math.PI/180)a/2), y-Math.sin(18Math.PI/180)a/2);/1-ok/<br>
context.lineTo(x+a-2(a/2-(Math.sin(72Math.PI/180)a/2)),y-Math.sin(18Math.PI/180)a/2);/2-ok/<br>
context.lineTo(x+a/2-(Math.sin(36Math.PI/180)a/2),(Math.sin(54Math.PI/180)a/2)+y);/3-ok/<br>
context.lineTo(x+a/2,y-a/2);/4-ok/<br>
context.lineTo(x+a-(Math.sin(36Math.PI/180)a/2),(Math.sin(54Math.PI/180)a/2)+y);/5-ok/<br>
context.lineTo(x+a/2-(Math.sin(72Math.PI/180)a/2),y-Math.sin(18Math.PI/180)*a/2);/6-ok/<br>
context.fill();<br>
context.stroke();<br>
}<br>
console.log();<br>
filledStar(225,50,70);</p>
