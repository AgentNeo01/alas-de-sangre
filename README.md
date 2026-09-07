# 🐉 Alas de Sangre — Portal de Campaña

Sitio web (estático) de la campaña de D&D 5e **Alas de Sangre**, ambientada en el Colegio de Guerra de Basgiath. Pensado para publicarse **gratis en GitHub Pages** y compartir un solo enlace con los jugadores.

Material de aficionado, sin fines de lucro. No oficial. Universo de *Fourth Wing* de Rebecca Yarros.

## Contenido
```
campaign-site/
├─ index.html          → la web (una sola página)
├─ assets/
│  ├─ img/             → retratos de PNJ (player-safe)
│  └─ pdf/             → Libro del Jugador y fichas imprimibles
└─ README.md
```
> El sitio es **player-safe**: no incluye spoilers (nada de venin, ni de que Corvin es un cebo, ni fichas de combate).

---

## 🚀 Cómo publicarlo GRATIS en GitHub Pages

### Opción A — sin tocar la terminal (la más fácil)
1. Crea una cuenta en **github.com** (gratis).
2. Botón **New repository** → nombre p. ej. `alas-de-sangre` → **Public** → Create.
3. En el repo: **Add file → Upload files** → arrastra TODO el contenido de la carpeta `campaign-site/` (el `index.html` debe quedar en la raíz del repo) → **Commit**.
4. **Settings → Pages** → en *Branch* elige `main` y carpeta `/root` → **Save**.
5. Espera 1-2 min. Tu web estará en:
   `https://TU-USUARIO.github.io/alas-de-sangre/`
6. Pega ese enlace en `#bienvenida` de tu Discord. ¡Listo!

### Opción B — con Git (para versionar todo)
```bash
cd campaign-site
git init
git add .
git commit -m "Portal de campaña Alas de Sangre"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/alas-de-sangre.git
git push -u origin main
```
Luego activa **Settings → Pages → Branch: main /root**.

---

## ✍️ Cómo actualizarlo tras cada sesión
- Abre `index.html`, busca la sección `id="recaps"` y añade un bloque `<div class="recap">` nuevo con el resumen de la sesión.
- Sube el cambio (Upload files o `git commit && git push`). La web se actualiza sola en ~1 min.

## 🔒 Nota de privacidad
Si prefieres que la web NO sea pública en buscadores, puedes hacer el repo **privado** y usar el enlace solo con tu grupo (GitHub Pages en repos privados requiere plan de pago; para gratis, mantenlo público — al no estar enlazado en ningún sitio, es prácticamente invisible salvo para quien tenga el link).
