
Portal Condesuyos - React + Vite (entrega inicial)

Instrucciones rápidas:
1. Instalar dependencias: npm install
2. Ejecutar en modo desarrollo: npm run dev (http://localhost:5173)
3. Para producción: npm run build y npm run preview

Contador de visitas (funciona en 2 modos):
- Modo A (recomendado): despliega la Cloud Function en Firebase (cloud_functions/index.js).
  1. npm i -g firebase-tools
  2. firebase login
  3. firebase init functions (elige Node.js 18+)
  4. Copia cloud_functions/index.js a functions/index.js
  5. firebase deploy --only functions
  6. Copia la URL y colócala en un archivo .env con VITE_VISIT_FN_URL=<URL>
- Modo B (fallback): sin función, el contador usa localStorage (demo).

Formulario de contacto:
- Reemplaza action en src/pages/Contacto.jsx por tu endpoint Formspree (https://formspree.io/f/XXXXX).
- Si no lo configuras, el formulario abrirá el cliente de correo como respaldo.

Logo integrado: public/logo_pc_horizontal.svg, public/logo_pc_icon.svg, public/logo_pc_favicon.svg

Repo / dominio:
- Nombre del repo sugerido: portalcondesuyos
- Para GitHub Pages o Vercel, sube todo el contenido del proyecto y configura variables de entorno (VITE_VISIT_FN_URL).

Si quieres que despliegue la función por ti en Vercel o genere los PNGs exportados, dime y lo hago.
