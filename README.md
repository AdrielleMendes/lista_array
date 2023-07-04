from estrutura_elementar import estrutura_elementar


class ArrayList(estrutura_elementar):
    def __init__(self):
        self.elemento=[]
        pass

    def esta_vazio(self) -> bool:
        if len(self.elemento)==0:
            return True
        else:
           return False

    def inserir(self, item):
        self.elemento.append(item)
        pass

    def remove(self, item):
        if item in self.elemento(item):
            self.elemento.remove(item)

    def tamanho(self) -> int:
        if len(self.elemento):
            return 1
        

    def limpa(self):
        self.elemento=[]
        pass

    def procura(self, item) -> bool:
        if item in self.elemento:
            return True
        else:
           return False

    def indice_de(self, item):
        if item in self.elemento:
            return self.elemento.index(item)
        else:
           return 1

    def recupera_indice(self, index):
        if 0 <= index <len(self.elemento):
            return self.elemento[index]
        else:
            return 1
