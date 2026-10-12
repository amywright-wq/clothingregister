# Paddock Yield Estimator

Estimates wheat, barley and lentil grain yield (t/ha and bags/ac) from paddock counts:

    yield (t/ha) = heads/m² × grains/head × thousand grain weight (g) ÷ 100,000

less any harvest loss allowance. Tests are averaged per paddock, saved paddocks give a farm total,
and everything is stored on the device.

## Offline use

The app is a small installable web app (`manifest.webmanifest` + `sw.js`). Once hosted over HTTPS
(e.g. GitHub Pages) and opened once with signal, it works with no connection.

- **iPhone:** open it in Safari → Share → **Add to Home Screen**.
- **Android:** open it in Chrome → ⋮ menu → **Add to Home screen** / **Install app**.

When you change any file, bump `VERSION` in `sw.js` so installed copies pick up the update.
