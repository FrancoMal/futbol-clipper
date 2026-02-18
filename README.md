# ⚽ Fútbol Clipper

Webapp para marcar timestamps de jugadores durante partidos de fútbol.

## 🌐 Uso Online

**https://francomal.github.io/futbol-clipper/**

## 📱 Uso

1. Crear un nuevo partido
2. Agregar los jugadores a seguir
3. Durante el partido:
   - Usar el reloj con SYNC para mantener el tiempo correcto
   - Cambiar entre 1T y 2T
   - Tocar el botón de cada jugador para marcar intervalos
   - Agregar etiquetas (Gol, Asistencia, etc.)
4. Exportar el JSON para usar con el Compilador

## ⏱️ Formatos de Tiempo

- **Standard**: 1T (00:00-45:00), 2T (00:00-45:00)
- **90min**: 1T (00:00-45:00), 2T (45:00-90:00)

## 📤 Export

Genera un JSON con:
```json
{
  "match": "Boca vs River",
  "date": "2026-02-17",
  "appVersion": "1.1",
  "players": [
    {
      "name": "Enzo Fernández",
      "intervals": [
        {"id": 1, "half": 1, "start": "12:30", "end": "12:58", "tags": [{"text": "Gol", "color": "#2ecc71"}]}
      ]
    }
  ]
}
```

## 🔗 Compilador

Para convertir los timestamps en videos compilados, usá el **[Fútbol Compilador](https://github.com/FrancoMal/futbol-compilador)**.

## 💾 Datos

Los datos se guardan automáticamente en localStorage del navegador.

---
**v1.1** - Edit timestamps, Tags, 90min format
