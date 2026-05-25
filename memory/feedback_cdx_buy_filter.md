---
name: Filtro CDX para BUY — Al menos 1min o 5min Bullish
description: BUY no válido si CDX es 100% Bearish en todos los TF, incluso si RSI 3m ambos >50
type: feedback
---
Para que un BUY sea válido en macro bajista, **al menos el CDX de 1min o 5min debe estar Bullish**.

**Why:** Si CDX es 100% Bearish en todos los timeframes (1min, 5min, 15min, 1h, 4h), no hay momentum alcista suficiente para sostener el move. El precio rebota brevemente y vuelve a caer.

**How to apply:**
- Antes de confirmar ✅ TRADE BUY → revisar CDX
- Si CDX 1min o 5min = Bullish → BUY puede proceder
- Si CDX 100% Bearish (todos los TF) → ❌ NO TRADE / ⏸ ESPERAR aunque RSI 3m ambos >50
- Esta advertencia SIEMPRE debe aparecer en la sección 🚦 Decisión cuando CDX no acompañe la dirección del trade
- En macro bajista: el BUY es un rebote técnico — necesita al menos señal mínima de momentum en TF cortos (1min/5min)
