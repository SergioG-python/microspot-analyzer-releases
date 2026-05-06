# MicroSpot Analyzer Releases

Repositorio publico de distribucion para MicroSpot Analyzer.

Este repositorio no contiene el codigo fuente de la aplicacion. Solo se usa para publicar releases,
instaladores y manifiestos de actualizacion.

## Que es MicroSpot Analyzer

MicroSpot Analyzer es una aplicacion de escritorio para analizar imagenes de microscopia de forma
local. Su objetivo es ayudar en flujos de deteccion, revision humana y conteo de puntos/candidatos
en imagenes importadas por el usuario.

La aplicacion funciona localmente en Windows:

- la interfaz de escritorio se ejecuta con Tauri;
- el backend de analisis se ejecuta como proceso local;
- las imagenes, sesiones y resultados se guardan en el equipo del usuario;
- no se usa este repositorio para almacenar datos de usuario.

## Releases

Cada release puede incluir:

- instalador Windows (`.exe`);
- firma del instalador para el actualizador (`.sig`);
- manifiesto `latest.json` usado por la aplicacion para buscar actualizaciones;
- checksums SHA-256 para verificacion manual.

## Datos y privacidad

Los datos de usuario no se suben a este repositorio.

En una instalacion normal, la base de datos local, imagenes importadas y resultados quedan en el
equipo del usuario, bajo la carpeta local de datos de la aplicacion.

## Estado

Alpha privada. No es una version final validada para uso productivo general.

## Instalacion

Descarga el instalador desde la seccion **Releases** de este repositorio.

En Windows puede aparecer un aviso de SmartScreen porque la firma Windows Authenticode queda
aplazada durante la fase alpha.

## Actualizaciones

La aplicacion puede consultar este repositorio para buscar nuevas versiones mediante el archivo
`latest.json` publicado en el ultimo release.
