//# juego-prueba
//primer repositorio de juego piloto
alert('vamos a jugar un juego divertido, pon mucha atención') 
let numeromaximoposible=20;
let numeroSecreto = Math.floor(Math.random()*numeromaximoposible)+1;
let numeroUsuario = 0;
let intentos = 1;
let palabraveces= 'vez';
let maximosintentos= 6;
console.log(numeroSecreto);
while (numeroUsuario != numeroSecreto){ 
    numeroUsuario=parseInt(prompt (`escribe un número entre 1 y ${numeromaximoposible}:`));
 console.log(typeof(numeroUsuario));
  
  if (numeroUsuario == numeroSecreto) {
    alert(`¡Genial! acertaste, el numero es ${numeroUsuario},lo hiciste en ${intentos} ${intentos == 1?'vez':'veces'} `);
   }
     else{
     alert('casi...pero no, intentalo otra vez')
     intentos = intentos +1;
     if (numeroUsuario > numeroSecreto){
     alert('el numero secreto es menor');
     } else{
     alert ('el numero secreto es mayor');
    }
    //intentos = intentos +1;
    intentos++;
    if (intentos >maximosintentos){
      alert (`llegaste al número de intentos máximo${maximosintentos}, intenta otra vez`)
      break;
    }
  }
//}
