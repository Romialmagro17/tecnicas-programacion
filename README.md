# tecnicas-programacion
from abc import ABC, abstractmethod

class Vehiculo(ABC):
    @abstractmethod
    def encender(self):
        pass

    @abstractmethod
    def apagar(self):
        pass

class Coche(Vehiculo):
    def encender(self):
        print("El coche está encendido.")

    def apagar(self):
        print("El coche está apagado.")

# Uso
mi_coche = Coche()
mi_coche.encender()
mi_coche.apagar()
