# class240
the repository for  class

this is h3


 //global variable
//colors
var red, blue, yellow;

//circle centers
var redX, redY, blueX, blueY, yellowX, yellowY;

//varcirclesize





//function
drawline(mouseX,mouseY,pmouseX,pmouseY){
//stroke(255,0,0);
//line(mouseX,mouseY,pmouseX,pmouseY);
//}

    
    
function.setup(){
createCanvas(windowwidth,windowHeight);
red = color(255,0,0);
yellow = color(255,255,0);
blue = color(0,0,255);
//set the sizeof the circles
circleSize = 90;
//set the location of the circles
redX = 100;
redY = 100;
yellowX = 100;
yellowY = 100;  
blueX = 100;   
blueY = 500;    

//create the three circles
fill(red); 
ellipse(redX,redY,circleSize,circleSize);
    
fill(yellow);    
    

    
ellipse(yellowX,yellowY,circleSize,circleSize);  
    
    
    
fill(blue);
ellipse(blueX,blueY,circleSize,circleSize);  
        

    

function draw(){
 if(mouseIsPressed){ 
   //draw a line
     stroke(linecolor);
     line(pmouseX,pmouseY,mouseX, mouseY);
 }
}//end draw()
    
    function mousepressed(){
        console.log('mouseClicke');
        var redLine = dist(mouseX, mouseY, redX, 
redY);
        var yellowLine = dist(mouseX, mouseY, yellowX, yellowY);
        var blueLine = dist(mouseX, mouseY, blueX, blueY);
     //   
    if(redLine < circleSize){
            //the clicked on the red circle
            //change the lineColor
            linecolor = red;
        }
//
if  (yellowLine < circkeSize) {
    //the clicked on the yellow circle
    //change the line color
    LineColor = yellow;
    }
    //
        if (blueLine < circleSize){
            console.log("clicked blue");
            console.log("blueLine",blueLine);
            console.log("circleSize", circleSize);
            linecolor = blue;
circleSize);                        
    }
    line(mouseX, mouseY,pmouseX,pmouseY);)
    }
