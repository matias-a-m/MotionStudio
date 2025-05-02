# MotionStudio

**Laboratorio de animaciones nativas, microinteracciones y feedback háptico.**

`MotionStudio` es un espacio de experimentación visual. Permite validar, comparar e iterar microinteracciones con SwiftUI y UIKit. Ideal para explorar gestos, transiciones, curvas de animación y efectos hápticos en un entorno desacoplado del producto final.

---

## Propósito

- Validar patrones de animación en interfaces reales.
- Experimentar con gestos, transiciones y respuesta táctil.
- Documentar decisiones visuales a través del código.
- Servir como base para definir estándares visuales del producto.

---

## Contenido

- Ejemplos de animaciones contextuales.
- Pruebas de respuesta háptica (`UIFeedbackGenerator`).
- Microinteracciones específicas de UI.
- Transiciones entre vistas controladas.
- Implementaciones en SwiftUI y UIKit.

---

## Pruebas

El módulo incluye pruebas automáticas para:

| Componente              | Tipo de prueba              |
|------------------------|-----------------------------|
| Transiciones           | Snapshot + validación lógica|
| Gestos                 | Unitarias (condicionales)   |
| Feedback háptico       | Unitarias                   |

```swift
func testHapticFeedbackGenerator() {
    let feedback = HapticEngine.preview()
    XCTAssertNotNil(feedback)
}
```

---

## Integración

Este módulo se visualiza e integra desde `ProductSuiteApp`. No se exporta como framework reutilizable, sino como espacio de exploración visual controlada.

---

## Requisitos

- iOS 15+
- Swift 6
- Swift Package Manager

---

## Licencia

MIT © Matías Adrián Molina
