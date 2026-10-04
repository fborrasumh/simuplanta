# SimuPlanta AI

Simulador interactivo de respuestas fisiológicas en cultivos ante variaciones ambientales (estrés hídrico, salinidad, temperatura, luz y nutrición). Aplicación web de un solo fichero, con el diseño Forja de la Universidad Miguel Hernández de Elche.

**Usar la app:** https://fborrasumh.github.io/simuplanta/

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23138255.svg)](https://doi.org/10.5281/zenodo.23138255)

> Catálogo [fborrasumh/ia](https://fborrasumh.github.io/ia/) · Universidad Miguel Hernández de Elche

## Qué hace

- Permite elegir entre 26 especies (hortalizas, leñosos mediterráneos, subtropicales, cereales, forrajeras e industriales) y ajustar déficit de riego, salinidad (CE), temperatura, luz (PAR) y nutrición.
- Simula día a día, de 7 a 120 días, la fotosíntesis relativa, la conductancia estomática, la biomasa acumulada y el estrés integrado, con gráfico y tabla diaria.
- Muestra los cinco factores de reducción (0–1) y señala cuál limita más al cultivo.
- Guarda hasta 8 escenarios y los compara en una tabla y en barras de biomasa y estrés; cualquiera puede volver a cargarse en el laboratorio.
- Genera un informe del escenario actual y descarga un informe HTML y dos CSV (serie diaria y escenarios; separador «;» y coma decimal).
- Incluye un ejemplo (tomate con y sin estrés) que funciona sin clave de IA.

## Cómo se usa la IA

Es opcional y solo sirve para redactar una interpretación del escenario. Se usa con la propia clave de OpenAI, Google Gemini o Anthropic Claude, que se guarda solo en el navegador. No hace falta servidor. El código comprueba que las cifras que cita la IA figuren en el escenario y marca las que no.

## Privacidad

Los cálculos se hacen en el navegador. Los escenarios y la configuración se guardan en este navegador (IndexedDB) y la clave de IA en `localStorage`. Solo si se pulsa «Interpretar con IA» salen hacia el proveedor elegido los parámetros del escenario y sus resultados numéricos. No se envía ningún texto ni dato personal.

## Límites

Es un modelo didáctico y exploratorio, con factores multiplicativos calibrados por especie, no por cultivar. No sustituye a modelos de cultivo de proceso (DSSAT, APSIM, etc.) ni a ensayos experimentales, y no sirve para predecir una cosecha. La interpretación de la IA puede equivocarse: la comprobación de cifras no valida su razonamiento. No se ha probado con claves reales de los proveedores.

## Autoría

María Emma García Pastor (Universidad Miguel Hernández de Elche) y Fernando Borrás Rocher (Universidad Miguel Hernández de Elche).

Idea original de María Emma García Pastor: laboratorio virtual y herramienta preliminar para escenarios de cambio climático y pre-ensayo en invernadero.

ORCID: María Emma García Pastor [0000-0002-4959-9419](https://orcid.org/0000-0002-4959-9419) · Fernando Borrás Rocher [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573)

## Cómo citar

García Pastor, M. E. y Borrás Rocher, F. (2026). *SimuPlanta AI* (v2.0.0) [Software]. Universidad Miguel Hernández de Elche. DOI: [10.5281/zenodo.23138255](https://doi.org/10.5281/zenodo.23138255)

## Licencia

MIT. Véase [LICENSE](LICENSE).
