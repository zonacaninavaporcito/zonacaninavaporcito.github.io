# Design

<!-- impeccable:design-schema 1 -->

## Visual World

**Bando en la Caseta** — mundo híbrido entre bando municipal gaditano y caseta de feria. Papel verjurado crema (#FDF8F0) como campo, tinta azul noche (#121E2A) y azul indigo (#163A59) para autoridad, vermellón municipal (#C43C2A) como sello único, albero (#F2C14E) como acento festivo, sarga (#7A8B6F) y azulejo (#1B6B6B) para detalles. Materiales: papel con borde sutil, rayas de caseta (franja de 8px repeating-linear), azulejo strip, sello circular con sombra suave. Nunca cream + serif genérico aislado: el sistema completo es bando + feria + azulejo.

## Typography

Display: **EB Garamond** 600/700 (bando masthead, citas legales) — serif con italica para tesis.  
Pancarta: **Bricolage Grotesque** 700/800 (titulares cortos, contadores, badges) — grotesca con carácter.  
Lectura: **Manrope** 400/500/600/700 (cuerpo, navegación, UI).  
Escala: display max 64px, medida 65–75ch, tracking -0.02em en display. Pesos con salto obvio, no gradiente.

## Color Strategy

Committed — vermellón carga ~30% en CTAs/sellos/progreso, albero ~15% como luz, indigo como campo oscuro para ley, resto neutro papel. Composición a escala de página, no acentos dispersos. Uso claro (luz de mañana en patio) — fondo claro por defecto, indigo solo en bloque ley.

## Components

Bando header sticky con sello circular + marca + nav + CTA vermellón. Counter-card papel con dígitos en celdas (nixie-donada) + barra de progreso con thumb. Math-cards con icono en celdas 44px + tag vermellón. Map-card con iframe + pin flotante + caption. Law-card indigo con cita con barra interior dorada + timeline vertical. Compartimentos ekiben (3 columnas, franja superior rayada) para claims. Share-cards con iconos 42px y CTA ghost.

## Motion

Un momento autoral: progreso del contador de 0→38% con ease exponencial (900ms) respetando prefers-reduced-motion. Resto estático. Transiciones de hover suaves (150ms) solo en CTAs. Sin entradas por sección.

## Constraints

Contraste ≥4.5:1, focus visible en albero, selección en albero, scroll-margin para anclas, sticky CTA solo en <700px, imágenes reales verificadas (map embed oficial), copy en español rioplatense neutro para UI pero tono de campaña “indignación tranquila + humor local”.

## Provenance

Built from PRODUCT.md (web, Astro static → GitHub Pages), shape brief 2026-08-28 (Persuade, firma+compartir, 80% móvil + institucional, prueba completa), direction seed cce5f0b3 assigned 7 (Bando en la Caseta) with raises from nixie (dígitos tabulares) and ekiben (compartimentos index).
