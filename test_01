*
Primera prueba para una obra de desplazamiento medial:
transcribir un poema a código. El poema es el siguiente:

el magenta es el no verde
pero el verde
   no es el no magenta
verde es el pasto no seco
*/

int x,y;

//para ejecutar en pantalla completa:
boolean sketchFullScreen() {
  return true;
}

void setup() {
  size(1366,768);
  //size(250,250);
  background(0);
  smooth();
  
  PFont f = createFont("Courier", 50); // create the font and set the text rendering size to 175
  textFont(f); // use the font for upcoming text rendering (i.e. when using the text() method)
  textAlign(CENTER, CENTER);
}

void draw() {
  //create an alpha blended background
  //fill(0,1);
  
  //strokeWeight(200); // 
   
  rect(0,0,width,height);

  //probabilities for 3 different cases (these need to add up to 100% since something always occurs here!)
  float p1   = 0.5;               // 5% chance of pure white occurring
  float p2 = 0.50 + p1;    // 80% chance of gray occuring
  //float p3  = 1.0 - p2 ; // 15% chance of black (we don't actually need this line since it is
  // by definit n, the "in all other cases" part of our else
    float num = random(1);                 // pick a random number between 0 and 1
  if (num <p1) {
    fill(255, 0, 255);
  } else if (num < p2) {
    fill(0,255,0);
  } else {
    fill(200,90,255);
  }

  // el color del texto desplegado 
  // es el mismo que el del lienzo de fondo
  // pero se ve distinto debido al efecto de parpadeo a gran velocidad
  text("el pasto es verde", width/2, height/2); 

}
