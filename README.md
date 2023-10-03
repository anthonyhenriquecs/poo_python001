# poo_python001

class Bicibleta:
    def __init__(self, cor, modelo, ano, valor):
        self.cor = cor
        self.modelo = modelo
        self.ano = ano
        self.valor = valor


    def buzinar(self):
        print("BUZINA")

    def parar(self):
        print("parando...")
    def correr(self):
        print("bicicleta correndo")


    #def __str__(self):
    #    return f"Bicicleta: cor={self.cor}, modelo={self.modelo}, ano={self.ano}, valor={self.valor}"

    def __str__(self):
        return f"{self.__class__.__name__}: {', '.join([f'{chave}={valor}' for chave, valor in self.__dict__.items()])}"
           
        
caloi = Bicibleta("vermelha", "caloi", 2022, 600)

caloi.buzinar()
caloi.correr()
caloi.parar

print(caloi)
