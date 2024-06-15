---
layout: default
title: Home
---
<img src="{{ site.url }}/images/19_inch_vs_10_inch_rack.svg" style="display: block; margin: auto;" width="800" />

The Raspberry Pi has PCI Express! There are some quirks to getting certain devices working with 64-bit Arm (arm64), so [Jeff Geerling](https://www.jeffgeerling.com) started testing PCIe devices on the Compute Module 4 and Pi 5, and is centralizing the resources on this site. Many experiences are documented on [Jeff Geerling's YouTube channel](https://www.youtube.com/c/JeffGeerling)!

[This project is maintained on GitHub](https://github.com/geerlingguy/raspberry-pi-pcie-devices); suggest new cards to test or share your own experiences there.

## Categories
{: .no_toc}

- TOC
{:toc}

### Racks

<table class="racks_table">
  <thead>
    <tr>
      <th>Picture</th>
      <th>Device</th>
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
        <a href="{{ rack.url }}"><strong>{{ rack.title }}</strong></a><br>
        (<a href="{{ rack.buy_link }}">Buy this rack</a>)
      </td>
	  
      <td>{{ rack.product_status }}</td>
    </tr>
{% endfor %}
  </tbody>
</table>










## About
{: .no_toc}

[![GitHub Stats](https://github-readme-stats.vercel.app/api/pin?username=geerlingguy&repo=raspberry-pi-pcie-devices&show_icons=true&hide_border=true&show_owner=true&theme=graywhite)](https://github.com/geerlingguy/raspberry-pi-pcie-devices)

This project is maintained by [Jeff Geerling](https://www.jeffgeerling.com). The Raspberry Pi Compute Module 4 and Raspberry Pi 5 model B are products of [Raspberry Pi (Trading) Limited](https://www.raspberrypi.org/about/).

> Many of the device links on this page are Amazon affiliate links. If you do not wish to use those links, copy the device name to search for it at any major electronics retailer (e.g. [Newegg](https://www.newegg.com), [Micro Center](https://www.microcenter.com), [Amazon](https://www.amazon.com), etc.).
