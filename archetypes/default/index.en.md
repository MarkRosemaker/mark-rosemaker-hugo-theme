---
{{/* Split the path at the dash to create an array. */ -}}
{{- $split := split .Path "\\" -}}
{{- /* Take the second to last entry of the array (the folder above this file). */ -}}
{{- $title := index $split (sub (len $split) 2) -}}
{{- /* Convert minus to space and capitalize words. */ -}}
title: "{{ replace $title "-" " " | title }}"
subtitle: ""

date: {{ .Date }}
years: "{{ now.Year }}"
lastmod: {{ .Date }}

draft: true
spellchecked: false
shared: [] # 'twitter', 'facebook'
meetedgar: [] # insert library entry IDs

comments: true
toc: false

seo_title: ""
description: ""

categories: []
tags:
 - untagged
people: []
orgs: []
---