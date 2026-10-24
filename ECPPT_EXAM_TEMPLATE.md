# 🧭 Plantilla de Documentación para Examen eCPPTv3

> Cuaderno privado para simulacros y prácticas con varios hosts, redes e identidades. Utilízalo en una convocatoria solo si sus instrucciones lo permiten. Guarda la copia con tus evidencias y secretos fuera del repositorio.

[Volver a la cheatsheet](README.md) · [Plantilla de laboratorio](LAB_TEMPLATE.md)

---

## 📌 Información general

| Campo | Valor |
|---|---|
| Fecha y zona horaria | `[Completar]` |
| Convocatoria / laboratorio | `[Completar]` |
| Instrucciones aplicables | `[Versión y ubicación]` |
| Inicio / fin previsto | `[Completar]` |
| Interfaz e IP de trabajo | `[Completar]` |
| Rangos autorizados | `[Completar]` |
| Exclusiones | `[Completar]` |
| Recursos y herramientas permitidos | `[Completar]` |
| Estado | `[En progreso / revisión / finalizado]` |

## 🗺️ Topología y accesibilidad

```text
Equipo de trabajo → punto de entrada → red interna → objetivos
[Dibujar las IP, interfaces y conexiones realmente confirmadas]
```

| Red / destino | Visible desde | Sesión / ruta / túnel | Prueba de conectividad | Estado |
|---|---|---|---|---|
| `[Red]` | `[Host]` | `[Identificador]` | `[Comando y evidencia]` | `[Confirmado / pendiente]` |

## 🖥️ Inventario de hosts

| ID | IP / FQDN | SO / función | Puertos | Acceso confirmado | Próximo paso |
|---|---|---|---|---|---|
| H01 | `[Completar]` | `[Completar]` | `[Completar]` | `[Ninguno / identidad]` | `[Completar]` |

## 🔎 Registro de hipótesis

| Hora | Host | Evidencia de partida | Hipótesis | Prueba | Resultado | Decisión |
|---|---|---|---|---|---|---|
| `[Hora]` | H01 | `[Salida]` | `[Qué podría permitir]` | `[Acción]` | `[Hecho observado]` | `[Continuar / descartar]` |

Evita registrar «vulnerable» sin una prueba. Distingue **indicio**, **verificado** y **descartado**.

## 🎯 Cobertura personal del programa

Consulta el [índice de temas](README.md#indice). Añade una fila por objetivo: una sección leída no equivale a una práctica completada.

| Objetivo | Sección de la guía | Fecha / versión del entorno | Evidencia | Qué necesito repetir | Estado |
|---|---|---|---|---|---|
| `[Objetivo publicado por INE]` | `[Enlace o título]` | `[Completar]` | `[Identificador privado]` | `[Completar]` | Pendiente |

## 🧩 Ficha por host — duplicar para cada equipo

### H01 · Identidad y servicios

| Campo | Valor |
|---|---|
| IP / FQDN / nombre NetBIOS | `[Completar]` |
| Dominio o grupo de trabajo | `[Completar]` |
| Identidad inicial / actual | `[Completar]` |
| Privilegios e integridad | `[Completar]` |
| Arquitectura | `[Completar]` |
| Servicios y versiones confirmadas | `[Completar]` |
| Capturas / salidas | `[Rutas privadas]` |

### Enumeración y acceso

```text
Recurso o parámetro:
Requisito confirmado:
Comando / petición exacta:
Salida relevante:
Identidad obtenida:
Qué habilita este acceso:
Qué sigue sin estar demostrado:
```

### Escalada y movimiento

```text
Permiso / mala configuración:
Propietario del recurso:
Quién ejecuta la acción:
Prueba mínima:
Identidad / permisos resultantes:
Redes o hosts nuevos:
Restauración necesaria:
```

## 🔐 Credenciales y material de autenticación

Mantén secretos en un almacén privado. Aquí puedes utilizar identificadores como `CRED-01` para evitar repetirlos.

| ID | Usuario | Ámbito local/dominio | Tipo de material | Origen | Servicio probado | Resultado |
|---|---|---|---|---|---|---|
| CRED-01 | `[Usuario]` | `[Ámbito]` | `[Contraseña / NT / ticket / clave]` | `[Evidencia]` | `[Host y protocolo]` | `[Completar]` |

### Control de intentos online

| Cuenta | Política efectiva | Fallos previos | Intento actual | Hora | Bloqueo / siguiente ventana |
|---|---|---|---|---|---|
| `[Cuenta]` | `[Umbral y ventana]` | `[Número conocido]` | `[ID del candidato]` | `[Hora]` | `[Estado]` |

No conviertas una ausencia de datos sobre la política en permiso para lanzar múltiples intentos.

## 🏢 Active Directory

| Dato | Valor confirmado |
|---|---|
| Dominio / realm / SID | `[Completar]` |
| DC y DNS | `[IP y FQDN]` |
| Hora y diferencia observada | `[Completar]` |
| Usuarios y grupos relevantes | `[Completar]` |
| SPN / cuentas de servicio | `[Completar]` |
| Candidatos sin preautenticación | `[Completar]` |
| Colector / versión / fecha | `[Completar]` |

### Rutas de privilegios

| Origen | Relación / permiso | Objeto destino | Requisito | Validación actual | Efecto demostrado |
|---|---|---|---|---|---|
| `[Principal]` | `[ACE / grupo / sesión]` | `[Objeto]` | `[Completar]` | `[Evidencia]` | `[Completar]` |

### Tickets y hashes

| ID privado | Principal | Tipo / cifrado | Servicio o ámbito | Inicio / fin de validez | Uso comprobado |
|---|---|---|---|---|---|
| `[ID]` | `[Completar]` | `[TGT / TGS / AS-REP / NT]` | `[SPN / host / dominio]` | `[Fechas]` | `[Evidencia]` |

## 🛣️ Pivoting y retornos

| ID | Tipo | Máquina donde escucha | Bind / puerto | Destino visto por el pivote | Sesión dependiente |
|---|---|---|---|---|---|
| TUN-01 | `[SOCKS / local / remoto / TUN]` | `[Host]` | `[IP:puerto]` | `[IP:puerto o red]` | `[Sesión]` |

```text
Ruta de ida:
Ruta de retorno:
DNS empleado:
Prueba simple realizada:
Comando exacto de creación:
Cómo detenerlo y restaurar rutas:
```

## 🧾 Objetivos y evidencias

| ID del objetivo | Hecho que se necesita demostrar | Host | Evidencia | Estado |
|---|---|---|---|---|
| OBJ-01 | `[Descripción permitida]` | H01 | `[Ruta privada]` | `[Pendiente / verificado]` |

No publiques preguntas, respuestas ni información reservada de una convocatoria.

## 🧹 Cambios y restauración

| Host | Recurso | Estado anterior | Cambio | Prueba | Estado restaurado |
|---|---|---|---|---|---|
| H01 | `[Archivo / servicio / ruta]` | `[Completar]` | `[Completar]` | `[Evidencia]` | `[Sí / no / motivo]` |

## ✅ Cierre

- [ ] Alcance e instrucciones revisados.
- [ ] Hosts y rutas confirmados, sin mezclar resultados de otras sesiones.
- [ ] Cada objetivo tiene evidencia suficiente y contexto.
- [ ] Credenciales clasificadas por tipo y ámbito.
- [ ] Las rutas del grafo se han validado en el entorno.
- [ ] Cambios y túneles revisados.
- [ ] Se ha realizado la entrega que exige esta convocatoria.
- [ ] Copia privada de notas y evidencias conforme a sus reglas.

## 🧠 Lecciones aprendidas

```text
Qué me hizo perder tiempo:
Qué hipótesis fue decisiva:
Qué comando o requisito no entendía:
Qué necesito repetir sin consultar apuntes:
```

---

**Saúl Ruiz Plaza · eCPPT Cheatsheet**
