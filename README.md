# Stock Lab - Ejecutable

Repositorio publico de distribucion de **Stock Lab**. Contiene las versiones del ejecutable de Windows utilizadas por la descarga manual y el actualizador automatico de la aplicacion.

## Ultima version

[Descargar `stock-lab.exe`](https://github.com/sebasbanegas/stock-lab/releases/latest/download/stock-lab.exe)

[Ver notas, fecha y checksum de la ultima release](https://github.com/sebasbanegas/stock-lab/releases/latest)

Los enlaces usan `releases/latest`, por lo que siempre apuntan a la publicacion vigente sin mantener un numero de version fijo en este README.

## Actualizacion automatica

Stock Lab consulta la ultima GitHub Release al iniciar. Cuando existe una version superior, descarga el asset llamado exactamente `stock-lab.exe` y reemplaza el ejecutable al reiniciar.

La actualizacion conserva el `config.json`, las credenciales y las bases locales que ya existen en el equipo. Esos archivos no se publican en este repositorio.

## Integridad

Cada release incluye:

- `stock-lab.exe`: ejecutable consumido por el autoupdate.
- `stock-lab-X.Y.Z.exe.sha256`: checksum SHA-256 para validacion manual.

El checksum correspondiente se encuentra entre los assets de cada publicacion en [Releases](https://github.com/sebasbanegas/stock-lab/releases).

## Alcance del repositorio

Este repositorio contiene solamente artefactos de distribucion:

- No contiene el codigo fuente.
- No contiene `config.json` ni tokens de Turso.
- No contiene bases de datos ni backups de usuarios.
- No se utiliza para desarrollo.

El codigo fuente, la arquitectura, las pruebas y la documentacion tecnica se mantienen por separado en el repositorio privado `sebasbanegas/stock-lab-tauri`.
