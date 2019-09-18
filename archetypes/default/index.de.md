---
{{/* Split the path at the dash to create an array. */ -}}
{{- $split := split .Path "\\" -}}
{{- /* Take the second to last entry of the array (the folder above this file). */ -}}
{{- $slug := index $split (sub (len $split) 2) -}}
{{- /* Convert minus to space and capitalize words. */ -}}
{{- $title := replace $slug "-" " " | title -}}
title: "[translation of {{ $title }}]"
subtitle: ""

slug: "../[translation of {{ $slug }}]/"
aliases: ["../[translation of {{ $slug }}]/", "../de/{{ $slug }}/"]

date: {{ .Date }}
years: "{{ now.Year }}"
lastmod: {{ .Date }}

draft: true
spellchecked: false
shared: [] # 'twitter', 'facebook'
meetedgar: [] # insert library entry IDs

# meta data
seo_title: ""
description: ""

# dates
publishDate: {{ .Date }} # update from ISO 8601: https://www.unixtimestamp.com/

# Categorization
tags: []
people: []
orgs: []
categories: []
difficulty: []

draft: true
spellchecked: false
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