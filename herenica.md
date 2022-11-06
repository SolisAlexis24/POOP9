@startuml

class Animal{
    -nombre: String
    -lugarOrigen: String
    -color: String
    +sonido(string): void
    +comer(): void
}

class AnimalAcuatico{
    -numAletas: int
    +nadar(): void
    +comer(): void
}

class AnimalTerrestre{
    -numPatas: int
    +correr(): void
    +comer(): void
}

class AnimalAereo{
    -numAlas: int
    +volar(): void
    +comer(): void
}

class Ballena{
    -largo: int
    +pelearConPinocho(): void
}

class Perro{
    -colorCollar: String
    +hacerTrucos(): void
}

class Pajaro{
    -tipoPico: String
    +recolectarRamas(): void
}

Animal <|-- AnimalAcuatico
Animal <|-- AnimalTerrestre
Animal <|-- AnimalAereo
AnimalAcuatico <|-- Ballena
AnimalTerrestre <|-- Perro
AnimalAereo <|-- Pajaro

@enduml