---
name: Zonas críticas RSI Purple — Límites de entrada
description: Si Purple ya está en zona extrema (< 35 SELL / > 65 BUY) es riesgo; si llega a < 30 / > 70 es agotamiento y NO se entra.
type: feedback
---

El nivel del Purple RSI al momento del análisis determina si el momentum está fresco o consumido. **No basta con que Purple < Yellow y ambos < 50 para SELL — el nivel absoluto de Purple también importa.**

## Zonas de RSI Purple

### Para SELL
| Nivel Purple | Estado | Acción |
|---|---|---|
| 50 → 35 | ✅ Momentum activo | Entrada válida si RSI confirma |
| 35 → 30 | ⚠️ Zona de riesgo | Esperar reset: Purple retorne a ~45 |
| < 30 | ❌ Agotamiento bajista | NO TRADE — movimiento consumido |

### Para BUY
| Nivel Purple | Estado | Acción |
|---|---|---|
| 50 → 65 | ✅ Momentum activo | Entrada válida si RSI confirma |
| 65 → 70 | ⚠️ Zona de riesgo | Esperar reset: Purple retorne a ~55 |
| > 70 | ❌ Agotamiento alcista | NO TRADE — movimiento consumido |

## En la condición de entrada (✅ Entrar X solo cuando)

SIEMPRE describir el **comportamiento RSI esperado**, NO un nivel de precio:
- "RSI 3m: Yellow cruza bajo 50 junto con Purple (Patrón 1)"
- "RSI 3m: Purple retorne a ~45 con Yellow < Purple y ambos < 50"
- "RSI 3m: Yellow haga reset sobre 50 y vuelva a caer bajo 50 (Patrón 2 completado)"

**NUNCA** poner "cuando precio llegue al FVG ~X,XXX" como condición de entrada.

**Why:** En el trade del 23-May-2026 (MGC SELL NY), el Purple ya estaba en ~33 — técnicamente cumplía la regla pero el momentum ya estaba consumido. Resultado: -$200.80.

**How to apply:** Antes de indicar ✅ TRADE o ⏸ ESPERAR, verificar el nivel absoluto de Purple. Si está fuera de la zona activa, marcar como zona de riesgo y cambiar la condición de entrada a "Purple retorne a ~45/55".
