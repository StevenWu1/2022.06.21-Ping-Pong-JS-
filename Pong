function setup() {
  createCanvas(600, 400);
}

let mousex = 0;
let mousey = 300;
let circleX = 25;
let speed = 3;
let circley = 25;
let speedy = 3;
let circleSize = 50;
let border = 0;
let padWidth = 150;
let padHeight = 15;
let bounceCount = 0;
let calor = (0, 0, 0);
function draw() {
  background("black");
  stroke("white");
  strokeWeight(border);
  fill("white");
  text("Bounces: ", 525, 20);
  text(bounceCount, 575, 20);
  mousex = mouseX;
  rect(mouseX-50, 300, padWidth, padHeight);

  circle(circleX, circley + border, circleSize);
  if (circleX > width - circleSize/2) {
    speed = speed * -1;
  } 
  if (circleX < 0 + circleSize/2) {
    speed = speed * -1;
  }
  if (circley > height - circleSize/2) {
    speedy = speedy * -1;
  }
  if (circley < 0 + circleSize/2) {
    speedy = speedy * -1;
  }
  circleX = circleX + speed;  
  circley = circley + speedy;

  bouncePad();
}

function fillcircle() {
  fill(random(0, 255), random(0, 255), random(0, 255));
}

function bouncePad() {
  if (circleX > (mousex - circleSize / 2 - padHeight - 25)) {
    if (circleX < (mousex + (circleSize / 2) + padWidth)){
      if (circley >= 290) {
        if (circley <= 310){
          fillcircle();
        speedy = speedy * -1.1;
        bounceCount = bounceCount + 1;
        }
      }
    } 
  }
}
