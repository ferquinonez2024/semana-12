# semana 12
 temperatura
# Definición de la matriz 3D con datos de temperaturas
temperaturas = [
    # Semana 1
    [
        # Ciudad 1
        [25, 26, 24, 23, 22, 24, 25],  # Temperaturas de lunes a domingo
        # Ciudad 2
        [27, 28, 26, 25, 24, 26, 27],
        # ... Otras ciudades
    ],
    # Semana 2
    [
        # Ciudad 1
        [26, 27, 25, 24, 23, 25, 26],
        # Ciudad 2
        [28, 29, 27, 26, 25, 27, 28],
        # ... Otras ciudades
    ],
    # ... Otras semanas
]

# Calcular el promedio de temperaturas por ciudad y semana
for semana, datos_semana in enumerate(temperaturas, start=1):
    print(f"Semana {semana}:")
    for ciudad, datos_ciudad in enumerate(datos_semana, start=1):
        promedio_temperaturas = sum(datos_ciudad) / len(datos_ciudad)
        print(f"  Ciudad {ciudad}: Promedio = {promedio_temperaturas:.2f}")
