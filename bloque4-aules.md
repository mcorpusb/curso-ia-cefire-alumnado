---
layout: page
title: "Guía · Aules y manuscritos"
parent: "Bloque 4: Evaluación y Personalización"
nav_order: 2
lang: es
translation_key: bloque4-aules
nav_exclude: false
---

{% include language-switcher.html %}

# Aules y corrección asistida · Guía práctica
{: .fs-8 }

## 1. Compartir «Detectives de IA» en Aules

[Probar la aplicación en castellano]({{ '/detectives-ia/' | relative_url }}){: .btn .btn-primary } [Versión en valenciano]({{ '/detectives-ia/va.html' | relative_url }}){: .btn }

**Opción A · URL (recomendada)**

1. Publica la actividad en una dirección HTTPS accesible al alumnado, como GitHub Pages **una vez publicada la versión del curso**.
2. En Aules activa edición → añade recurso **URL** → pega la dirección de la aplicación.
3. Escribe una consigna y guarda. Comprueba que funciona con una cuenta de prueba o vista del alumnado.
4. No se envían automáticamente notas al libro de calificaciones.

**Opción B · iframe, solo cuando esté permitido**

En un recurso Página, usa el editor HTML si está disponible. Prueba con una dirección pública autorizada:

```html
<iframe src="https://EJEMPLO-VALIDO/actividad/"
 title="Detectives de IA" width="100%" height="620"
 loading="lazy" style="border:1px solid #ccc"></iframe>
```

Comprueba si Aules conserva la etiqueta y si el servidor permite incrustarla. Si no funciona, utiliza URL. No intentes eludir los filtros de seguridad.

**Opción C · HTML descargado, si la plataforma lo admite**

Descarga `index.html` con sus recursos, sube el archivo o paquete compatible como recurso Archivo y comprueba cómo se abre desde Aules. Algunas instalaciones fuerzan la descarga o bloquean scripts. Si falla, utiliza URL.

**Para obtener notas:** valora crear un Cuestionario nativo, H5P o SCORM, siempre que la instalación y la configuración lo admitan.

| Problema | Qué revisar |
|---|---|
| El alumnado no puede abrir el enlace | Permisos y acceso público del alojamiento |
| El iframe sale vacío | Filtros HTML, CSP o X-Frame-Options: usa URL |
| HTML descargado no ejecuta JS | Restricciones del recurso: usa URL |
| Faltan imágenes o estilos | Rutas relativas y archivos incluidos |
| No aparece nota en Aules | Una app externa no sincroniza resultados automáticamente |

## 2. ¿Qué ha escrito? Exámenes manuscritos ficticios

Practica con dos imágenes **sintéticas**. No son exámenes de estudiantes reales. Están intencionadamente muy difíciles de leer; son muestras para estudiar los límites de la transcripción asistida y **no deben usarse para exigir a la IA una lectura inventada**.

<div style="display:flex;gap:1rem;flex-wrap:wrap">
<figure><img src="{{ '/assets/img/bloque4/examen-ficticio-ciencias.jpg' | relative_url }}" width="160" height="215" alt="Hoja ficticia de ciencias con escritura casi ilegible."><figcaption>Ciencias Naturales · Fotosíntesis</figcaption></figure>
<figure><img src="{{ '/assets/img/bloque4/examen-ficticio-tecnologia.jpg' | relative_url }}" width="160" height="215" alt="Hoja ficticia de tecnología con escritura casi ilegible."><figcaption>Tecnología · Circuito en serie</figcaption></figure>
</div>

### Prompt para copiar y probar

```text
Observa esta imagen ficticia. Actúa como asistente de transcripción
sin inventar contenido:
1. Separa el enunciado impreso de la respuesta manuscrita.
2. Transcribe literalmente solo los fragmentos que puedas leer.
3. Escribe [ilegible] cuando no puedas descifrar una palabra.
4. Si dudas entre dos lecturas, indica [dudoso: A/B]; no adivines.
5. No reformules la transcripción ni completes expresiones por contexto.
6. En una sección aparte, indica posibles interpretaciones con
   incertidumbre. No califiques la respuesta como si fuese legible.
7. Solicita revisión del original físico antes de valorar.
```

**Comparación y feedback:** el profesor aportará su rúbrica y corregirá **solo lo que pueda verificar en el original**. En Ciencias, la referencia conceptual aborda luz, agua, CO₂, producción de materia orgánica y oxígeno. En Tecnología, circuito en serie significa recorrido único y misma intensidad en los elementos; una interrupción abre el circuito. **Estas ideas son pautas conceptuales, no una transcripción confirmada del manuscrito.**

**Retroalimentación posible:** «Hay partes de la respuesta que no puedo leer con seguridad. Antes de corregir, necesito aclarar esas palabras y comprobar si la explicación expresa el concepto solicitado».

**Privacidad:** cubrir el nombre no siempre convierte un examen real en anónimo. Utiliza aquí únicamente los ejemplos sintéticos; con materiales reales se requieren autorizaciones y garantías institucionales específicas.

## 3. Adaptación por etapa

Infantil: interpretar dibujos o instrucciones propias ficticias; Primaria: respuesta sencilla de ciencias; ESO: explicación conceptual; Bachillerato: argumentación; FP: respuesta técnica; EOI: producción escrita. La IA nunca sustituye la comprobación docente.
