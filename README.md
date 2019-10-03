# checkers-cmst103
//Code for a checkerboard pattern made for CMST 103 class
let boardSize = 500;
let sqCount = 8;
let size = boardSize/sqCount;
let color1 = "black";
let color2 = "red";

function setup() {
  createCanvas(boardSize,boardSize);
}

function draw() {
  background(255);
  for (let row = 0; row <= sqCount; row++) {
    //creates row
    for (let col = 0; col <= sqCount; col++) {
      if ( (col+row) % 2 === 0) {
      fill(color1) }
      else { 
      fill(color2)}
      square(col * size, row * size, size)
     /* if (row+i, i*size+size/2, tow*size+size/2)
        fill(color1)*/
    }
  }
}
