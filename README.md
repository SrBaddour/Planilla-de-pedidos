# Pedidos — cliente petrolero (Grupo GomJK)

Página estática para registrar pedidos y checklist de entregas. Sin servidor propio: se puede publicar con **GitHub Pages**.

## Publicar en línea (GitHub Pages)

1. Crea un repositorio vacío en GitHub (por ejemplo `pedidos-petrolero-web`).
2. En tu PC, dentro de esta carpeta:

```bash
git remote add origin https://github.com/TU_USUARIO/pedidos-petrolero-web.git
git branch -M main
git push -u origin main
```

3. En GitHub: **Settings → Pages → Build and deployment → Source** → **Deploy from a branch**. Rama **main**, carpeta **/ (root)**. Guarda.
4. Tras el despliegue, la web quedará en una URL del tipo:

`https://TU_USUARIO.github.io/pedidos-petrolero-web/`

Comparte esa URL con tu cliente.

## Nota sobre los datos

Cada persona guarda los datos **en su propio navegador** (no en el servidor). Para respaldos o compartir, usen **Exportar CSV**. Si más adelante necesitan un único listado compartido en tiempo real, habría que añadir backend o una hoja de cálculo conectada.
