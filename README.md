# Pirámide

Solver en HTML para el **Rubik's Pyramid / Pyramorphix**.

El programa permite cargar manualmente los colores de las cuatro caras y calcula una secuencia de movimientos para llevar la pirámide al estado resuelto.

## Uso

1. Colocar el rompecabezas en forma de pirámide.
2. Identificar cada cara por el color de su triángulo central.
3. Para cada cara:
   - indicar qué cara queda abajo;
   - cargar los tres triángulos exteriores tal como se ven.
4. Presionar **Resolver**.
5. Seguir los movimientos indicados por la página.

La solución usa los movimientos

- `R`, `R2`, `R3`;
- `L`, `L2`, `L3`;
- `B`, `B2`, `B3`.

El número indica cuántos cuartos de vuelta se hacen en el mismo sentido. Por ejemplo, `R3` equivale a tres movimientos `R` consecutivos.

Durante la resolución se muestra también el estado esperado de la pirámide para poder controlar el procedimiento.

## Archivos

El proyecto no necesita servidor ni dependencias externas.

```text
piramide/
├── index.html
└── README.md
```

Para usar la versión actual, renombrar:

```text
rubiks_pyramid_solver_v5.html
```

como:

```text
index.html
```

## GitHub Pages

1. Crear o usar el repositorio `piramide`.
2. Subir `index.html` y `README.md` a la rama principal.
3. En GitHub ir a:

   **Settings → Pages**

4. En **Build and deployment**, elegir:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main`
   - **Folder:** `/ (root)`

5. Guardar.

GitHub publicará la página en una dirección de la forma:

```text
https://TU-USUARIO.github.io/piramide/
```

## Funcionamiento

El solver corre completamente en el navegador.

No envía los colores ingresados a ningún servidor.

A partir de la configuración cargada, reconstruye el estado del rompecabezas y busca una secuencia de movimientos que lo lleve al estado resuelto.

## Referencia

La convención de movimientos y la estructura del procedimiento están basadas en la guía oficial de solución del Rubik's Pyramid.

## Licencia

Este repositorio contiene únicamente el código del solver.  
Rubik's es una marca de sus respectivos propietarios.
