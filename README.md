# finalProject

# Project Title and purpose

One Paragraph of project description goes here

### Difficulties or opportunities you encountered along the way.

The toughest part was...

### Most interesting piece of your code and explanation for what it does.

```JavaScript
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
  
  let yOffset = height / 2; // Center the wave vertically
  let amplitude = 50; // Height of the wave
  let wavelength = 20; // Distance between points
  let waveSpeed = frameCount * 0.1; // Animation factor

  noFill();
  stroke(0);
  strokeWeight(2);
  
  beginShape();
  for (let x = 0; x < width; x += 10) { // Loop across the width
    let y = yOffset + sin((x + waveSpeed) * 0.1) * amplitude; // Sine wave calculation
    vertex(x, y); // Define each point
  }
  endShape();
}

```
This is the code that moves down the tree as decisions are made. It gets each value from both left and right and also casts the value to a String. If the progressions arrives at the leaf nodes, those values are printed.
## Built With

* [P5js](https://editor.p5js.org/) - The JavaScript editor used

## Authors

* **Billie Thompson** 

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
