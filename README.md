---
title: "SPD - Autoritat Certificadora"
author: [Francesc Xavier Bullich Parra, GEINF (UDG-EPS)]
date: 2 de Gener de 2020
subject: "Udg - Eps"
tags: [CA]
subtitle: "Tutor de la pràctica : Antonio Bueno"
titlepage: true

...

\newpage


# Objectiu

L'objectiu del treball és mostrar quins son els elements que composen una autoritat certificadora (CA). També mostraré una forma de crear una autoritat certificadora pròpia, per tal de poder crear certificats de confiança propis.


# Introducció

Una autoritat certificadora és una entitat de confiança que és responsable d'emetre i revocar certificats digitals. Aquests certificats s'usen principalment per garantitzar la seguretat de les comunicacions digitals via TLS-HTTPS. S'utilitiza criptograrfia de clau pública per generar les claus i els certificats.

La CA dona el servei de certificació, que garantitza la relació entre una persona (física o jurídica) i la seva clau pública (certificat), es a dir, un certificat digital ha de identificar a una persona i s'ha de poder confiar en aquesta relació.


## Infraestructura PKI

Tota la gestió de certificats digitals es fa a través d'un PKI (Public key infraestructure). De fet la CA és només una part del PKI.

El PKI es divideix en diversos subsistemes:

- CA: Rep les peticions i crea els certificats. Es responsable d'administrar el cicle de vida dels certificats (temps màxim de validesa o revocació).
- RA: Autoritat de registre és una interficie entre l'usuari i l'autoritat de certificació. Ha d'identificar el solicitants o titulars dels certificats. 
- VA: Autoritat de validació emmagztzema els certificats digitals i aministra l allista de certificats caducats o revocats. També posa a disposició tots els certificats emesos per l'autoritat de certificació.
- Autoritat de custodia: Emmagatzema de forma segura les claus de xifrat que utilitza l'autoritat certificadora.


![Esquema PKI - Wikipedia](images/pki-wiki.png)

# Referències

[1] Que és una CA [https://es.wikipedia.org/wiki/Autoridad_de_certificaci%C3%B3n](https://es.wikipedia.org/wiki/Autoridad_de_certificaci%C3%B3n)
