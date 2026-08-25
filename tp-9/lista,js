var listaNumerosEjemplo = [2, 4, 6, -1, 5, -4, 0];


/**
 * 01 - invertirLista
 */
function invertirLista(listaDeNumeros) {
    // Usamos .slice() para crear una copia del array antes de invertirlo con .reverse()
    // Así evitamos modificar la lista original que entra por parámetro
    return listaDeNumeros.slice().reverse();
}
console.log("invertirLista([2,3,4]): ", invertirLista([2,3,4]));


/**
 * 02 - sumarLista
 */
function sumarLista(listaDeNumeros) {
    return listaDeNumeros.reduce((acumulado, num) => acumulado + num, 0);
}
console.log("sumarLista([2,3,4]): ", sumarLista([2,3,4]));


/**
 * 03 - contarElementosLista
 */
function contarElementosLista(listaDeNumeros) {
    return listaDeNumeros.length;
}
console.log("contarElementosLista([2,3,4]): ", contarElementosLista([2,3,4]));


/**
 * 04 - calcularPromedio
 */
function calcularPromedio(listaDeNumeros) {
    if (contarElementosLista(listaDeNumeros) === 0) return 0;
    
    // Reutilizamos sumarLista y contarElementosLista
    return sumarLista(listaDeNumeros) / contarElementosLista(listaDeNumeros);
}
console.log("calcularPromedio([2,3,4]): ", calcularPromedio([2,3,4]));
console.log("calcularPromedio(listaNumerosEjemplo): ", calcularPromedio(listaNumerosEjemplo));


/**
 * 05 - triplicarLista
 */
function triplicarLista(listaDeNumeros) {
    return listaDeNumeros.map(num => num * 3);
}
console.log("triplicarLista([1, 2, 3]): ", triplicarLista([1, 2, 3]));


/**
 * 06 - crearListaDeNumeros
 */
function crearListaDeNumeros(inicio, fin) {
    const lista = [];
    for (let i = inicio; i <= fin; i++) {
        lista.push(i);
    }
    return lista;
}
console.log("crearListaDeNumeros(2,5): ", crearListaDeNumeros(2,5));


/**
 * 07 - ordenarDeMayorAMenor
 */
function ordenarDeMayorAMenor(listaDeNumeros) {
    // Usamos .slice() para no mutar el array original y ordenamos de mayor a menor (b - a)
    return listaDeNumeros.slice().sort((a, b) => b - a);
}
console.log("ordenarDeMayorAMenor([2,3,4]): ", ordenarDeMayorAMenor([2,3,4]));
console.log("ordenarDeMayorAMenor(listaNumerosEjemplo): ", ordenarDeMayorAMenor(listaNumerosEjemplo));


/**
 * 08 - encontrarNumeroMayor
 */
function encontrarNumeroMayor(listaDeNumeros) {
    return Math.max(...listaDeNumeros);
}
console.log("encontrarNumeroMayor([2,3,4]): ", encontrarNumeroMayor([2,3,4]));
console.log("encontrarNumeroMayor(listaNumerosEjemplo): ", encontrarNumeroMayor(listaNumerosEjemplo));


/**
 * 09 - ordenarPalabrasPorLongitud
 */
function ordenarPalabrasPorLongitud(listaDePalabras) {
    return listaDePalabras.slice().sort((a, b) => a.length - b.length);
}
console.log("ordenarPalabrasPorLongitud(['abc', 'a', 'ab']): ", ordenarPalabrasPorLongitud(['abc', 'a', 'ab']));


/**
 * 10 - encontrarPalabraMasCorta
 */
function encontrarPalabraMasCorta(listaDePalabras) {
    if (listaDePalabras.length === 0) return "";
    
    return listaDePalabras.reduce((masCorta, palabraActual) => {
        return palabraActual.length < masCorta.length ? palabraActual : masCorta;
    });
}
console.log("encontrarPalabraMasCorta(['abc', 'a', 'ab']): ", encontrarPalabraMasCorta(['abc', 'a', 'ab']));


/**
 * 11 - filtrarSoloPositivos
 */
function filtrarSoloPositivos(listaDeNumeros) {
    return listaDeNumeros.filter(num => num > 0);
}
console.log("filtrarSoloPositivos([1,-1,0]): ", filtrarSoloPositivos([1,-1,0]));
console.log("filtrarSoloPositivos(listaNumerosEjemplo): ", filtrarSoloPositivos(listaNumerosEjemplo));


/**
 * 12 - contarAprobados
 */
function contarAprobados(listaDeNotas) {
    // Asumiendo que se aprueba con 6 o más
    const aprobados = listaDeNotas.filter(nota => nota >= 6);
    return contarElementosLista(aprobados);
}
console.log("contarAprobados([10, 4, 6, 7, 1, 9]): ", contarAprobados([10, 4, 6, 7, 1, 9]));


/**
 * 13 - filtrarSoloTruthy
 */
function filtrarSoloTruthy(listaDeValores) {
    // Boolean convierte cada elemento a true si es truthy o false si es falsy
    return listaDeValores.filter(Boolean);
}
console.log("filtrarSoloTruthy(): ", filtrarSoloTruthy(["Hola", "", null, 1, 0, -1, undefined, [], {}]));


/**
 * 14 - enumerarLista
 */
function enumerarLista(listaDePalabras) {
    if (listaDePalabras.length === 0) return "";
    if (listaDePalabras.length === 1) return `${listaDePalabras[0]}.`;

    // Tomamos todas las palabras excepto la última
    const primerasPalabras = listaDePalabras.slice(0, -1).join(", ");
    // Tomamos la última palabra
    const ultimaPalabra = listaDePalabras[listaDePalabras.length - 1];

    return `${primerasPalabras} y ${ultimaPalabra}.`;
}
console.log("enumerarLista(): ", enumerarLista(["Han", "Leia", "Luke", "Yoda"]));
