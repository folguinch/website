---
layout: page
title: Cycling
description: My bicycles and adventure trips.
img: assets/img/cycling_kom.jpg
#img: assets/img/
importance: 1
category: fun
---

## Cycling challenges

{% assign mydata=site.data.challenges%}
<table class="mytable" >
  <thead>
  {% for col in mydata[0] %}
    {% if col[0] != "link" %}
      {% if forloop.first %}
        <th>{{ col[0] | capitalize }}</th>
      {% else %}
        <th class="table-right">{{ col[0] | capitalize }}</th>
      {% endif %}
    {% endif %}
  {% endfor %}
  </thead>
  <thead>
  {% for col in mydata[0] %}
    {% if col[0] != "link" %}
      {% if forloop.first %}
        <th>{{ col[1] }}</th>
      {% else %}
        <th class="table-right">{{ col[1] }}</th>
      {% endif %}
    {% endif %}
  {% endfor %}
  </thead>

  <tbody>
  {% for row in mydata %}
    {% if forloop.first %}
      {% continue %}
    {% endif %}
    <tr>
    {% for cell in row %}
      {% if forloop.first and row["link"] %}
        <td><a href="https://www.strava.com/activities/{{ row["link"] }}">{{ cell[1] }}</a></td>
      {% else %}
        {% if cell[0] != "link" %}
          {% if forloop.first %}
            <td>{{ cell[1] }}</td>
          {% else %}
            <td class="table-right" >{{ cell[1] }}</td>
          {%endif%}
        {% endif %}
      {% endif %}
    {% endfor %}
    </tr>
  {% endfor %}
  </tbody>
</table>


## Cycling trips

<div class="container">
  <div class="row row-cols-2">
    <div class="col">
      <a data-flickr-embed="true" data-header="true" data-footer="true" href="https://www.flickr.com/photos/faoch/albums/72157680080387628" title="Cycling Taiwan"><img src="https://live.staticflickr.com/65535/40735736163_3deaed2161_n.jpg" width="320" height="240" alt="Cycling Taiwan"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
    </div>
    <div class="col">
      <a data-flickr-embed="true" data-header="true" data-footer="true" href="https://www.flickr.com/photos/faoch/albums/72157666638728105" title="The Yorkshire Dales Cycle Way"><img src="https://live.staticflickr.com/1583/26140148516_cd6074cd38_n.jpg" width="320" height="240" alt="The Yorkshire Dales Cycle Way"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
    </div>
    <div class="col">
      <a data-flickr-embed="true" data-header="true" data-footer="true" href="https://www.flickr.com/photos/faoch/albums/72157647734510758" title="The Great Glen Way"><img src="https://live.staticflickr.com/3895/15196741619_715be2ebe1_n.jpg" width="320" height="240" alt="The Great Glen Way"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>
    </div>
  </div>
</div>


## The machines

### For the road

{% include figure.html path="assets/img/merida_scultura_7000E.jpg" class="img-fluid rounded z-depth-1" zoomable=true %}
Merida Scultura 7000-E

Specs:

- Carbon frame
- Shimano Ultegra Di2 RT8000 groupset
- Shimano Ultegra hydraulic disc brakes
- 52/36 chainset

### For touring

{% include figure.html path="assets/img/ridgeback.jpg" class="img-fluid rounded z-depth-1" zoomable=true %}
Rigdgeback World Panorama 2015.

Specs:

- Reynolds 725 chrome-moly steel frame
- Shimano Deore XT (rear), Sora (front), Sora ST shifters
- 48/36/26 chainset

