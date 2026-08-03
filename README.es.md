<!-- hide -->
<div align="center">

# Master TypeScript: Arreglos

[![Tutorial certificado](https://img.shields.io/badge/4Geeks_Academy-Tutorial_certificado-2563eb)](https://4geeks.com/es/interactive-exercise)
[![Autocorregido con LearnPack](https://img.shields.io/badge/LearnPack-73_ejercicios_autocorregidos-2563eb)](https://github.com/learnpack/learnpack)
[![Abrir en GitHub Codespaces](https://img.shields.io/badge/Abrir_en-GitHub_Codespaces-fb5a1f)](https://codespaces.new/4GeeksAcademy/master-typescript-arrays-exercises)

Lee estas instrucciones en [🇺🇸 inglés](https://github.com/4GeeksAcademy/master-typescript-arrays-exercises/blob/HEAD/README.md)

</div>
<!-- endhide -->

Master TypeScript: Arreglos es un paquete de LearnPack con 74 carpetas de ejercicios: una pantalla de bienvenida y 73 retos autocorregidos. Escribes cada solución dentro de `app.ts` y 442 casos de prueba de Jest comprueban el valor que retorna tu función, nunca lo que imprimes. Cubre acceso por índice, mutación frente a copias, filtros, agregaciones, lógica numérica, matrices y búsqueda binaria, con instrucciones en español e inglés.

<!-- hide -->
## 📋 Sobre este tutorial

- **Dificultad:** intermedia, según declara `learn.json`; los primeros ejercicios son de nivel principiante y la exigencia sube de forma progresiva.
- **Ejercicios:** 74 carpetas, 73 de ellas con archivo de test automático.
- **Casos de prueba:** 442 en total, entre 3 y 14 por ejercicio, unos 6 de media.
- **Tecnologías:** TypeScript 5.9, Node.js 22, Jest 29.7.0 y la CLI de LearnPack.
- **Corrección:** automática y aislada por ejercicio, con `rewire` leyendo las funciones dentro de tu archivo compilado.
- **Idiomas:** cada ejercicio incluye `README.md` y `README.es.md`.
<!-- endhide -->

## 🎯 ¿Qué vas a aprender?

Este paquete es práctica pura sobre colecciones, con una idea por ejercicio:

- **Acceso por índice:** leer el primer elemento, el último y el enésimo, y qué retornar cuando esa posición no existe.
- **Mutar frente a copiar:** `push`, `unshift`, `shift` y `pop` modifican el array que recibiste; `slice`, `concat` y el operador spread crean uno nuevo. Hay cuatro parejas de ejercicios, ocho en total, cuyo único objetivo es que esa diferencia se te quede grabada.
- **Filtrar:** quedarte solo con los elementos que cumplen una condición y retornar un array vacío cuando no coincide ninguno.
- **Transformar:** elevar al cuadrado cada número, aplanar arrays de arrays, unir dos o tres arrays en uno solo.
- **Agregar:** total, producto, promedio, el más largo, el más corto, el mayor y el menor, incluso en arrays con elementos de tipos mezclados.
- **Cadenas como secuencias:** contar caracteres, separar una frase en palabras o en letras, colapsar espacios dobles, intercambiar caracteres por pares.
- **Lógica numérica sin atajos:** reconstruir `%` y `*` desde cero, factoriales, suma de dígitos, interés compuesto y conversión de puntaje a calificación.
- **Matrices:** leer `matrix[fila][columna]` sin romperte y transponer filas en columnas.
- **Algoritmos de búsqueda:** recorrer una cadena carácter a carácter en `getIndexOf` y aplicar búsqueda binaria sobre un array ordenado en los dos últimos ejercicios de búsqueda.
- **TypeScript aplicado:** interpretar la firma tipada que te dan y trabajar con `number[]`, `unknown[]`, `unknown[][]` y retornos de unión como `number | null`.

## 👀 ¿Qué vas a construir?

73 funciones pequeñas y tipadas, una por carpeta, repartidas en siete bloques progresivos. 40 reciben un array, 16 reciben una cadena, 13 reciben un número y 2 reciben una matriz; las dos restantes reciben booleanos (`or`) y objetos (`extend`):

- **`001`–`012` Acceso, agregar y quitar (12 ejercicios):** `getNthElement`, `getFirstElement`, `getLastElement`, `addToFront`, `addToBack`, `joinArrays`, `getElementsAfter`, `getElementsUpTo`, `removeFromFront`, `removeFromBack`, `removeFromFrontOfNew`, `removeFromBackOfNew`. Ejemplo: `getNthElement([1, 3, 5], 1)` retorna `3` y `getNthElement([], 3)` retorna `undefined`.
- **`013`–`025` Palabras, comparaciones y booleanos (13 ejercicios):** `countCharacter`, `getAllLetters`, `getAllWords`, `or`, `extend`, `convertDoubleSpaceToSingle`, `areValidCredentials`, `getIndexOf`, `findMinLengthOfThreeWords`, `findMaxLengthOfThreeWords`, `repeatString`, `getLongestOfThreeWords`, `findShortestOfThreeWords`. Aquí reconstruyes el operador `||` usando solo `!` y `&&`.
- **`026`–`033` Copias y filtros (8 ejercicios):** `joinThreeArrays`, `addToFrontOfNew`, `addToBackOfNew`, `getAllElementsButNth`, `keep`, `removeElement`, `filterOddLengthWords`, `filterEvenLengthWords`. Ejemplo: `keep([1, 2, 3, 2, 1], 2)` retorna `[2, 2]` y `keep([1, 2, 1, 2, 1], 3)` retorna `[]`.
- **`034`–`049` Agregaciones y arrays mixtos (16 ejercicios):** longitud del elemento más largo y del más corto, `squareElements`, `filterOddElements`, `filterEvenElements`, `computeProductOfAllElements`, `computeSumOfAllElements`, `joinArrayOfArrays` y cuatro funciones que buscan el número menor o mayor, y la palabra más corta o más larga, dentro de arrays que además contienen otros tipos.
- **`050`–`063` Lógica numérica (14 ejercicios):** `sum` y `average` juntas en el mismo archivo, `calculateBillTotal`, `multiplyBetween`, `computeSumBetween`, `computeSummationToN`, `convertScoreToGrade`, `convertScoreToGradeWithPlusAndMinus`, `computeFactorialOfN`, `sumDigits`, `computeCompoundInterest`, `modulo`, `multiply`, `isOddWithoutModulo`, `isEvenWithoutModulo`.
- **`064`–`070` Algoritmos sobre secuencias (7 ejercicios):** `flipPairs`, `flipEveryNChars`, `detectOutlierValue`, `findPairForSum`, `isRotated`, `search`, `isIsogram`. Ejemplo: `detectOutlierValue("2 4 7 8 10")` retorna `3`, la posición (empezando en 1) del único número impar.
- **`071`–`073` Matrices y búsqueda binaria (3 ejercicios):** `getMatrixValue`, `transposeMatrix`, `binarySearchSortedArray`. Ejemplo: `transposeMatrix([[1, 2, 3], [4, 5, 6]])` retorna `[[1, 4], [2, 5], [3, 6]]` y `binarySearchSortedArray([1, 3, 5, 7, 9], 7)` retorna `3`.

## 🎓 ¿Qué necesitas antes de empezar?

- **Fundamentos de JavaScript:** variables, `if`, bucles y saber llamar a una función. El paquete arranca en `arr[n]` y da por hecho que eso ya lo tienes.
- **Nada de TypeScript avanzado:** cada `app.ts` llega con la firma ya tipada, por ejemplo `function keep(arr: number[], keeper: number): number[]`. Lo tuyo es el cuerpo de la función, no diseñar los tipos.
- **Cero instalación si usas Codespaces:** el contenedor deja listos Node.js 22, Jest 29.7.0, la CLI de LearnPack y el plugin de TypeScript.
- **Node.js si trabajas en local:** son programas de consola; en todo el paquete no hay navegador, ni HTML, ni DOM.

## ✅ ¿Cómo funciona la corrección automática?

73 de las 74 carpetas incluyen un archivo `test.js`; la única sin test es `00-Welcome`, la pantalla de bienvenida. Cuando pulsas `Test` ocurren cuatro cosas:

1. El plugin de TypeScript de LearnPack lee tu `app.ts` y lo compila a `app.js` usando el `tsconfig.json` del proyecto (target ES2019, módulos CommonJS).

2. `rewire` carga ese `app.js` compilado y extrae tu función **por su nombre exacto**, con una línea del estilo `const keep = rewire('./app.js').__get__('keep')`.

3. Jest 29.7.0 ejecuta las comprobaciones. Los 73 archivos verifican primero que la función existe, 69 comprueban además que retorna algo y 62 revisan con `typeof` el tipo de lo que devuelve, antes de probar valores concretos.

4. Ninguno de los 442 casos de prueba mira la consola. Todas las comprobaciones llaman a tu función y comparan el valor retornado, así que aquí `console.log` sirve para depurar, nunca como respuesta.

Ese mismo `learnpack audit` se ejecuta en GitHub Actions con Node.js 22 en cada push, y por eso los archivos de los ejercicios se mantienen consistentes.

> 💡 Los errores de tipos no tumban los tests. El plugin transpila tu archivo en lugar de comprobar tipos, así que solo un error de sintaxis detiene la ejecución. Para la revisión estricta completa ejecuta `npm run typecheck`, que lanza `tsc --noEmit` con `"strict": true`.

## 💡 ¿Qué errores debes evitar?

1. **Imprimir en vez de retornar.** Cero tests leen la consola. Si tu función termina en `console.log(resultado)` y no tiene `return`, retorna `undefined` y fallan todas las comprobaciones aunque la salida se vea perfecta.

2. **Editar `app.js` en lugar de `app.ts`.** El plugin regenera `app.js` a partir de `app.ts` en cada Run y en cada Test, así que todo lo que escribas directamente en el archivo JavaScript se sobrescribe antes de corregirse.

3. **Cambiarle el nombre a la función.** `rewire` la busca por nombre literal, y en cinco ejercicios el nombre de la carpeta no coincide con el de la función: `045-joinArraysOfArrays` espera `joinArrayOfArrays`, `047-findSmallestnumberAmongMixedElements` espera `findSmallestNumberAmongMixedElements`, `050-averageIntegers` espera `sum` y `average`, `056-convertScoreToGradeWithPlus` espera `convertScoreToGradeWithPlusAndMinus` y `070-isogram` espera `isIsogram`. Fíate del esqueleto de `app.ts`, no de la carpeta.

4. **Usar el operador prohibido en `060` y `061`.** Los dos tests leen el archivo compilado como texto plano y le pasan una expresión regular. `060 modulo` falla si aparece un `%` en cualquier parte y `061 multiply` falla si aparece un `*` en cualquier parte, comentarios incluidos: un `/* ... */` olvidado basta para suspender el ejercicio.

5. **Resolver el `050` con una sola función.** Ese archivo trae dos esqueletos, `sum` y `average`, y los dos se corrigen. Además las instrucciones piden reutilizar la primera dentro de la segunda: `sum(arr) / arr.length`.

6. **Confundir la versión que muta con la que copia.** `004 addToFront` y `009 removeFromFront` trabajan sobre el array que recibes; `027 addToFrontOfNew` y `011 removeFromFrontOfNew` deben dejarlo intacto. Los tests del `011` y del `012` revisan el array de entrada después de llamarte: `removeFromFrontOfNew([9, 21, 74, 33])` tiene que retornar `[21, 74, 33]` y dejar la entrada tal cual, `[9, 21, 74, 33]`. El `027` y el `028` cazan el mismo error por otra vía: exigen que el array retornado sea más largo que el que recibiste.

7. **Saltarte los casos límite que están en las instrucciones.** Se corrigen: un array vacío retorna `undefined` en el `001`, `keep` retorna `[]` cuando no coincide nada, `getMatrixValue` retorna `undefined` si la fila o la columna no existen, y los dos ejercicios de búsqueda difieren a propósito, porque `069 search` retorna `null` cuando no encuentra el valor mientras que `073 binarySearchSortedArray` retorna `-1`.

8. **Dejar el retorno de relleno.** La mayoría de los esqueletos vienen con `return 0;`, `return '';`, `return false;` o `return [];` debajo del comentario `// your code here`, y seis llegan sin ningún `return`. Están ahí para que el archivo compile, no como respuesta válida.

## ❓ Preguntas frecuentes

### ¿Necesito saber TypeScript para empezar?

No, pero sí JavaScript. Cada ejercicio te entrega la firma ya tipada, así que lees tipos en lugar de diseñarlos. Te vas a acostumbrar a `number[]`, `string`, `unknown[]`, `unknown[][]` y a retornos de unión como `number | null` solo con rellenar 73 cuerpos de función. Si nunca has visto una anotación de tipos, con el capítulo de [tipos del día a día](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html) del manual oficial vas sobrado.

### ¿Puedo resolver los ejercicios con JavaScript normal dentro de `app.ts`?

Sí, y pasarán, porque TypeScript es un superconjunto de JavaScript y el plugin transpila el archivo en lugar de comprobar tipos. Pero pierdes el sentido del paquete: la gracia está en respetar los tipos declarados. Ejecuta `npm run typecheck` en la raíz para ver qué opina el modo estricto de tus soluciones.

### ¿Por qué falla el ejercicio si la salida de la consola es correcta?

Porque nadie está corrigiendo la consola. Los tests llaman a tu función con valores que probablemente no probaste, como un array vacío, un índice de matriz fuera de rango o un número negativo, y comparan el valor retornado. Lee el nombre de la comprobación que falla: te dice exactamente qué caso se rompió.

### ¿Tengo que instalar algo para practicar?

No, si abres el repositorio en [GitHub Codespaces](https://codespaces.new/4GeeksAcademy/master-typescript-arrays-exercises): el contenedor instala Node.js 22, Jest 29.7.0, LearnPack y el plugin de TypeScript, y los ejercicios se abren dentro de VS Code. [Gitpod](https://gitpod.io#https://github.com/4GeeksAcademy/master-typescript-arrays-exercises) también está configurado. En local solo necesitas Node.js y tres comandos.

### ¿En qué se diferencian los ejercicios `069` y `073`?

Los dos implementan búsqueda binaria sobre un array ordenado y los dos retornan el índice cuando encuentran el valor. Lo que cambia es el contrato de fallo: `069 search` retorna `null` si el valor no está en el array, mientras que `073 binarySearchSortedArray` retorna `-1`. Es intencionado, porque las dos convenciones se usan en proyectos reales y cada test comprueba la suya al pie de la letra.

### ¿Cuesta algo y de quién es el código que escribo?

El repositorio es público, así que clonarlo y resolver los 73 ejercicios no cuesta nada, y las soluciones que escribas dentro de `app.ts` son código tuyo. Ten en cuenta que este repositorio no incluye archivo `LICENSE`, de modo que por defecto no concede permiso de redistribución sobre su contenido: si quieres republicar o reutilizar los ejercicios, consúltalo antes con 4Geeks Academy.

<!-- hide -->
## 📚 Tutoriales relacionados

Este paquete forma parte de la serie interactiva de TypeScript y da continuidad a la de JavaScript:

1. [Fundamentos de TypeScript con práctica para desarrolladores JavaScript](https://4geeks.com/es/interactive-exercise/fundamentos-de-typescript-con-practica-para-desarr)
2. [Master TypeScript: Funciones](https://github.com/4GeeksAcademy/master-typescript-functions-exercises), 42 ejercicios autocorregidos
3. **Master TypeScript: Arreglos** ← estás aquí
4. [Master TypeScript: Objetos](https://github.com/4GeeksAcademy/master-typescript-objects-exercises), 55 ejercicios autocorregidos

Si los arrays todavía se te atragantan, calienta motores con [Ejercicios de arrays y loops de Javascript interactivos](https://4geeks.com/es/interactive-exercise/javascript-array-loops-exercises-es) y luego vuelve aquí.

## 🚀 Cómo empezar

Lo más rápido es [abrirlo en GitHub Codespaces](https://codespaces.new/4GeeksAcademy/master-typescript-arrays-exercises). El contenedor instala todo y VS Code abre los ejercicios por ti.

Si no arrancan solos, ejecuta esto en la terminal:

```bash
learnpack start
```

También puedes abrir el paquete en [Gitpod](https://gitpod.io#https://github.com/4GeeksAcademy/master-typescript-arrays-exercises). Usa el menú superior para moverte entre ejercicios y para cambiar las instrucciones entre español e inglés.

## 💻 Instalación local

Clona el repositorio y sigue estos pasos, con Node.js ya instalado:

1. Instala LearnPack de forma global:

    ```bash
    npm i @learnpack/learnpack -g
    ```

2. Instala el plugin de TypeScript que viene dentro de este repositorio:

    ```bash
    learnpack plugins:install file:$(pwd)/learnpack-typescript-plugin
    ```

3. Arranca los ejercicios desde la misma carpeta donde está `learn.json`:

    ```bash
    learnpack start
    ```

Si algo se tuerce, la [guía rápida de LearnPack para estudiantes](https://4geeks.com/docs/learnpack/quickstart-for-learners) repasa la instalación completa.

## 📚 Cómo están organizados los ejercicios

Cada una de las 73 carpetas de ejercicio dentro de [`exercises/`](https://github.com/4GeeksAcademy/master-typescript-arrays-exercises/tree/HEAD/exercises) contiene siempre los mismos seis archivos, con `00-Welcome` como única excepción, porque solo tiene los dos README:

- **`app.ts`:** el único archivo que editas. Llega con la firma tipada, un comentario `// your code here` y un `export {}` al final que convierte el archivo en un módulo.
- **`app.js`:** la salida compilada que ejecuta LearnPack y que importa Jest. Se regenera desde `app.ts` en cada Run y cada Test.
- **`README.md`:** las instrucciones en inglés.
- **`README.es.md`:** las mismas instrucciones en español.
- **`test.js`:** el archivo de Jest que corrige tu solución. No necesitas abrirlo, aunque leerlo te dice exactamente qué se te está pidiendo.
- **`solution.hide.js`:** una solución funcional, que LearnPack mantiene oculta hasta que la pides.

En la raíz del repositorio están además el `tsconfig.json` con `"strict": true` y los scripts de npm `typecheck`, `audit:signatures`, `regenerate:app-ts` y `transpile:all`, que sirven para mantener sincronizados los 73 esqueletos con sus tests.

## 🤝 Colaboradores

- [Ehiber Graterol (ehiber)](https://github.com/ehiber): único colaborador en el historial del repositorio; autor de los ejercicios, de sus tests y del plugin de TypeScript de LearnPack.
- Según el [CHANGELOG.md](https://github.com/4GeeksAcademy/master-typescript-arrays-exercises/blob/HEAD/CHANGELOG.md), los primeros bloques de ejercicios en los que se basa este paquete los escribió Mike Berrio.

Puedes ver la lista completa en el [gráfico de colaboradores](https://github.com/4GeeksAcademy/master-typescript-arrays-exercises/graphs/contributors). Se agradece cualquier contribución: si encuentras un error o una errata en un ejercicio, abre un issue o manda un pull request.
<!-- endhide -->
