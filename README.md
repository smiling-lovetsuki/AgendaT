# Inicializa una lista vacía donde se almacenarán las tareas
agenda = []

# Función para agregar una tarea a la agenda
def agregar_tarea(fecha, hora, descripcion, prioridad):
    tarea = {
        "fecha": fecha,
        "hora": hora,
        "descripcion": descripcion,
        "prioridad": prioridad
    }
    agenda.append(tarea)

# Función para mostrar todas las tareas en la agenda
def mostrar_agenda():
    if not agenda:
        print("La agenda está vacía.")
    else:
        for tarea in agenda:
            print(f"Fecha: {tarea['fecha']}, Hora: {tarea['hora']}, Descripción: {tarea['descripcion']}, Prioridad: {tarea['prioridad']}")
