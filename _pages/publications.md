---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

## Published:
*You can also find my published articles on my [Google Scholar profile](https://scholar.google.com/citations?user=efcvlPIAAAAJ&hl=en)*

Jaramillo, F., **Aminjafari, S**., Castellazzi, P., et al., **2024**. The Potential of Hydrogeodesy to Address Water-related Problems and Sustainability Challenges. Water Resources Research, 60(11), e2023WR037020. [DOI](https://doi.org/10.1029/2023WR037020)

**Aminjafari, S**., Frappart, F., Papa, F., Brown, I., and Jaramillo, F., **2024**. Enhancing the Temporal Resolution of Water Levels from Altimetry Using D-InSAR: A Case Study of 10 Swedish Lakes. Science of Remote Sensing, 10, 100162. [DOI](https://doi.org/10.1016/j.srs.2024.100162)

**Aminjafari, S**., Brown, I., and Jaramillo, F., **2024**. Evaluating D-InSAR Performance to Detect Small Water Level Fluctuations in Two Small Lakes in Sweden. Environmental Research Communications, 6(9), 091006. [DOI](https://doi.org/10.1088/2515-7620/ad7701).

**Aminjafari, S**., Brown, I.,  Frappart, F., Papa, F., Blarel F., Vahidi Mayamey, F., and Jaramillo, F., **2024**. Distinctive Patterns of Water Level Change in Swedish Lakes Driven by Climate and Human Regulation. Water Resources Research, 60(3), e2023WR036160. [DOI](https://doi.org/10.1029/2023WR036160)

**Aminjafari, S**., Brown, I., Vahidi Mayamey, F., and Jaramillo, F., **2024**. Tracking Centimeter-Scale Water Level Changes in Swedish Lakes Using D-InSAR. Water Resources Research, 60(2), e2022WR034290. [DOI](https://doi.org/10.1029/2022WR034290)

**Aminjafari, S**., Brown, I., Chalov, S., Simard, M., Lane, C.R., Jarsjö, J., Darvishi, M. and Jaramillo, F., **2021**. Drivers and extent of surface water occurrence in the Selenga River Delta, Russia. Journal of Hydrology: Regional Studies, 38, p.100945. [DOI](https://doi.org/10.1016/j.ejrh.2021.100945)

Darvishi, M., Destouni, G., **Aminjafari, S**. and Jaramillo, F., **2021**. Multi-Sensor InSAR Assessment of Ground Deformations around Lake Mead and Its Relation to Water Level Changes. Remote Sensing, 13(3), p.406. [DOI](https://doi.org/10.3390/rs13030406)

Liu, D., Wang, X., **Aminjafari, S**., Yang, W., Cui, B., Yan, S., Zhang, Y., Zhu, J. and Jaramillo, F., **2020**. Using InSAR to identify hydrological connectivity and barriers in a highly fragmented wetland. Hydrological Processes, 34(23), pp.4417-4430. [DOI](https://doi.org/10.1002/hyp.13899)

Soltanpour, A., Pirooznia, M., **Aminjafari, S**. and Zareian, P., **2018**. Persian Gulf and Oman sea tide modeling using satellite altimetry and tide gauge data (TM-IR01). Marine Georesources & Geotechnology, 36(6), pp.677-687. [DOI](https://doi.org/10.1080/1064119X.2017.1366608)

**Aminjafari, S**., **2017**. Monitoring of Masjed-Soleiman embankment dam’s deformation using a combination of Interferometric Synthetic Aperture Radar (InSAR) and finite element modeling. Geodesy and Cartography, 43(1), pp.14-21. [DOI](https://doi.org/10.3846/20296991.2017.1299842)


{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
