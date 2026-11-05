# BOM — Brazo robótico

Medidas tomadas en vivo del modelo de Fusion 360 (API interna en cm,
convertidas a mm). Volumen de sólidos B-Rep; masa estimada con acero
7.85 g/cm³ salvo servos comerciales.

| # | Pieza | Cant. | Envolvente (mm) | Vol. unit. (cm³) | Masa est. (g) | Función aparente |
|---|---|---|---|---|---|---|
| 1 | S1M | 1 | 358 × 355 × 81 | 2653.4 | 20830 | placa base |
| 2 | MB1M | 1 | 176 × 102 × 43 | — (malla) | — | torreta de base |
| 3 | MB1R | 1 | 73 × 74 × 12 | 8.6 | 68 | anillo de giro |
| 4 | MB2M | 1 | 4 × 114 × 81 | 18.8 | 148 | placa soporte |
| 5 | MB4M | 1 | 28 × 52 × 82 | — (malla) | — | escuadra perforada |
| 6 | B1 | 1 | 90 × 51 × 45 | 23.3 | 183 | balancín hombro |
| 7 | B2 | 1 | 90 × 51 × 45 | 27.4 | 215 | balancín hombro |
| 8 | M1 | 1 | 131 × 40 × 32 | 34.5 | 271 | eslabón codo |
| 9 | M2 | 1 | 131 × 40 × 32 | 45.7 | 359 | eslabón codo |
| 10 | F1 | 1 | 118 × 70 × 32 | 32.9 | 258 | palma de garra |
| 11 | F2 | 1 | 118 × 70 × 27 | 30.3 | 238 | horquilla muñeca |
| 12 | G1M | 1 | 56 × 30 × 33 | 26.3 | 206 | tambor guía |
| 13 | G2M | 1 | 2 × 26 × 45 | 1.6 | 13 | placa guía |
| 14 | G3M | 2 | 27 × 30 × 13 | 4.6 | 36 | canal en U |
| 15 | GEAR | 2 | Ø23 × 2 | 0.7 | 5 | engrane de garra |
| 16 | mg996R | 4 | 60 × 21 × 44 | ~31.6 | ~55 c/u | servos (Tower Pro MG996R) |
| 17 | mg996_arm_4pad | 1 | 40 × 40 × 6 | 1.2 | 9 | cuerno servo en X |
| 18 | mg996_arm_round | 3 | Ø21 × 6 | 0.9 | 7 | cuerno servo redondo |
| 19 | SG90 | 1 | 37 × 32 × 17 | malla | ~9 | micro servo garra |

Notas:

- `mg996R` es un ensamble comercial de 11 cuerpos (carcasa, engranes,
  cuerno); la masa real del servo es ~55 g.
- `SG90` y `MB1M`/`MB4M` vienen como malla o superficie: sin volumen
  sólido computable.
- Faltantes históricos del proyecto (no incluidos): `mg996R_v2`,
  `mg996_arm_6pad`, `GEAR_2`, `MB3M`.
