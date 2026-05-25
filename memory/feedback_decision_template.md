---
name: Template OBLIGATORIO — Sección 🚦 Decisión actual
description: Formato compacto y estructurado que SIEMPRE se debe usar en la sección 🚦 Decisión de cada análisis Duck FVG
type: feedback
---
La sección **🚦 Decisión actual** SIEMPRE debe seguir este template exacto.

**Why:** La usuaria valora la concisión y claridad operativa. Este template integra todos los filtros críticos (CDX, RSI 3m, Patrón 1 vs 2) en formato escaneable de un vistazo.

---

## TEMPLATE OBLIGATORIO

```
🚦 Decisión: ⏸ ESPERAR / ✅ TRADE / ❌ NO TRADE

El Escenario [A/B] [BUY/SELL] es el de mayor probabilidad por [razón breve], pero hay dos filtros que deben cumplirse antes de entrar:

1️⃣ Filtro CDX — [✅/⚠️/❌] [Estado actual]. Para [BUY/SELL] válido se necesita que [condición CDX].

2️⃣ Filtro RSI 3m — [✅/⚠️/❌] [Patrón 1 o Patrón 2 + valores purple/yellow].

✅ Entrar [BUY/SELL] solo cuando:
1. [Condición CDX específica]
2. [Comportamiento RSI 3m esperado — NO usar niveles de precio, sino el estado del RSI]
   - Patrón 1 limpio: "RSI 3m: Yellow cruza [bajo/sobre] 50 junto con Purple"
   - Purple extendido (35–45 SELL / 55–65 BUY): "RSI 3m: Purple retorne a [45/55]"
   - Patrón 2: "RSI 3m: Yellow haga reset y vuelva a cruzar 50 con Purple"

⚠️ ZONA DE RIESGO RSI Purple: Si Purple < 35 (SELL) o > 65 (BUY) → zona de riesgo.
Si Purple < 30 o > 70 → agotamiento, NO entrar.

TP 1: ~[nivel] | TP 2: ~[nivel] 🐤
```

---

## REGLAS

1. **Máximo 2 filtros numerados** (CDX + RSI 3m)
2. **Siempre identificar Patrón 1 vs Patrón 2**
3. **Siempre 2 condiciones de entrada** en "✅ Entrar X solo cuando"
4. **TPs siempre al final**, separados por `|`, terminando con 🐤
5. **Si es ✅ TRADE**: omitir filtros, dar entrada/stop/TPs directamente
6. **Si es ❌ NO TRADE**: omitir condiciones de entrada, explicar por qué

---

## EJEMPLO — Patrón 2 / ESPERAR

```
🚦 Decisión: ⏸ ESPERAR

El Escenario A BUY es el de mayor probabilidad, pero hay dos filtros que deben cumplirse:

1️⃣ Filtro CDX — ⚠️ 100% Bearish. Para BUY válido se necesita que al menos CDX 1min o 5min gire Bullish.

2️⃣ Filtro RSI 3m — ⚠️ Patrón 2 (yellow ya está arriba de 50 en 56.93). Necesita reset bajo 50 primero.

✅ Entrar BUY solo cuando:
1. CDX 1min o 5min gira Bullish
2. RSI 3m: Yellow baja bajo 50, hace el reset, y vuelve a subir sobre 50 con Purple (Patrón 1 completado)

TP 1: ~4,533 | TP 2: ~4,546–4,549 🐤
```

---

## EJEMPLO — Purple en zona de riesgo

```
🚦 Decisión: ⏸ ESPERAR

El Escenario A SELL es el de mayor probabilidad, pero hay dos filtros que deben cumplirse:

1️⃣ Filtro CDX — ⚠️ Mixto (1m+5m Bullish, 15m+1h+4h Bearish). Para SELL válido se necesita que CDX 1min y 5min giren Bearish.

2️⃣ Filtro RSI 3m — ⚠️ Purple en zona extendida (~33). ZONA DE RIESGO: momentum bajista consumido. Esperar que Purple retorne a ~45.

✅ Entrar SELL solo cuando:
1. CDX 1min y 5min giran Bearish
2. RSI 3m: Purple retorne a ~45 Y Yellow siga por debajo de Purple (ambos < 50)

TP 1: ~4,510 | TP 2: ~4,492 🐤
```
