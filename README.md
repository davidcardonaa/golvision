# ⚽ Golvisión

Analizador de fútbol en una sola página (HTML, CSS y JavaScript, sin dependencias). Busca un equipo, abre su próximo partido y muestra probabilidades calculadas con un modelo de Poisson (Dixon-Coles simplificado).

## Qué hace

- Lista los partidos de ayer, hoy, mañana y pasado, agrupados por liga.
- Busca un equipo (por ejemplo, Atlético Nacional) y abre directamente su próximo partido con las probabilidades.
- Calcula 1X2, doble oportunidad, goles totales y por equipo, ambos marcan, hándicap, portería a cero y más.
- Si escribes la cuota de tu casa de apuestas, indica si hay valor y sugiere una apuesta (Kelly fraccionado, tope del 5 % de la banca, en COP).
- Calculadora "cuánto quiero ganar": muestra la probabilidad real que implica la cuota necesaria.

## Cómo usarla

Abre `index.html` en el navegador. No necesita instalación ni servidor.

Para publicarla gratis con GitHub Pages: `Settings → Pages → Deploy from a branch → main / (root)`.

## Datos

Usa la API gratuita de [TheSportsDB](https://www.thesportsdb.com) con la clave pública `123`. Esa clave tiene límites: la app espera 2 segundos entre consultas, por lo que abrir un equipo por primera vez puede tardar unos segundos. Para algunos equipos puede no haber partidos publicados; en ese caso se puede analizar a mano.

## Limitaciones

- El modelo usa solo los goles de los últimos partidos de cada equipo (muestra pequeña) y no distingue local de visitante ni la fuerza de los rivales.
- No conoce lesiones ni sanciones; las bajas se marcan a mano en Ajustes.
- Las casas de apuestas no publican cuotas abiertas: se escriben a mano.
- Corners, tarjetas y tiros no se calculan.

## Aviso

Golvisión estima probabilidades, no predice el futuro, y ninguna apuesta es segura. Es solo para mayores de edad. Juega con responsabilidad y solo con dinero que puedas permitirte perder.
