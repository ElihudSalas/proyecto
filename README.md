#maximum draws

instrucciones: 
1.-crear una carpeta con el archivo txt y el codigo .c 
2.-al compilar ya sea directamente de devc++ o en terminal cmd con el comando gcc "maximum-draws (1).c" -o maximum

obtendremos otro txt con los valores de salida 


descripccion:
una persona se esta preparando para irse y necesita un par de calcetines a juego. si existen varios colores de calcetines en el cajon
cuantos calcetines deben quitarse para estar seguros de tener un par a juego? 

tenemos una variable n que representa el color de cada par de calcetines 

solucion: 

suponemos que tenemos 3 pares de calcetines, sabiendo que cada par contiene dos calcetines, para asegurar que al menos uno tenfa par, debemos sacr un calcetin de cada par de calcetines y uno mas para que ese haga par con alguno de los antes ya obtenidos, es por eso que la funcion que hace falta es 

return n + 1;

para poder completar el codigo a esto se tiene que comdifical la linea de 

FILE* fptr = fopen(getenv("OUTPUT_PATH"), "w"); 

ya que el codigo trabaja con entradas que le proporciona la pagina misma por lo que debemos remplazar on las siguientes lineas y adjuntar un archivo txt. con las entradas para poder recibir las salidas correspondientes 

FILE* input_file = fopen("input1.txt", "r");
    FILE* output_file = fopen("output1.txt", "w");

    if (input_file == NULL || output_file == NULL) {
        printf("Error al abrir el archivo de entrada o de salida.\n");
        return 1;


el archivo txt contiene las salidas que se dan de ejemplo en la pagina hackerranks 
