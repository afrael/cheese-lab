---
layout: page
title: Donde estamos
permalink: /mapa/
---

{% leaflet_map {"zoom" : 2 } %}
    {% leaflet_marker { "latitude" : 33.9562,
                       "longitude" : -83.9880,
                       "popupContent" : "Moleros Artisan Cheese",
                       "href" : "https://www.instagram.com/moleros_artisancheese/"} %}

    {% leaflet_marker { "latitude" : 28.5653,
                       "longitude" : -81.5862,
                       "popupContent" : "SK Pizzarelli"} %}

    {% leaflet_marker { "latitude" : 27.9506,
                       "longitude" : -82.4572,
                       "popupContent" : "Luis Mejia"} %}
{% endleaflet_map %}