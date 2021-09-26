---
layout: collection
collections: directory
title: Una Comunidad de Queseros
permalink: /comunidad/
---

Nuestros Quesos nace de una idea de Afrael Ortiz, Irwin Molero y Sergio Pizzarelli. El principal objetivo de esta idea es agrupar en una página todos aquellos que hacemos quesos Venezolanos, o quesos artesanales, por hobby o para la venta.

Ademas de ser una comunidad de queseros, también quisimos crear un recetario de quesos y otros productos lácteos, ser una guía para principiantes o recetas complejas para los más experimentados.

## Paises donde nos encontramos

{% assign sorted = site.directory | sort: 'country' %}
{% assign grouped = sorted | group_by: 'country' %}
{% for country in grouped %}
<h3>{{ country.name }}</h3>

  {% for item in country.items %}
  
  <table>
    <colgroup>
        <col width="18%" />
        <col width="20%" />
        <col width="63%" />
    </colgroup>
    <tbody>
        {% assign firstLink = item.links[0] | strip %}
        <tr>
            {% if firstLink == '' %}
            <td markdown="span"><img class="author-avatar u-photo" src="{{ item.image }}"/></td>
            {% else %}
            <td markdown="span"><a href="{{ firstlink }}"><img class="author-avatar u-photo" src="{{ item.image }}"/></a></td>
            {% endif %}
            <td markdown="span"> {{item.name}} - {{ item.city }}</td>
            <td markdown="span">{{ item.bio }}</td>
        </tr>
        {% if firstLink != '' %}
        <tr>
            <td colspan="3">
                <p>{{ linkCount }}</p>
                <ul>
                {% for lnk in item.links %}
                  <li> <a href="{{ lnk}}">{{ lnk }}</a> </li>
                {% endfor %}
                </ul>
            </td>
        </tr>
        {% endif %}
    </tbody>
  </table>

  {% endfor %}
{% endfor %}
