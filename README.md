let xBolinha = 300;
let yBolinha = 200;
let diametro = 20;

let velocidadeXBolinha = 6;
let velocidadeYBolinha = 6;

function setup() {
    createCanvas(600, 400);
}

function draw() {
    background(0);
    circle(xBolinha, yBolinha, diametro);
    xBolinha += velocidadeXBolinha;
    yBolinha += velocidadeYBolinha;
    
   if (xBolinha > width || xBolinha < 0) {
    velocidadeXBolinha *= -1;
    }

 if (yBolinha > height || yBolinha < 0) {
        velocidadeYBolinha *= -1;
    }
   
}

