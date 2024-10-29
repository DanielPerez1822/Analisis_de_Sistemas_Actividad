## Diagramas Comportamentales

## 1. Diagrama de Secuencia
```js
@startuml
actor Usuario
participant "Carrito" as C
participant "Producto" as P
participant "Factura" as F

Usuario -> C: agregarProducto(P, 2)
C -> P: consultarProducto()
Usuario -> C: modificarProducto(P, 3)
Usuario -> C: eliminarProducto(P)
Usuario -> C: generarFactura()
C -> F: crear()
@enduml
```
- **Explicación:** El diagrama de secuencia muestra la interacción temporal entre los objetos Usuario, Carrito, Producto y Factura durante el proceso de agregar, modificar, eliminar un producto en el carrito y generar una factura. Este diagrama es útil para entender el flujo de mensajes y la secuencia de eventos en el sistema.
![alt text](c:\Users\DANIEL\Desktop\Analisis_de_Sistemas\out\Diagrama_wsd\Diagramas_Dinamicos_wsd\Diagrama-1\Diagrama-1.png)