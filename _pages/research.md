---
title: "Earth System & Global Change Lab - Research"
layout: textlay
excerpt: "Allan Lab -- Research"
sitemap: false
permalink: /research/
---

# Research

I am an earth system scientist. I am interested in how climate determines vegetation, how vegetation reshapes our climate, and many other global change issues. My long-term goal is to develop a more mechanistic and predictive ecological climatology. This is very important given that the human-dominated Earth has deviated from her equilibrium state and we all are at risk that self-reinforcing feedbacks of the Earth may push the planet to extreme states (e.g. Hothouse Earth). Among the feedbacks, the biogeophysical feedbacks within the Earth System coupled with direct human influences of the biosphere are the key. To achieve this long-term goal, we need to increase observations for quantification of human impacts on the biosphere, and to advance our understanding on the feedbacks of biosphere change to water cycle and climate system. I have long worked on understanding and modelling the role of vegetation in the terrestrial water cycle and the global climate system, determining the response of the biosphere to human impacts, and quantifying how the biosphere response feeds back to the water cycle and climate system. My research draws heavily upon transdisciplinary inference, process-based approaches, and data-driven machine learning to develop mechanistic and predictive ecological climatological models. My background gives me a unique perspective for addressing questions about the interactions between the biosphere and the atmosphere, and their implications to global environmental change.

Global climate change is a major challenge of our generations that determines the sustainable development of human society. Tropical forests and wetlands are important "stabilizers" for the Earth's climate system. However, global agriculture expansion is rapidly decreasing and degrading tropical forest and wetland ecosystems. It is likely caused by the fact that our demand for food and energy is dramatically increasing along with the population booming and the economic development, yet the land suitable for farming in the temperate regions has basically been converted into agricultural land; thus global agriculture has to expand from the temperate regions into the tropical regions (Searchinger et al., 2019; Song et al., 2018; Zeng et al., 2018a, b). This pattern of global land cover and land use change is a critical factor for the current and future climate change, via interactions among various layers of the climate system (IPCC, 2014). Climate change, in turn, can cause degradation of tropical ecosystems (forests and wetlands in particular). Degradations of tropical forests and wetlands may lead to a collapse of the Earth’s climate system. My research, with the support of Southern University of Science and Technology, will focus on the dynamics of tropical agriculture, forests, wetlands and climate in the context of global change.


## Highlights

(For a full list see [Publication](https://www.zhenzhongzeng.com/publications) or go to [Google Scholar](https://scholar.google.com/citations?user=GsM4YKQAAAAJ&hl=en), [Researchgate](https://www.researchgate.net/profile/Zhenzhong_Zeng))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>





