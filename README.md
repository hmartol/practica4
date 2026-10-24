# Práctica 4: Gestión Avanzada de Ramas y Resolución de Conflictos

**Hugo Martín Toledano - 2º DAW**

---

# Fase base

He creado el proyecto WebNova, iniciado el repositorio y realizado el primer commit.

![Fase base](capturas/1.png)

Así quedó el `index.html` inicial.

![Index inicial](capturas/2.png)

---

# Parte 1: Desarrollo en paralelo

He creado las ramas `cabecera`, `contenido` y `pie` a partir de `main`.

![Creación de ramas](capturas/3.png)

## Rama cabecera

He creado `header.html` y guardado el cambio en C2.

![Header](capturas/4.png)

![Commit C2](capturas/5.png)

## Rama contenido

He creado `content.html` y guardado el cambio en C3.

![Contenido](capturas/6.png)

![Commit C3](capturas/7.png)

## Rama pie

He creado `footer.html` y guardado el cambio en C4.

![Footer](capturas/8.png)

![Commit C4](capturas/9.png)

---

# Parte 2: Integración

He vuelto a `main` y he unido las tres ramas.

![Fusión de las ramas](capturas/10.png)

Después he juntado todo el contenido dentro de `index.html`.

![Index completo](capturas/11.png)

He creado C5 y eliminado las ramas que ya no hacían falta.

![Commit C5 y eliminación de ramas](capturas/12.png)

---

# Parte 3: Conflicto y resolución

He creado la rama `rediseño` y cambiado el título principal.

![Título en rediseño](capturas/13.png)

![Rama rediseño](capturas/14.png)

He guardado el cambio en C6.

![Commit C6](capturas/15.png)

Después he vuelto a `main` y cambiado la misma línea de otra forma.

![Título en main](capturas/16.png)

![Commit C7](capturas/17.png)

Al intentar unir `rediseño` con `main`, apareció un conflicto.

![Conflicto](capturas/18.png)

En `index.html` aparecieron las dos versiones del título.

![Marcas del conflicto](capturas/19.png)

He unido las dos ideas y dejado el título definitivo.

![Conflicto resuelto](capturas/20.png)

Después he guardado la solución en C8.

![Commit C8](capturas/21.png)

---

# Parte 4: Historial

Este es el historial final de ramas y cambios de la práctica.

![Historial final](capturas/22.png)

---

# Reflexión teórica

## ¿Por qué ocurrió el conflicto en la Parte 3 y no en la Parte 2?

En la Parte 2 cada rama trabajaba con archivos diferentes, así que Git pudo unirlas, pero en la Parte 3, `main` y `rediseño` cambiaron la misma línea de `index.html` de formas diferentes, por eso apareció el conflicto.

## ¿Qué ocurrió con los archivos al ejecutar `git switch main`?

Al volver a `main`, los archivos cambiaron a la versión que tenía guardada esa rama. El cambio que había hecho en `rediseño` dejó de aparecer hasta que las ramas se unieron.