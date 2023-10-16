# javascript-tp-doce
js con array 
//  creación de un array vacío para guardar las palabras
var palabras = [];

// se pide que introduzca 8 palabras por teclado
for (var i = 0; i < 8; i++) {
    var palabra = prompt("Introduce una palabra: ");
    // se agrega la palabra al array
    palabras.push(palabra);
}

// Imprime el array en el documento
document.write("El array de palabras es: " + palabras);

// Definimos la función que genera un número entero aleatorio en un rango
function numeroAleatorio(min, max) {
  // Usamos la función Math.random() para obtener un número entre 0 y 1
  var rand = Math.random();
  // Calculamos el rango total como max - min + 1
  var range = max - min + 1;
  // Multiplicamos el rango por el número aleatorio y lo sumamos al mínimo para obtener el número dentro del rango especificado
  return Math.floor(rand * range + min);
}

// Pedimos al usuario que introduzca el rango
var min = parseInt(prompt("Introduce el límite inferior del rango: "));
var max = parseInt(prompt("Introduce el límite superior del rango: "));

// Llamamos a la función y mostramos el resultado
var resultado = numeroAleatorio(min, max);
alert("El número aleatorio entre " + min + " y " + max + " es: " + resultado);
