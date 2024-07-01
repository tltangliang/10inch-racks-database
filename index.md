---
layout: default
title: Home
---
<img src="{{ site.url }}/images/19_inch_vs_10_inch_rack.png" style="display: block; margin: auto;" width="800" />

The 10-inch rack (aka “half-rack”) isn’t a standard . Instead, it’s more like a general consensusso. 

Whereas there is no formal specification for "half rack", the term half-rack can have different separate meanings: It can describe equipment that fits in a certain number of rack units, but occupy only half the width of a 19-inch rack (9.5 inches (241.30 mm)). These are commonly used when a piece of equipment does not require full rack width, but may require more than 1U of height.


[This project is maintained on GitHub](https://github.com/tltangliang/10inch-racks-database); suggest new devices to test or share your own experiences there.

## Categories
{: .no_toc}

- TOC
{:toc}

### Racks

<table class="racks_table">
  <thead>
    <tr>
      <th>Picture</th>
      <th>Title</th>
      <th>Brand</th>
      <th>Height</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
{% for rack in site.racks %}
    <tr>
      <td class="rack_picture_td">
        {% if rack.picture %}
          <a href="{{ rack.url }}"><img class="rack_table_picture" src="{{ rack.picture | image_thumbnail }}" alt="{{ rack.title }}"></a>
        {% endif %}
      </td>
	  
      <td>
        <a href="{{ rack.url }}"><strong>{{ rack.title }}</strong></a>
      </td>

      <td>
        {{ rack.brand }}
      </td>

      <td>
        {{ rack.height }}
      </td>
	  
      <td>{{ rack.product_status }}</td>
    </tr>
{% endfor %}
  </tbody>
</table>



## About
{: .no_toc}


This project is maintained by [Rex Tang](https://github.com/tltangliang). 

> Many of the device links on this page are Amazon affiliate links. If you do not wish to use those links, copy the device name to search for it at any major electronics retailer (e.g. [Newegg](https://www.newegg.com), [Micro Center](https://www.microcenter.com), [Amazon](https://www.amazon.com), etc.).
