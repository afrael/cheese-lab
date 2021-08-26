---
layout: page
title: Donde estamos
permalink: /mapa/
---

Si deseas formar parte del mapa de nuestros quesos, solo tienes que llenar el [siguiente formulario](https://forms.gle/j3jdZuhkQxVSSdAH8), una vez aprobado tu registro el marcador será agregado en el mapa.

{% leaflet_map {"zoom" : 2 } %}
    {% leaflet_marker { "latitude" : 33.9562,
                       "longitude" : -83.9880,
                       "popupContent" : "Moleros Artisan Cheese. Quesos Venezolanos, ofrece los siguientes quesos: Palmita, Semiduro, Concha roja y negra, De Mano, Telita y Guayanes, Cabra, De Matera",
                       "href" : "https://www.instagram.com/moleros_artisancheese/"} %}

    {% leaflet_marker { "latitude" : 28.5653,
                       "longitude" : -81.5862,
                       "popupContent" : "SK Pizzarelli"} %}

    {% leaflet_marker { "latitude" : 27.9506,
                       "longitude" : -82.4572,
                       "popupContent" : "Luis Mejia"} %}

    {% leaflet_marker { "latitude" : 52.5200,
                       "longitude" : 13.4050,
                       "popupContent" : "Richard Serf"} %}
    
    {% leaflet_marker { "latitude" : 13.6929,
                       "longitude" : -89.2182,
                       "popupContent" : "Nancy de Alvarado",
                       "href" : "https://www.instagram.com/7estrellassv/"} %}
    
    {% leaflet_marker { "latitude" : 25.9087,
                       "longitude" : -80.3087,
                       "popupContent" : "Mawell"} %}
{% endleaflet_map %}