---
{{/* Split the path at the dash to create an array. */ -}}
{{- $split := split .Path "\\" -}}
{{- /* Take the second to last entry of the array (the folder above this file). */ -}}
{{- $slug := index $split (sub (len $split) 2) -}}
{{- /* Convert minus to space and capitalize words. */ -}}
{{- $title := replace $slug "-" " " | title -}}
title: "[translation of {{ $title }}]"
subtitle: ""
description: ""

slug: "../[translation of {{ $slug }}]/"
aliases: ["../[translation of {{ $slug }}]/", "../de/{{ $slug }}/"]

date: {{ .Date }}
years: "{{ now.Year }}"
lastmod: {{ .Date }}

categories: []
tags:
 - untagged
people: []
orgs: []

draft: true
spellchecked: false

shared: [] # z.B. ['twitter', 'facebook', 'linkedin']
meetedgar: [] # insert library entry IDs
---






comments: true
toc: false

subtitle: ""
seo_title: ""
description: ""

categories: []
tags:
 - untagged
people: []
orgs: []
---