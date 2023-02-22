Para poder solucionar el primero de los problemas para evitar que un componente salga de su espacio padre
se necesita poder colocar una propiedad de tipo overflow: hidden en css para que este pueda mantener al item
dentro, otra manera en la que se podria realizar seria colocando al elemento hijo una posicion sticky pero
esto impacta al momento de agregar mas elementos por ende se decarto ese tipo de posicion.

Para poder mostrar las imagenes de forma aleatoria se necesita poder acceder al arreglo en el cual se obtienen
los parametros necesarios, para esto realice un nuevo array en el cual almacene solamente los elementos que iba
a necesitar, en este caso solo al url para poder mostrar la imagen, seguido de esto se utilizo el parametro
color para poder mantener la estructura, al igual que se cambio en los estilos la propiedad 'color' por
'backgroundImage' en la cual se utilizo la url utilizar las imagenes traidas desde el fetch.

En el problema del rezise en el cual al realizar un estiramiento de la imagen realizaba un salto extraño para un lado o hacia la parte de arriba, para esto identifique en una de las constantes se estaba realizando de manera erronea la cual lleva por nombre absoluteTop, en la cual se le estaba sumando un valor extra al realizar el estiramientos de las imagenes, por lo cual decidi elimar esa suma y mantener el valor por defaul al realizar dicha modificacion, de esta manera se puede evitar ese error de salto.

Para poder eliminar los componentes ya existentes cree un boton en la cual se obtiene el array actual al igual que el tamaño del arreglo, de esta manera se puede filtrar los items para asi poder ir eliminando uno a uno del ultimo item generado hasta el primero.