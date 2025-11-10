# Ejercicio de Repaso: Semáforo para Parking

Este proyecto simula un sistema de control de acceso a un parking mediante semáforos, gestionando la entrada, salida y espera de coches. Se utiliza programación concurrente y sincronización mediante semáforos para garantizar que solo un número limitado de coches pueda acceder simultáneamente, evitando sobrepasar la capacidad máxima del parking.

## Descripción

El objetivo del ejercicio es practicar la sincronización de hilos/procesos utilizando semáforos. El sistema simula:

- **Entrada**: Los coches intentan acceder al parking. Si hay plazas disponibles, el semáforo permite el paso.
- **Espera**: Si el parking está lleno, los coches esperan hasta que haya sitio disponible.
- **Salida**: Los coches salen liberando plazas, permitiendo que otros coches entren.

Esta simulación es útil para comprender los conceptos de sección crítica, exclusión mutua y sincronización en programación concurrente.

## Características

- Gestión del acceso concurrente a un recurso limitado (las plazas del parking).
- Uso de semáforos para controlar entrada, salida y espera.
- Permite modificar fácilmente la capacidad máxima del parking y el número de coches.
- Código comentado orientado al aprendizaje.

## Instalación

1. Clona el repositorio:
    ```bash
    git clone https://github.com/tu-usuario/tu-repo.git
    cd tu-repo
    ```
2. Asegúrate de tener instalado el compilador/intérprete adecuado (por ejemplo, `gcc` para C, `python` para Python, etc.).

## Uso

Ejecuta el simulador. Por ejemplo, en C:
```bash
gcc parking_semaforo.c -o parking_semaforo -lpthread
./parking_semaforo
```

En Python:
```bash
python parking_semaforo.py
```

## Dependencias

- **C**: Compilador con soporte para POSIX y la librería pthread.
- **Python**: Python 3.x (requiere el módulo `threading` estándar).

## Ejemplo de funcionamiento

```
Coche 1 intenta entrar... Plaza disponible, accede al parking.
Coche 2 intenta entrar... Parking lleno, espera.
Coche 1 sale del parking. Plaza liberada.
Coche 2 accede al parking.
```
