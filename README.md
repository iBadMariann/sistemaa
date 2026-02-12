<!DOCTYPE html>
<html>
<head>
<title>Sistema de Mariann</title>

<style>
body {
  background-color: black;
  color: #fff9f8;
  font-family: monospace;
  font-size: 18px;
  padding: 40px;
  transition: 1s;
}

#terminal::after {
  content: "|";
  animation: blink 1s infinite;
}

@keyframes blink {
  50% { opacity: 0; }
}

button {
  background-color: #ff4da6;
  border: none;
  padding: 12px 25px;
  color: white;
  border-radius: 8px;
  font-size: 16px;
  margin-top: 25px;
  cursor: pointer;
  display: none;
}
</style>
</head>

<body><body>

<audio id="musicaFinal" loop>
  <source src="musica.mp3" type="audio/mp3">
</audio>

<div id="terminal"></div>

<button id="btn1" onclick="recuerdos()">Ver recuerdos desbloqueados</button>
<button id="btn2" onclick="final()" style="display:none;">Abrir archivo definitivo</button>

<script>

const mensajes = [
  "Bienvenido al Sistema de Mariann",
  "yo soy tu asistente virtual, diseñado para ayudarte a entender y analizar tus sentimientos de mariann o eso creo...",
  "por lo tanto yo os guiaré en este proceso",
  "muy bien, comencemos",
  "Cargando Sistema de Mariann...",
  "Versión anterior detectada.",
  "...",
  "Errores encontrados:",
  "- Miedo a todo lo que se le cruce.",
  "- Pensamientos en bucle.",
  "- Kaoss interno activo.",
  "basicamente como podemos apreciar, el gordito teton de mariann no estaba taaan estable, es decir, algunas cositas le pasaban",
  "pwro chill",
  "vamos a hacer algunos cambios, ahh",
  "Buscando actualización externa...",
 "OSTIAAAAAAAAAAAAAAAAAAAAAAAAAA....",
  "actualizacion encontrada...",
  "desea instalarla? SI/NO",
  "-Mariann: no estoy del todo seguro del cambio, pwro va, SI",
  "-sistema: okey bro, comenzando instalación...",
  "comenzando la instalacion...",
  "Instalando nueva versión... 0%",
  "Instalando nueva versión... 25%",
  "Instalando nueva versión... 50%",
  "Instalando nueva versión... 75%",
  "Instalando nueva versión... 100%",
  "instalacion completada.",

  "mostrando cambios...",


"OSTAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA",
  "Nueva energía detectada...",
  "Nombre: YAZMIN",

  "-sistema:deseas continuar?",
  "-Mariann:ostia chaval, claro que si",
  "-sistema:...",
  "okey bro, datos a tener en cuenta:",
  "es el genero opuesto al tuyo bro xd",
  "es decir, es una mujer bro",
  "-Mariann:ya lo se bro, tranki",
  "-sistema:por lo tanto todas mienten, no?...",

  "error",
  "system34 está fallando...",
  "-Mariann: y ahora que te pasa",
  "-sistema: no se bro, no se que me pasa, creo que es algo interno,  no se si es por la actualización o que, pero",
  "vamos a scanear todo el sistema para detectar que fue...",
  "...",

  "scan realizado pwro....",
  "ninguna mentira detectada...",
  "-Mariann:ps es obvio, estamos hablando de Yazmin, que te pensas?",
  "-sistema: bueno si vos decis",
  "hablas como si ya la conocieras de antes bro, que raro...",
  "solicitando permisos para escanear mas a fondo...",
  "-Mariann: prosiga",
  "verificación manual en proceso...",
  "que raro...",
  "figura como tu mamá we...",
  "como tu mejor amiga también...",
  "-Mariann: JAJSAJSJ pasan que cosas pwro ya te vas a dar cuenta y vas a entender un poco mas",
  "-sistema:ostia chaval, bueno, sigamos con el análisis...",

  "Compatibilidad emocional: 100%",
"euuu, es un montonnn",
"que me ocultas?",
"-mariann: shhhh vos segui nomas",
"-sistema:bueno, sigamos con el análisis...",

  "...",
  "Efectos secundarios detectados:",
  "ahre virgo de mierda, era algo por el 14 de febrero",
  "-Mariann: ostia chaval, me re fui de tema",
  "que iba a decir?...",
  "-sistema: sos tonto o te haces? YAZMIN ahora si te acordas que ibas a hacer????",
  "-Mariann: que si chaval, solo estaba jodiendo",


];

let i = 0;
let j = 0;
let textoActual = "";
let velocidad = 30;

function escribir() {
  if (i < mensajes.length) {
    if (j < mensajes[i].length) {
      textoActual += mensajes[i][j];
      document.getElementById("terminal").innerHTML = textoActual;
      j++;
      setTimeout(escribir, velocidad);
    } else {
      textoActual += "<br><br>";
      i++;
      j = 0;
      setTimeout(escribir, 500);
    }
  } else {
    document.getElementById("btn1").style.display = "inline-block";
  }
}

function recuerdos() {
  document.getElementById("terminal").innerHTML =
  "-sistema:Analizando Latidos...<br><br>" +
  "Frecuencia cardiaca inestable con ella, estable sin ella...<br><br>" +
 "mariann, te seguis poniendo nerviso o es pq la amas mucho?<br><br>" +
 "mariann:....<br><br>" +
  "-sistema: pueda que la ames bro, meparece, no se, digo lo que veo en el sistema<br><br>" +
  "que dices bro?...<br><br>" +
  "-Mariann: y no te equivocas, yo la amo mucho, es mi luz en la oscuridad y en plena luz del dia, es todo para mi<br><br>" +
  "-sistema:se ve que de verdad la amas bro, no es solo un capricho o algo pasajero, se nota que es algo profundo y real lo que sientes por ella<br><br>" +
 "comprobando en el sistema...<br><br>" +
  "conclusion final: estoy, digo... estas muy enamorado de esa personita.<br><br>" +
  "no te preocupes bro, es algo hermoso lo que sientes por ella, es algo que no se puede explicar con palabras, es algo que se siente en el corazón y en el alma<br><br>" +
  "y bueno, ahora que ya sabes eso, solo queda disfrutar de ese amor tan bonito que tienes por ella y seguir construyendo recuerdos juntos<br><br>" +
  "que lindo bro, me alegra mucho por vos y por ella, se nota que son el uno para el otro<br><br>" +
  "bueno, sigamos con el análisis...<br><br>" +
  "-Mariann:amor?<br><br>" +
"en serio crees que eso era todo? jajaja<br><br>" +
"nono, esto no puede terminar asi<br><br>" +
  "porfavor mariann del pasado, ponele un poco mas de color gordo qliao<br><br>" +
  "perdon amor, ahora si, tocá el boton para entrar en un mejor ambiente (ponele)";
document.getElementById("btn1").style.display = "none";
  document.getElementById("btn2").style.display = "inline-block";
}

function final() {

  let musica = document.getElementById("musicaFinal");
  musica.volume = 0.3;
  musica.play();

  document.body.style.backgroundColor = "#1a001a";
  document.body.style.color = "#ff4da6";

  document.getElementById("terminal").innerHTML =

  document.body.style.backgroundColor = "#1a001a";
  document.body.style.color = "#ff4da6";

  document.getElementById("terminal").innerHTML =
  "-Mariann:ahora si xd...<br><br>" +
  "Hola mi amorr<br><br>" +
  "como estas??<br><br>" +
  "todo bien, todo correcto??<br><br>" +
  "bueno, ojala que si bro, ahh<br><br>" +
  "el plan es el siguiente amor, el 14 caigo a tu casa con las manos vacias o con unas pepitos y cuando estemos desayunando, plash, video de esto o el link de la pagina<br><br>" +
  "claramente video en el hipotetico caso de que yo a esto no lo pueda transformar en una pagina normal<br><br>" +
  "dada esta pequeña introducción<br><br>" +
  "comencemos<br><br>" +
  "ahr pq hablaba asi si esto no va a parecer de a poco como en la primera parte xd<br><br>" +
  "bueno<br><br>" +
  "yazmin, mi amor, mi vida, mi todo<br><br>" +
  "mi novia que yo amo tanto (por cierto, unica novia)<br><br>" +
  "hoy es un dia seria un dia especial o uno normal?<br><br>" +
  "pregunto pq yo no solo te amo en fechas importantes si no mas bien yo te amo todo el tiempo<br><br>" +
  "cada dia, cada hora, cada segundo<br><br>" +
  "asi que se podria decir que lo que yo siento por vos no necesita una fecha en concreto como para tener que celebrarla? no se pwro no masivoo<br><br>" +
  "pwro bueno...<br><br>" +
  "quiero aprovechar este primer San Valentín (primero muchos, muchos san valentins)(lo digo asi para que no aparezca el nombre de otro, no por bruto JAJSJKAJS)<br><br>" +
  "para decirte...<br><br>" +
  "yo como persona en serio que te amo un monton y si, la palabra se queda corta ya lo que yo siento va mas allá por sobretodo y siento que ya lo habré dicho en varias ocasiones pwro es que es verdad<br><br>" +
  "y si...<br><br>" +
  "capaz que eso no se note a simple vista lo cual puede ser verdad, pero yo se que vos sabes lo que yo siento por vos por mas que me trates de infiel, rata asquerosa o chanta xd<br><br>" +
  "pwro...<br><br>" +
  "te amo, no se el pq pwro te amo un monton.<br><br>" +
"en otras noticias, te gusto el metodo? que opinas? claramente me falta pulirme pwro approved?<br><br>" +
"si es asi besito, ahr que lo vas a ver despues de que me vaya xdd<br><br>" +
"bro, era una carta y el chavon hablaba solo JAJSJJAJSJ dios, unos problemitass<br><br>" +
"volviendo a lo importante<br><br>" +
"lo unico que quiero ademas de cumplir nuestras metas juntos, es verte feliz yhacerte sentir la personita mas especial de este mundo,<br><br>" +
"ya que lo sos para mi, sos lo mas importante que tengo y lo que mas quiero en este mundo<br><br>" +
"te amo mucho mi amor, y espero que podamos seguir construyendo recuerdos juntos y seguir creciendo como pareja cada dia mas<br><br>" +

  "Feliz san valentín mi amor, te amo mucho❤️<br><br>" +
  "like si llegaste hasta el final ahhh<br><br>" +
  "❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️❤️";

  document.getElementById("btn2").style.display = "none";
}

escribir();

</script>

</body>
</html>
