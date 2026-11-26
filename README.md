# HGW Business Game — Academia interactiva

Aplicación educativa web para aprender el plan de compensación de HGW Bolivia a partir del **Catálogo HGW Bolivia, enero de 2026**.

## Requisitos
- Node.js 18 o superior
- npm

## Ejecutar localmente
```bash
npm install
npm run dev
```
Abre la URL que indique Vite (normalmente http://localhost:5173).

## Crear versión de producción
```bash
npm run build
npm run preview
```
La carpeta `dist/` contiene el sitio listo para publicar.

## Publicar en GitHub y Vercel
1. Crea un repositorio nuevo en GitHub.
2. Sube todos los archivos de esta carpeta (incluidos `package.json`, `index.html`, `src/`, `vercel.json` y `.gitignore`).
3. En Vercel, selecciona **Add New → Project** y conecta ese repositorio.
4. Vercel detecta Vite. Comprueba estos valores:
   - Framework Preset: Vite
   - Build Command: `npm run build`
   - Output Directory: `dist`
   - Install Command: `npm install`
5. Pulsa **Deploy**. Para futuras actualizaciones, sube los cambios a GitHub y Vercel volverá a desplegar.

## Características
- Aplicación React + Vite, sin backend ni credenciales.
- Diseño responsive para móviles, tablets y escritorio.
- Ocho mundos de aprendizaje, navegación interactiva y progreso guardado en el dispositivo con `localStorage`.
- Carrusel de productos de muestra, simuladores, calculadoras, examen final, puntos y celebración sonora opcional.
- Sonido sintetizado con Web Audio API (se activa al completar misiones y puede silenciarse).
- Configuración SPA para Vercel mediante `vercel.json`.

## Alcance y precisión
- El juego no afilia personas, no procesa pedidos ni liquida comisiones.
- Los BV no se convierten automáticamente a bolivianos. El catálogo indica que el factor BV/moneda puede ser revisado anualmente.
- La matriz del Bono de Desarrollo se presenta literalmente como aparece en el catálogo; no se inventa un factor ni se presume su orientación.
- La lista de productos es una muestra pedagógica. Precios y BV por producto deben actualizarse desde la lista vigente de HGW.
- Para liquidación real prevalece el Manual de Pago de Compensaciones y la documentación oficial vigente.

## Personalización
- Colores principales: verde bosque `#064b32`, verde HGW `#087448`, verde `#39b54a`, lima `#8cc63f`, blanco y fondos verde muy claro.
- Punto de entrada: `src/main.jsx`.
- Estilos responsive: `src/style.css`.


## Novedades de la versión 2.1

- Examen final de una pregunta por pantalla, con avance y desplazamiento automático a la siguiente pregunta.
- Botón para reiniciar el examen y botón para borrar el progreso e iniciar toda la experiencia desde cero.
- Reporte de resultados con puntos, avance, mundos completados y calificación, listo para copiar y pegar en WhatsApp.
- Diseño responsive reforzado para pantallas pequeñas.
- Ficha didáctica del producto real Ganoderma Plus (código 0003), con presentación, uso descrito, dosis y advertencias transcritas del catálogo HGW Bolivia, enero de 2026. La composición no se inventa cuando no está detallada en la ficha.

Para actualizar un repositorio existente, reemplaza los archivos del proyecto por el contenido de esta versión y realiza un nuevo commit. Vercel desplegará la actualización al detectar el commit.
