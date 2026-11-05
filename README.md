# Brazo robótico articulado — Fusion 360

Brazo robótico de sobremesa diseñado en **Fusion 360**: base giratoria,
hombro y codo en paralelogramo, muñeca y garra de dos dedos,
accionado por 4 servos MG996R + 1 micro servo SG90.

## Estado

Ensamblaje funcional y verificado pieza por pieza desde la API de Fusion:
19 componentes, 28 cuerpos sólidos, 25 de 26 referencias externas sanas.
La referencia `MB3M` quedó colgante (el archivo de esa pieza no existe
en el proyecto); el resto del brazo está completo y articulado.

## Contenido

```text
brazo-robotico/
├── README.md
├── CAD/
│   ├── BrazoRobotico.f3d    # ensamble nativo de Fusion 360
│   └── BrazoRobotico.step   # intercambio CAD (12 MB, geometría completa)
└── docs/
    ├── render_ensamble.png  # vista del ensamble completo
    ├── despiece_piezas.png  # hoja de contacto de las piezas
    └── BOM.md               # lista de materiales con medidas reales
```

## Cómo abrirlo

- **Fusion 360:** abre `CAD/BrazoRobotico.f3d` (Archivo → Abrir).
- **Cualquier CAD:** importa `CAD/BrazoRobotico.step`.

## Cadena cinemática

Base S1M → torreta MB1M/MB1R (giro de base, MG996R n.º 1) →
balancines B1/B2 (hombro) → eslabones M1/M2 (codo, MG996R n.º 2 y 3) →
horquilla F2 + palma F1 (muñeca, MG996R n.º 4) →
garra con engranes G1M/G2M/G3M/GEAR y micro servo SG90.

## Piezas destacadas

| Pieza | Dimensiones (mm) | Volumen (cm³) | Función aparente |
|---|---|---|---|
| S1M | 358 × 355 × 81 | 2653.4 | placa base |
| MB1M | 176 × 102 × 43 | — | torreta de base |
| MB1R | 73 × 74 × 12 | 8.6 | anillo de giro |
| B1 / B2 | 90 × 51 × 45 | 23.3 / 27.4 | balancines de hombro |
| M1 / M2 | 131 × 40 × 32 | 34.5 / 45.7 | eslabones de codo |
| F1 | 118 × 70 × 32 | 32.9 | palma de garra |
| F2 | 118 × 70 × 27 | 30.3 | horquilla de muñeca |
| MG996R (×4) | 60 × 21 × 44 | ~31.6 c/u | servos principales |
| SG90 (×1) | 37 × 32 × 17 | malla | micro servo de garra |
| GEAR | Ø23 × 2 | 0.7 | engrane de garra |

Tabla completa con todas las piezas en [docs/BOM.md](docs/BOM.md).
Medidas tomadas en vivo del modelo (unidades de Fusion 360).
