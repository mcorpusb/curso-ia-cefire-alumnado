---
layout: page
title: "Guia · Aules i manuscrits"
parent: "Bloc 4: Avaluació i Personalització"
nav_order: 2
lang: va
translation_key: bloque4-aules
nav_exclude: true
---

{% include language-switcher.html %}

# Aules i revisió assistida · Guia pràctica
{: .fs-8 }

## 1. Compartir «Detectius d'IA» en Aules

[Prova l'aplicació en valencià]({{ '/detectives-ia/va.html' | relative_url }}){: .btn .btn-primary } [Versió en castellà]({{ '/detectives-ia/' | relative_url }}){: .btn }

**Opció A · URL (recomanada)**

1. Publica l'activitat en una adreça HTTPS accessible per a l'alumnat, com ara GitHub Pages **quan s'haja publicat la versió del curs**.
2. En Aules activa l'edició → afig un recurs **URL** → apega l'adreça de l'aplicació.
3. Escriu la consigna i guarda. Comprova que funciona en la vista de l'alumnat o amb un compte de prova.
4. Les qualificacions no es transferixen automàticament al llibre de notes.

**Opció B · iframe, només si està permés**

En un recurs Pàgina, usa l'editor HTML quan estiga disponible. Prova amb una adreça pública autoritzada:

```html
<iframe src="https://EXEMPLE-VALID/activitat/"
 title="Detectius d'IA" width="100%" height="620"
 loading="lazy" style="border:1px solid #ccc"></iframe>
```

Comprova que Aules no elimina l'etiqueta i que el servidor permet incrustar-la. Si falla, usa el recurs URL. No intentes evitar els filtres de seguretat.

**Opció C · Fitxer HTML, si la plataforma l'admet**

Baixa `index.html` i tots els recursos, puja el fitxer o paquet compatible com a recurs Fitxer i comprova com s'obri. Algunes instal·lacions obliguen a baixar-lo o bloquegen scripts. Si falla, utilitza un enllaç URL.

**Per a registrar notes:** planteja't un Qüestionari natiu, H5P o SCORM, sempre que estiguen habilitats i configurats.

| Problema | Comprova |
|---|---|
| L'alumnat no pot obrir l'enllaç | Permisos d'accés i allotjament públic |
| iframe buit | Filtres HTML, CSP o X-Frame-Options: utilitza URL |
| El fitxer HTML no executa JavaScript | Restriccions del recurs: utilitza URL |
| Falten imatges o estils | Rutes relatives i recursos inclosos |
| No apareix cap nota en Aules | Una app externa no sincronitza resultats automàticament |

## 2. Què hi ha escrit? Exàmens manuscrits ficticis

Practica amb dues imatges **sintètiques**, no són exàmens de cap alumne real. La lletra és deliberadament molt difícil de llegir: no demanes a la IA que se n'invente una transcripció.

<div style="display:flex;gap:1rem;flex-wrap:wrap">
<figure><img src="{{ '/assets/img/bloque4/examen-ficticio-ciencias.jpg' | relative_url }}" width="160" height="215" alt="Full fictici de ciències amb lletra quasi il·legible."><figcaption>Ciències Naturals · Fotosíntesi</figcaption></figure>
<figure><img src="{{ '/assets/img/bloque4/examen-ficticio-tecnologia.jpg' | relative_url }}" width="160" height="215" alt="Full fictici de tecnologia amb lletra quasi il·legible."><figcaption>Tecnologia · Circuit en sèrie</figcaption></figure>
</div>

### Prompt per a copiar i provar

```text
Observa esta imatge fictícia. Actua com a assistent de transcripció
sense inventar informació:
1. Separa l'enunciat imprés de la resposta manuscrita.
2. Transcriu literalment només els fragments que pugues llegir.
3. Escriu [il·legible] quan no pugues desxifrar una paraula.
4. Si dubtes entre lectures, marca [dubtós: A/B]; no endevines.
5. No reformules la transcripció ni completes expressions pel context.
6. A banda, indica interpretacions possibles amb incertesa.
7. No qualifiques la resposta sense revisar l'original físic.
```

**Comparació i retroacció:** el docent aportarà una rúbrica i només corregirà els fragments verificables. En Ciències, els conceptes de referència són llum, aigua, CO₂, matèria orgànica i oxigen. En Tecnologia, un circuit en sèrie té un únic recorregut i la mateixa intensitat en tots els elements; si s'obri, deixa de circular corrent. **Són referències conceptuals, no transcripcions confirmades del text manuscrit.**

**Retroacció orientativa:** «Hi ha fragments de la resposta que no puc llegir amb seguretat. Abans d'avaluar-los, necessite aclarir-los i comprovar si expliquen el concepte sol·licitat».

**Privacitat:** tapar el nom no sempre anonimitza un examen real. Utilitza els exemples sintètics; per a treballs reals calen permisos i garanties institucionals.

## 3. Adaptació per etapa

Infantil: interpretar dibuixos ficticis amb mediació; Primària: resposta breu de ciències; ESO: explicació conceptual; Batxillerat: argumentació; FP: resposta tècnica; EOI: expressió escrita. La IA mai substituïx la revisió docent.
