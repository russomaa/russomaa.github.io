---
layout: page
permalink: /research/
title: Academic Publications
pubs:

   - title: "Towards an Ontology-Driven Approach to Document Bias"
     author: "Russo Mayra and Vidal Maria-Esther" 
     journal: "Journal of Artificial Intelligence Research"
     year: "2025" 
     url: "http://dx.doi.org/10.1613/jair.1.19388"
     
   - title: "Tracing Bias for Fairer Content-Based Misinformation Detection" 
     author: "Russo Mayra and Merenda Flavio and Gomez-Perez Jose Manuel and Vidal Maria-Esther"
     journal: "Companion Proceedings of the ACM on Web Conference 2025"
     year: "2025"
     url: "http://dx.doi.org/10.1145/3701716.3717534" 

   - title: "Employing Hybrid AI Systems to Trace and Document Bias in ML Pipelines"
     author: "Russo Mayra and Chudasama Yasharajsinh and Purohit Disha and Sawischa Sammy and Vidal Maria-Esther"
     journal: "IEEE Access" 
     year: "2024"
     url: "http://dx.doi.org/10.1109/ACCESS.2024.3427388" 

   - title: "Articulation Work and Tinkering for Fairness in Machine Learning"
     author: "Fahimi Miriam and Russo Mayra and Scott Kristen M. and Vidal Maria-Esther and Berendt Bettina and Kinder-Kurlanda Katharina" 
     journal: "Proceedings of the ACM on Human-Computer Interaction" 
     year: "2024" 
     url: "http://dx.doi.org/10.1145/3686973"

   - title: "Bridging Research and Practice Through Conversation: Reflecting on Our Experience"
     author: "Russo Mayra and Jorgensen Mackenzie and Scott Kristen M. and Xu Wendy and Nguyen Di H. and Finocchiaro Jessie and Olckers Matthew"
     journal: "Proceedings of the 4th ACM Conference on Equity and Access in Algorithms Mechanisms and Optimization" 
     year: "2024"
     url: "http://dx.doi.org/10.1145/3689904.3694705"

   - title: "Leveraging Ontologies to Document Bias in Data"
     author: "Russo Mayra and Vidal Maria-Esther"
     journal: "Proceedings of the Second Workshop on Fairness and Bias in AI"
     year: "2024"
    
   - title: "Policy advice and best practices on bias and fairness in AI"
     author: "Alvarez Jose M. and Colmenarejo Alejandra Bringas and Elobaid Alaa and Fabbrizzi Simone and Fahimi Miriam and  Ferrara Antonio and Ghodsi Siamak and Mougan Carlos and Papageorgiou Ioanna and Reyero Paula and Russo Mayra and Scott Kristen M. and State Laura and Zhao Xuan and Ruggieri Salvatore"
     journal: "Ethics and Information Technology"
     year: "2024"
     url: "https://doi.org/10.1007/s10676-024-09746-w"
     
   - title: "Tracing the Impact of Bias in Link Prediction" 
     author: "Russo Mayra and Sawischa Sammy Fabian and Vidal Maria-Esther"
     journal: "Proceedings of the 39th ACM/SIGAPP Symposium on Applied Computing"
     year: "2024"
     url: "http://dx.doi.org/10.1145/3605098.3635912" 

   - title: "Empowering machine learning models with contextual knowledge for enhancing the detection of eating disorders in social media posts"
     author: "Benitez-Andrades Jose Alberto and Garcia-Ordas Maria Teresa and Russo Mayra and Sakor Ahmad and Fernandes-Rotger Luis Daniel and Vidal Maria-Esther"
     journal: "Semantic Web"
     year: "2023"

   - title: "A Multidisciplinary Lens of Bias in Hate Speech" 
     author: "Reyero-Lobo Paula and Kwarteng Joseph and Russo Mayra and Fahimi Miriam and Scott Kristen and Ferrara Antonio and Sen Indira and Fernandez Miriam"
     journal: "Proceedings of the International Conference on Advances in Social Networks Analysis and Mining" 
     year: "2023"
     url: "http://dx.doi.org/10.1145/3625007.3627491"      

---

## Peer-reviewed Publications

[ORCiD](https://orcid.org/0000-0001-7080-6331)

<!-- {% assign thumbnail="left" %} -->

{% for pub in page.pubs %}
{% if pub.image %}
{% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
{% endif %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.year}}* {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}
{% if pub.media %}<br />Media: {% for article in pub.media %}[[{{article.name}}]({{article.url}})]{% endfor %}{% endif %}

{% endfor %}
