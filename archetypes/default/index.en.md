---
{{/* Split the path at the dash to create an array. */ -}}
{{- $split := split .Path "\\" -}}
{{- /* Take the second to last entry of the array (the folder above this file). */ -}}
{{- $title := index $split (sub (len $split) 2) -}}
{{- /* Convert minus to space and capitalize words. */ -}}
title: "{{ replace $title "-" " " | title }}"
subtitle: ""
description: ""

date: {{ .Date }}
years: "{{ now.Year }}"
lastmod: {{ .Date }}

comments: true
toc: false

categories: []
tags:
 - untagged
people: []
orgs: []

draft: true
spellchecked: false

shared: [] # e.g. ['twitter', 'facebook', 'linkedin']
meetedgar: [] # insert library entry IDs
---