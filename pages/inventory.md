---
title: Film Inventory
layout: table
permalink: /inventory.html
custom-foot: js/inventory.html
side-image: /assets/svg/inventory-vert.svg
top-image: /assets/svg/inventory-flat.svg
---

## Film Inventory

The table below provides sorting and basic search of an inventory of the **11,140 films** that were donated to Special Collections from Main Street Video. 

{% assign genres = site.data.mainstreet_inventory | map: 'genre' | compact | uniq %}
<div class="row justify-content-end">
    <div class="col-md-3 text-end"><label for="groupSelect" class="form-label">Filter by Genre: </label></div>
    <div class="col-md-3">
        <select class="form-select" id="groupSelect" aria-label="select genre">
            <option selected value="all">All Genres</option>
            {% for g in genres %}
            <option value="{{ g | strip }}">{{ g | strip }}</option>{% endfor %}
        </select>
    </div> 
</div>

<div class="table-responsive-md">
    <table id="item-table" class="table table-striped">
        <thead>
            <tr>
                <th scope="col">Title</th>
                <th scope="col">Genre</th>
                <th scope="col">Type</th>
                <th scope="col">Box Number</th>
            </tr>
        </thead>
    </table>
</div>
