# Calculadora de IMC

Aplicación Android desarrollada para la práctica **BMI Calculator Jetpack Compose**.

## Ramas del proyecto

El proyecto conserva dos versiones de la interfaz en ramas distintas:

- [`main`](https://github.com/ojaafar/IMCA2/tree/main): diseño inicial trabajado en clase.
- [`ui`](https://github.com/ojaafar/IMCA2/tree/ui): diseño mejorado, colores y una presentación más visual del resultado.

Este README y la captura corresponden a la versión de la rama **`ui`**.

## ¿Qué hace la aplicación?

Permite escribir un nombre, modificar el peso mediante los botones **−** y **+**, seleccionar la altura con una barra deslizante y calcular el índice de masa corporal (IMC).

Al pulsar **Calcular IMC**, muestra una tarjeta con el nombre, el resultado con un decimal y la categoría correspondiente. Si el nombre se deja vacío, utiliza el texto **Resultado**.

## Funcionamiento

1. Introducir el nombre (opcional).
2. Ajustar el peso en kilogramos. Los controles permiten valores entre 20 y 300 kg.
3. Seleccionar la altura en centímetros.
4. Pulsar **Calcular IMC**.
5. Consultar el resultado en la tarjeta inferior. La pantalla permite desplazarse para acceder a todo el contenido.

La altura se convierte a metros antes del cálculo:

```text
IMC = peso en kg / (altura en metros × altura en metros)
```

Por ejemplo, con 80 kg y 180 cm, el resultado mostrado es aproximadamente 24,7.

## Tecnologías utilizadas

- **Kotlin** para la lógica y el cálculo.
- **Jetpack Compose** para crear la interfaz mediante funciones composables.
- **Material 3** para los componentes visuales.
- **Android Studio y Gradle** para desarrollar y compilar el proyecto.

## Archivos principales

- `app/src/main/java/org/insbaixcamp/imca/MainActivity.kt`: pantalla, estado de los controles, cálculo y resultado.
- `app/src/main/java/org/insbaixcamp/imca/ui/theme/`: colores, tipografía y tema visual.

## Cómo ejecutar el proyecto

1. Clonar el repositorio y seleccionar la rama **`ui`**, o descargar el ZIP desde esa rama y descomprimirlo.
2. Abrir la carpeta principal del proyecto con Android Studio.
3. Esperar a que termine la sincronización de Gradle e instalar los componentes del SDK que solicite el proyecto.
4. Seleccionar un emulador o dispositivo Android compatible.
5. Pulsar **Run**.

## Captura de pantalla

![Interfaz de la calculadora de IMC mostrando un resultado](docs/captura.png)
![Interfaz de la calculadora de IMC mostrando un resultado](docs/captura1.png)

## Autor

Ousama
