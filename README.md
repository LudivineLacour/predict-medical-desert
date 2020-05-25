# Medical Desert

According to a [report from DREES](https://drees.solidarites-sante.gouv.fr/IMG/pdf/er1144.pdf) on doctors density in France, the ratio of population living in a medical desert is growing from 3.8% to 5.7%.

Some people have to drive many kilometers to find a doctor which can be hard for some of them having a limited way of commute (old people, people without any driving license). Also it would also mean that it could take more time to get a consultation from the moment you are identified as sick, and so life can depend on it. 

**Can we predict the medical desert of an area?**

Sub-questions:
- What is a medical desert? How is defined a medical desert?
- What is the proportion of medical desert in France? 
- Is there any area with an over-density of doctors?
- What factors would impact the lack of doctors in an area? 
- Can an area improve the situation by playing on these factors? 
- What could be the solution to improve the situation of medical desert?

DREES identifies medical desert through the APL indicator (Accessibilité Potentielle Localisée) which gives the potential number of consultation per resident per year for a given area. If the area has the indicator under 2.5C/r/y, it is considered as medical desert. 

## Project limitation

So my target would be the APL indicator. 

Altough the medical desert can be applied for any type of doctors (general practitioner, specialists, etc.), for this project we will only talk about general practitioners because the target is based on this type of doctors. 

Considering that liberal doctors are free to move wherever they want, the quality of life or the ecominic state of an area can impact much the area of practicing. 

Assumptions for features impacting medical desert in a given area (city):
- [x] Population / area density 
- [x] Population growth
- [ ] Population projection and growth projection
- [x] Population average age
- [ ] Birth rate
- [x] Socio-Professional Category
- [x] Level of poverty
- [x] Unemployement rate
- [x] Number of medical infrastructures
- [x] Level of medical education
- [x] Level of city amenities / investment in city amenities
- [ ] Expense in healthcare (per resident in a city)
- [ ] Average temperature
- [x] Number of doctors
- [ ] Doctors average age

Data Sources: 
- APL: [data.drees.sante.gouv.fr](http://www.data.drees.sante.gouv.fr/ReportFolders/reportFolders.aspx)
- Number of doctors: web-scraping doctolib
- Socio-Professional Category: [INSEE - Évolution et structure de la population en 2016](https://www.insee.fr/fr/statistiques/4171334?sommaire=4171351#consulter)
- Level of poverty, Population average age, area density, Level of city amenities, Unemployement rate: [INSEE - Base comparateur de territoires](https://www.insee.fr/fr/statistiques/2521169#consulter)
- Level of medical education: [INSEE - Base permanente des équipements (BPE)](https://www.insee.fr/fr/statistiques/3568638?sommaire=3568656#consulter)