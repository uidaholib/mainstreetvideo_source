---
title: About
layout: essay
permalink: /about.html
# include CollectionBuilder info at bottom
credits: false
# Edit the markdown on in this file to describe your collection
# Look in _includes/feature for options to easily add features to the page
side-image: /assets/svg/about-vert.svg
top-image: /assets/svg/about-flat.svg
---


{% include feature/nav-menu.html sections="About the Collection;Historical Background;Timeline;Credits" %}


## About the Collection 

Main Street Video presents 34 oral history interviews captured in 2021 exploring the phenomena of the "local video store" and documenting the history of Howard Hughes Video and the Main Street Video Co-op in Moscow, Idaho. The interviews were conducted by former board member Monique Lillard and former employee and store manager Beau Newsome. The exhibit also features a series of [interpetive essays]({{'/essay/' | relative_url }}) written by Milo Muise (MFA '22) that contextualize those interviews with larger local and historical trends. 

{% include feature/image.html objectid="https://webpages.uidaho.edu/library/spec/harvester/objects/small/vid-store_sm.jpg" caption="Geoff Crimmins/Daily News photo. - Store front of Howard Hughes Video" link="https://harvester.lib.uidaho.edu/posts/2024/03/31/video.html"%}

Howard Hughes Video / Main Street Video Co-op was a cornerstone of Moscow's unique culture and one of the last remaining video stores in the country.
The University of Idaho Archives and Special Collections adopted their inventory of films when they closed and launched this oral history project to document the history and impact of this important local institution. 
Interviews were recorded via Zoom with employees, customers, and other people associated with the store.

{% capture dulce %}For more on the collection and the history of the video store in Moscow, see this [Harvester blog post by Dulce Kersting-Lark](https://harvester.lib.uidaho.edu/posts/2024/03/31/video.html). {% endcapture %}

{% include feature/marginnote.html id="intro" text=dulce %}

To view a list of particants: <button data-bs-toggle="modal" data-bs-target="#creditsModal" type="button" aria-label="Open up a Credits Modal for the site" class="btn btn-outline-info fs-4">Roll Credits!</button>

(or check out the [list below](#credits))

## Historical Background

In 1977, the first compact yet still semi-affordable video home system, or VHS, became available to the general American public. Vast improvements in technology allowed people to use a video cassette recorder, or VCR, to record live TV to watch on their own time or purchase pre-recorded content such as feature films that people could watch in their own homes. To capitalize on the national trend, entrepreneur Howard Hughes of Moscow opened Howard Hughes Appliance, TV, and Video Store in 1978. He quickly learned in order to sell VCRs, the store needed to also stock pre-recorded VHS tapes to demonstrate how to use the machines. Once people bought the machines, Hughes then offered up the tapes for people to rent.  

Hughes sold the business in 1996 to Don Frei and Kevin Peterson, who kept the rental aspect of Howard Hughes Appliances as it remained a lucrative part of the business and beloved store in town. In the late 1980s and early 1990s Howard Hughes Video partnered with the Associated Students of the University of Idaho (ASUI) to sponsor the low-cost movies played in the Borah Theatre on the U of I campus offered for the entertainment of students. Rental discount ads and articles about what movies the store offered frequently turned up in the Argonaut student newspaper.  

When the new owners relocated the appliance store to a larger space in 2000, the video rental portion stayed at the current location on Washington Street downtown Moscow but kept the same name. Frei and Peterson eventually sold Howard Hughes Video to four Moscow residents and business owners in 2007, Gary Myers, Kelly Moore, Pat Engle and Deb Reynolds. They incorporated their business as Main Street Video, Inc, but also kept the business name as Howard Hughes Video. Shortly after purchasing the video store, they moved it to 520 S. Main Street, where it remained until its closure in 2020.  

{% include feature/image.html objectid="/assets/img/mainstreet-video-argonaut.jpg" caption="Outside of the Main Street Video Co-Op, Saydee Brass, Argonaut" link="https://www.uiargonaut.com/2020/05/04/mainstreet-video-closes-its-door/" %}

Facing economic troubles in 2015, the owners of Howard Hughes Video wanted to sell the business. In order to save the business, a group of Moscow residents came together to find a way to save the video rental store from closing. They ultimately decided to buy the store and turn it into a cooperative business, creating the Main Street Video Cooperative. Organized as a nonprofit, the Main Street Video Co-op operated with a Board of Directors and all customers had the opportunity to become members or "owners" for a fee of $200. Ownership was not compulsory to rent movies but did come with perks and other discounts, and fees and any donations collected helped the Co-op pay for the purchase of the business from the current owners. The Main Street Video Co-op officially took charge of the store on January 1st, 2018. 

The economic hardships created by the COVID-19 pandemic did not spare the video rental store, and the Main Street Video Co-op made the difficult decision to close permanently in March of 2020. The dream of maintaining a diverse collection of films continued, however, and the entire film library was transferred to the Kenworthy Performing Arts Center, a historic theatre and community performing art venue located next door to the Co-op. The Kenworthy cherished the value of the collection and so planned to reach out to donate parts to other local non-profits and libraries that could benefit from the collection. To recoup costs however, the Kenworthy ultimately sold to the public a large portion of the collection, then donated the rest to the University of Idaho Library Special Collections and Archives.  



## Timeline

- 1978: Howard Hughes (of Moscow) opened Howard Hughes appliance/TV/video store. Needed VHS tapes to demonstrate how machines worked, then started renting them. Advertised them on local radio station KRPL.  
    - Was Murphy’s Appliance, became Murphy-Hughes Appliance (1980 phone book, incorporated in Feb 1981). Located at 715 N. Main. 
    - 1990 phonebook: HH Appliances (with video) 114 E. Fifth  
- 1996: Don Frei and Kevin Peterson purchased appliance/TV/video store from Howard Hughes 
- March 2000 (planned according to Nov 1999 DNews article): HH Appliance, Video and Sleep Shop moved to 908 W. Pullman Rd. Video store staying at 407 S. Washington. 
- May 2007: Moscow residents Gary Myers, Kelly Moore, and Deb Reynolds purchased Howard Hughes Video. Incorporated as Main Street Video, Inc. 
- 2007: 114 E. Fifth St 
- Around 2008: moved to 520 S. Main St.  
- August 2012: ‘Howard Hughes Video’ officially filed in Idaho as assumed business name 
- (sometime between 2013 and 2015): Pat Engle, Neil Franklin, Kelly Moore, and Deb Reynolds are owners 
- 2015/16: Moscow Food Co-op joins with staff of Howard Hughes Video to create the Main Street Video Cooperative. Bylaws approved December 2015. 
- March 2020: Main Street Video Co-op closes 

## Credits

<h3>Interviewers</h3>
<p>Monique Lillard<br>Beau Newsome</p>
{%- assign people = site.data[site.metadata] | where_exp: 'item','item.interviewee'  -%}
{%- assign people = people | sort: 'interviewee' %}
<h3>Narrators</h3>
<p>
{% for p in people %}
<a href="{{ p.objectid | append: '.html' | prepend: '/items/' | relative_url }}">{{ p.interviewee | replace: ';',' & ' }}</a><br>
{% endfor %}</p>
<h3>Crew</h3>
<p>Interpretive Essayist: Milo Muise</p>    
<p>Producer: Courtney Berge</p>
<p>Metadata and Processing Work: Courtney Berge</p>
<p>Producer: Robert Perret</p>
<p>Trailer Producer: Hanwen Dong</p>
<p>Design: Devin Becker</p>
<p>Vintage Design/Metadata Guru: Klytie Xu</p>
<p>Transcriptionista: Andrew Weymouth</p>
<p>Media Archivist: Kevin Dobbins</p>
<p>Technically of some help: Evan Williamson</p>
<p>Writer/Researcher: Amy Thompson</p>
<p>Digital Archival Consultant: Sara Szobody</p>
<p>Archival Consultant: Dulce Kersting-Lark</p>