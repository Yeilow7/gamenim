# Nim Game - Python AI

Este proyecto es una implementación del juego de **Nim** en **Python**, en el cual un jugador humano puede enfrentarse a una **IA** entrenada mediante **aprendizaje por refuerzo**. El objetivo del juego es evitar ser el jugador que tome el último objeto de las pilas.

## Características

- Juego de **Nim** para dos jugadores: uno humano y uno controlado por IA.
- La IA utiliza un modelo entrenado con **aprendizaje por refuerzo** para tomar decisiones óptimas.
- Posibilidad de entrenar la IA en nuevas partidas.
- Interfaz basada en la consola.

## Requisitos

- Python 3.x

## Archivos del proyecto

- `nim.py`: Contiene la lógica del juego y la implementación del **aprendizaje por refuerzo** para entrenar la IA.
- `play.py`: Permite ejecutar el juego entre el humano y la IA entrenada.

## Instalación

1. Clona este repositorio:

    ```bash
    git clone https://github.com/tu-usuario/nim-ai.git
    ```

2. Navega al directorio del proyecto:

    ```bash
    cd nim-ai
    ```

## Cómo entrenar a la IA

Antes de jugar, puedes entrenar a la IA para mejorar su rendimiento en el juego. Esto ya está implementado en el archivo `play.py`.

1. El código en `play.py` entrena a la IA durante 20,000 juegos simulados antes de que comience la partida entre el humano y la IA. Puedes ajustar este número cambiando la llamada a la función `train()`:

    ```python
    ai = train(20000)  # Cambia 20000 por el número de juegos de entrenamiento que desees.
    ```

2. Para entrenar a la IA, simplemente ejecuta el siguiente comando:

    ```bash
    python3 play.py
    ```

## Cómo jugar

1. Después de entrenar a la IA, el juego comenzará automáticamente. Verás el estado actual de las pilas y te indicará cuándo es tu turno.
2. Elige una pila y la cantidad de objetos que deseas retirar. El formato de entrada será:

    ```bash
    Choose Pile: [número de pila]
    Choose Count: [número de objetos a retirar]
    ```

3. La IA tomará su turno automáticamente después de que completes el tuyo.
4. El juego continuará hasta que uno de los jugadores sea forzado a tomar el último objeto, momento en el que ese jugador perderá.

## Ejecución

Para jugar contra la IA, simplemente ejecuta el siguiente comando:

```bash
python3 play.py
