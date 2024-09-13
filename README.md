# aula-tete
function setup() {
  createCanvas(400, 400);
  background('black')
 cor=color(random(0,255), random(0,255), random(0, 255));
 posicaohorizontal = 200;
  posicaovertical = 200;
} 

 function draw() {  
  fill("green");
  circle(posicaohorizontal,
 posicaovertical, 50);


  if(mouseX <  posicaohorizontal)  {
    posicaohorizontal--;
  }
  
  if(mouseX > posicaohorizontal) {
    posicaohorizontal++;   
  }

 if(mouseY < posicaovertical) { 
 posicaovertical--;
 }
 
 if(mouseY > posicaovertical) { 
   posicaovertical++;
 }
 
    if(mouseIsPressed) {
    cor=color(random(0, 255), random(0, 255), random (0, 255), 
   random(0, 100));  
        }
 
 }
