---
title: Päivämäärän lokalisointi
description: Luxon apuna päiääärien formatointiin
date: 2026-09-23
preview: ""
draft: false
tags: []
categories: []
---
Tartuin tämän Eleventyn tuottamaan päivämäärän formaattiin -tehtävään. Halusin sen suomalaisemmaksi, alkuperäinen kun oli englannin kielellä ja minä haluan artikkeleihin julkaisupäivämäärän muotoon: pp.kk.vvvv

Oli tsekattava MDN JavaScript-dokumentaatiosta, kuinka tämä nykyään menee. Siellähän olikin selkeät nuotit. 

[Mozilla MDN JavaScript Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Intl/DateTimeFormat/DateTimeFormat)

Samalla tsekkasin Eleventyn dokumentaation ja sieltä selvisi mainio **Filters** -ominaisuus. Niinpä tein oman filtterin ja onnistuinkin ekalla yrittämällä. Voi että omatunto kohoaa ;)
[Eleventy Docs - Filters](https://www.11ty.dev/docs/filters/).

Toimii.

Sitten pläräsin näitä konffifileitä ja huomasin, että _config -kansiossa on filters.js -tiedosto. Siellä olikin kerrottu, että apuna käytetään Luxon-nimista JavaScript-apuria päivämäärien manipulointiin. OK, no taulukosta löytyikin sitten vipu, jolla homma hoituu. Poistin siis oman filterin, vaikka olinkin siitä niiiiin ylpeä ;)
[Lucon - Table of tokens](https://moment.github.io/luxon/#/formatting?id=table-of-tokens).