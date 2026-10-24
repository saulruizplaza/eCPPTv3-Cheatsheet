# 🧪 Plantilla de Documentación eCPPT / Laboratorios de Pentesting

> Una ficha por máquina o ejercicio. Duplica la plantilla y trabaja en una carpeta privada. Registra lo que has demostrado y conserva los intentos fallidos que aportan información.

[Volver a la cheatsheet](README.md) · [Plantilla para varias máquinas](ECPPT_EXAM_TEMPLATE.md)

---

## 📌 Información general

| Campo | Valor |
|---|---|
| Nombre del laboratorio | `[Completar]` |
| Plataforma | `[INE / HTB / THM / local / otra]` |
| Fecha / autor | `[Fecha] / Saúl Ruiz Plaza` |
| Objetivo de aprendizaje | `[Completar]` |
| IP / FQDN / red | `[Completar]` |
| Sistema / arquitectura | `[Confirmado / pendiente]` |
| Alcance y restricciones | `[Completar]` |
| Estado | `[En progreso / terminado / revisado]` |

## 🎯 Qué quiero practicar

- [ ] Reconocimiento y enumeración.
- [ ] Aplicaciones web y bases de datos.
- [ ] Autenticación y acceso inicial.
- [ ] Escalada Linux o Windows.
- [ ] Pivoting y conectividad.
- [ ] Active Directory y relaciones de privilegios.
- [ ] Adaptación de PoC / análisis de memoria.
- [ ] Documentación y remediación.

## 🧱 Preparación

```text
IP e interfaz del equipo de pruebas:
Ruta hacia el objetivo:
DNS y nombres confirmados:
Herramientas y versiones:
Directorio privado de salidas:
Estado inicial / snapshot del laboratorio:
```

## 📋 Registro de verificación

Usa **documental**, **pendiente** o **validado en laboratorio**. Reserva el último estado para una ejecución con versión, contexto y evidencia.

| Técnica / sección de la guía | Fecha | Herramienta y versión exacta | Resultado esperado | Resultado observado | Evidencia privada | Estado |
|---|---|---|---|---|---|---|
| `[Completar]` | `[Fecha]` | `[Versión real]` | `[Qué debería observarse]` | `[Qué ocurrió]` | `[Ruta o identificador]` | Pendiente |

## 🔎 Descubrimiento y servicios

| Puerto / protocolo | Servicio y versión | Cómo se confirmó | Enumeración realizada | Próximo paso |
|---|---|---|---|---|
| `[Completar]` | `[Completar]` | `[Comando/salida]` | `[Completar]` | `[Completar]` |

```text
Comando inicial:
Resultado relevante:
Comando de profundización:
Resultado relevante:
Referencia privada de la evidencia:
```

## 🧩 Hipótesis y decisiones

| Hipótesis | Evidencia a favor | Requisito que falta | Prueba acotada | Resultado |
|---|---|---|---|---|
| `[Completar]` | `[Completar]` | `[Completar]` | `[Completar]` | `[Confirmada / descartada / pendiente]` |

## 🚪 Acceso inicial

```text
Servicio / parámetro:
Identidad usada:
Requisito y versión:
Procedimiento exacto:
Identidad obtenida:
Alcance del acceso:
Evidencia:
```

Si es web, añade petición original, cookie/contexto, petición de prueba y respuesta. Si usas un PoC, añade URL, versión o commit, hash del archivo y modificaciones realizadas.

## 🖥️ Enumeración interna

| Área | Hallazgo | Evidencia | Implicación |
|---|---|---|---|
| Identidad / grupos | `[Completar]` | `[Completar]` | `[Completar]` |
| Privilegios / sudo | `[Completar]` | `[Completar]` | `[Completar]` |
| Servicios / tareas | `[Completar]` | `[Completar]` | `[Completar]` |
| Archivos / permisos | `[Completar]` | `[Completar]` | `[Completar]` |
| Credenciales / claves | `[ID privado]` | `[Origen]` | `[Ámbito]` |
| Interfaces / rutas | `[Completar]` | `[Completar]` | `[Completar]` |

## 🧗 Escalada o movimiento lateral

```text
Identidad anterior:
Permiso o mala configuración:
Propietario / beneficiario:
Quién ejecuta el recurso:
Acción de prueba:
Identidad o acceso posterior:
Por qué demuestra el impacto:
Cambios que necesitan restauración:
```

En AD, incorpora la relación del grafo y su validación actual. En un túnel, registra bind, máquina donde escucha, destino, DNS y retorno.

## 🧾 Ficha del hallazgo

### `[H-01] Título concreto`

| Campo | Contenido |
|---|---|
| Activo | `[IP/FQDN, servicio o recurso]` |
| Condición vulnerable | `[Qué está mal configurado o es vulnerable]` |
| Prerrequisitos | `[Permisos, identidad, red, versión]` |
| Impacto demostrado | `[Acceso u operación concretos]` |
| Severidad razonada | `[Contexto; vector si se utiliza CVSS]` |
| Evidencias | `[Salidas y capturas privadas]` |
| Remediación | `[Cambio que elimina la causa]` |
| Verificación de la corrección | `[Cómo repetir la prueba]` |

### Pasos de reproducción

1. `[Preparación y contexto]`
2. `[Prueba exacta]`
3. `[Resultado observable]`

### Resultado esperado tras corregir

`[Qué operación debe dejar de funcionar y qué funcionalidad legítima debe conservarse]`

## 🧹 Restauración

| Recurso | Estado inicial | Cambio | Restauración | Confirmación |
|---|---|---|---|---|
| `[Completar]` | `[Completar]` | `[Completar]` | `[Completar]` | `[Evidencia]` |

## 🧠 Cadena de aprendizaje

```text
Hallazgo inicial → requisito → acceso → nueva información → siguiente decisión
```

| Qué funcionó | Qué falló y por qué | Qué repetir |
|---|---|---|
| `[Completar]` | `[Completar]` | `[Completar]` |

## ✅ Revisión final

- [ ] Cada afirmación tiene evidencia.
- [ ] Se distingue indicio de vulnerabilidad confirmada.
- [ ] El comando tiene contexto de consola, host e identidad.
- [ ] Se han anotado versiones y requisitos.
- [ ] Los cambios del laboratorio están restaurados o documentados.
- [ ] La ficha incluye remediación y prueba de corrección.
- [ ] La copia pública no contiene credenciales ni material reservado.

---

**Saúl Ruiz Plaza · eCPPT Cheatsheet**
