# 🐤 Pato Strategy — Duck FVG System

Repositorio de backup de la estrategia Duck FVG System para trading de MGC (Micro Gold) y MNQ (Micro Nasdaq).

## 📁 Estructura

```
/memory/          → Reglas y filtros del sistema (se cargan en Claude Cowork)
/indicators/      → Indicadores Pine Script para TradingView
```

---

## 🧠 Memory — Reglas del Sistema

| Archivo | Descripción |
|---|---|
| `feedback_decision_esperar.md` | Cuándo usar ⏸ ESPERAR vs ❌ NO TRADE |
| `feedback_rsi_ambos_50.md` | BUY/SELL válido solo si AMBOS RSI del mismo lado de 50 |
| `feedback_cdx_buy_filter.md` | BUY inválido si CDX 100% Bearish |
| `feedback_rsi_entry_quality.md` | Patrón 1 (alta prob) vs Patrón 2 (menor prob) |
| `feedback_decision_template.md` | Template obligatorio de la sección 🚦 Decisión |
| `feedback_rsi_purple_zones.md` | Zonas del Purple: activo / riesgo / agotamiento |

---

## 📊 Indicadores TradingView

### 🐤 RSI Zone Monitor (`DuckFVG_RSI_Zones.pine`)
Colorea el fondo del panel RSI según la zona del Purple:
- 🟢 Verde: zona activa (50→35 SELL / 50→65 BUY)
- 🟠 Naranja: zona de riesgo (35→30 / 65→70)
- 🔴 Rojo: agotamiento (<30 / >70) → NO TRADE

### 🐤 Gaussian 2m Color (`DuckFVG_Gaussian2m.pine`)
Muestra el color del Gaussian Channel de 2m en una tabla, sin cambiar de gráfico.

---

## 🔄 Cómo restaurar en una PC nueva

1. Instalar Claude Desktop + Cowork
2. Crear proyecto "Estrategia Pato Binns"
3. Copiar los archivos de `/memory/` a la carpeta de memoria de Claude:
   `AppData\Roaming\Claude\local-agent-mode-sessions\...\memory\`
4. Los indicadores `.pine` se importan directamente en TradingView (Pine Editor → Open → pegar código)
