# PRIMER-TRABAJO
import math

class Circulo:
    def __init__(self, radio):
        self._radio = radio

    @property
    def radio(self):
        return self._radio

    @radio.setter
    def radio(self, valor):
        if valor < 0:
            raise ValueError("El radio no puede ser negativo")
        self._radio = valor

    def area(self):
        return math.pi * self._radio**2

    def perimetro(self):
        return 2 * math.pi * self._radio
