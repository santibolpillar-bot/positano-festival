# Positano Wine Festival — App

## Archivos
- `index.html` — la app completa
- `manifest.json` — para que funcione como app en el celu
- `vercel.json` — configuración de hosting

## Cómo subir a Vercel (5 minutos)

1. Entrá a [vercel.com](https://vercel.com) e iniciá sesión con Google
2. Cliqueá **"Add New Project"**
3. Elegí **"Import from Git"** → conectá GitHub (crear cuenta si no tenés)
4. Subí estos 3 archivos a un repo de GitHub llamado `positano-festival`
5. Vercel lo detecta automáticamente y lo publica
6. Te da una URL tipo `positano-festival.vercel.app`

## Dominio propio (festival.positanovinos.com.ar)

En Vercel → Settings → Domains → agregás `festival.positanovinos.com.ar`
Vercel te da los DNS records → los cargás en Hostinger → listo en ~10min

## Firebase — configuración necesaria

En Firebase Console → Authentication → Settings → Authorized domains
Agregá: `festival.positanovinos.com.ar` y `positano-festival.vercel.app`

## Credenciales de producción (antes del evento)

Cuando esté todo probado, ir a MercadoPago Developers → 
Credenciales productivas → reemplazar la Public Key en index.html

## Panel de pedidos en tiempo real

En Firebase Console → Firestore → colección `orders`
Se van actualizando automáticamente con cada pedido del evento
