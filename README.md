# Planilla de pedidos — cliente petrolero (Grupo GomJK)

Repositorio: [SrBaddour/Planilla-de-pedidos](https://github.com/SrBaddour/Planilla-de-pedidos)

## Despliegue automático

Cada `git push` a la rama **main** ejecuta [GitHub Actions](https://github.com/SrBaddour/Planilla-de-pedidos/actions) y actualiza la rama **gh-pages** con `index.html`.

## URL para compartir con el cliente

### Opción A — GitHub Pages (recomendada, dominio propio de GitHub)

Solo hay que activarlo **una vez** en el repositorio:

1. Abre [Settings → Pages](https://github.com/SrBaddour/Planilla-de-pedidos/settings/pages).
2. En **Build and deployment → Source**, elige **Deploy from a branch**.
3. Rama **gh-pages**, carpeta **/ (root)** → **Save**.

En uno o dos minutos la planilla quedará en:

**https://srbaddour.github.io/Planilla-de-pedidos/**

### Opción B — Enlace inmediato (sin tocar Settings)

Mientras tanto puedes usar la copia servida por jsDelivr (misma página):

**https://cdn.jsdelivr.net/gh/SrBaddour/Planilla-de-pedidos@gh-pages/index.html**

*(Tras cada cambio en `main`, espera a que termine el workflow y, si hace falta, purga caché en [jsdelivr purge](https://www.jsdelivr.com/github) si no ves la última versión al instante.)*

### Activar Pages desde la terminal (alternativa)

Si tienes [GitHub CLI](https://cli.github.com/) y ya hiciste `gh auth login`:

```bash
gh api -X PUT repos/SrBaddour/Planilla-de-pedidos/pages -f source[branch]=gh-pages -f source[path]=/
```

## Nota sobre los datos

Cada usuario guarda los datos **en su navegador**. Para respaldos o compartir, usen **Exportar CSV**.
