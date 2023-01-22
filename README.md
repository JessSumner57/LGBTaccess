# LGBTaccess

---
bibliography: bio.bib
csl: harvard-cite-them-right.csl
title: Individual Reflection
format: 
  pdf:
    include-in-header:
      text: |
        \addtokomafont{disposition}{\rmfamily}
    #documentclass: report
    mainfont: "Spectral" # https://fonts.google.com/specimen/Spectral
    sansfont: "Roboto"   # https://fonts.google.com/specimen/Roboto
    monofont: "Inconsolata" # https://fonts.google.com/specimen/Inconsolata
    papersize: a4
    geometry:
      - top=25mm
      - left=40mm
      - right=30mm
      - bottom=25mm
      - heightrounded
    toc: false
    number-sections: true
    colorlinks: true
    highlight-style: github
---
Literature Review
Current academic literature on green space accessibility in the UK, largely focuses on the amount of availability as it relates to the population at large, with some recent attention being drawn to equal access for England’s Black, Asian, and Minority ethnic population (BAME) through initiatives by Friends of the Earth (2021). However, due to the newness of the ‘Sexual Orientation’ data to the UK census, more information is now available to analyse where LGB+ identifying people are, and what types of land is most available to them. Environmental LGB+ literature on the subject thus far focuses on the need for the LGB+ community to have a safe and inclusive space to convene, as a community that may feel unsafe in their own homes, living spaces, and workplace. Thus far, such reports as Arup’s on “Queering Public Space” (n.d.), discuss the need for further recognition of how public spaces need to be made to feel safe, especially for groups who face fears of experiencing hate-crime, and often feel the need to hide their identities in public spaces. An aspect that is important to consider for greenspace management it to draw attention to hostility and exclusion experienced by the LGB+ community. As explored by Friends of the Earth, “Access to Green Space: Are you missing out?”, this report sheds light on how communities within England do not receive equal access to different types of green space (Friends of the Earth n.d.). For the purpose of this report, equal access, signifies the compared reality to those who identify as straight, and often do not face the same discrimination or fear of how their identity may ostracize them as in society as LGB+ communities do. Moreover, it is well documented that particularly ethnic minorities are particularly excluded from green spaces, but it is worth noting how other marginalized communities have or do not have access. Specifically, access to green space, especially in a community-centric way, combats loneliness, improves mental-health, and is restorative for physical well-being. LGB+ groups often suffer from marginalization and exclusion from friends and families (Nicola 2021). It is worth mentioning, that of these groups, it is often ethnic minority LGB+ communities who face the most discrimination and often the least amount of accessibility to safe spaces in the urban environment. Therefore, having safe, accessible spaces for the LGB+ community is pertinent for its health and the ability to identify and participate in one’s community. 
Data
The population data covers the census question on sexual orientation where 44.9 million people aged 16 and over, answered the question. Of this sample size, 98.4% identified as heterosexual whereas only 3.2%, answered that they identify with the LGB+ orientation, meaning Lesbian, Gay, Bisexual, or other sexual orientation. In this report, the sample size has been condensed to account for only those who identified with LGB+ (Roskams, M. 2023). Unfortunately, this does not cover people who identify as Transgender, which is a community who often feels the most stigmatization in public space, and thus why the common acronym LGBT+ is shortened to LGB+. Moreover, the data in this report consists of Average garden size for flats in built up area (m2), Average size of nearest park or public garden (m2), Average combined size of parks or public gardens within 1,000 m radius (m2), those who identified as Straight in the sexual orientation part of the UK’s 2021 census, as well as the combined valued of those who identified as “Gay or Lesbian”, “Bisexual”, “Pansexual”, “Asexual”, and “Queer” (Roskams, M. 2023). Averages of different types of green spaces along with their proximity were selected because it allowed for a better understanding of what types of green space LGB+ communities have access to, and if these greenspaces had the possibility to facilitate community cohesion. Similar to the report by Fields in Trust titled “The ten-minute walk and why it’s important” (n.d), this report utilized green space data collected from Friends of the Earth who collated this data from the Office of National Statistics on gardens, along with data on public green space in Local Authority Districts. A green space in this report is defined by the ONS’s definition of “what is public green space” which doesn’t include public allotments nor wildlife sites or beaches. Also, it doesn’t consider the actual quality of the green space. Similarly, another factor that is not feasibly measured through this dataset is the sociability when assessing ‘Average Garden size of flats in built up area(m2), one can derive the assumption that having a smaller garden near a mass of flats, is unlikely to facilitate sociability, and thus is a form of an outlier if considering spaces for community building. 
Explanation of methodology
H_(0 The LGBT community has equal access to green space as the straight identified population.) H_(1 The LGBT community does not have equal access to green space as the straight identified population.)
To explore this relationship, I took a clustering approach because multiple variables are considered over a wide area of space, both geographically and mathematically. Clustering allowed for a better visualization of patterns of how to identify areas where LGB+ groups have greater or lesser access to green space compared to straight people. Moreover, clustering allowed me to reduce the dimensions of my data, as I was analysing a segment of the population against a measurement of area. Once I had rescaled my data using MinMaxScaler, because of the variability in the range of the data. I also assessed the K means value to gain insight into how many clusters would form and to further understand where these points of similarity between the data might lie. The quality of this clustering was tested using SSE and reinforced using a silhouette score test. Lastly, for a better understanding of where clustering occurs, the data was visualized using several different scatter plots, as well as mapped.  
Presentation of results
Based on the results, where there are higher densities of LGB+ community members there are subsequently lower levels of volume of green space. It is worth noting that there were several outliers when this data was visualized according to data points specific to London. The most notable areas of clustering, when geography was used as a comparative factor, included Manchester, London, and Bristol, all of which have higher percentages of the LGB+ community located centrally with far lower numbers on the periphery. Furthermore, LGB+ and Average combined size of parks or public gardens within 1,000 m radius were clustered in areas of Hackney and Victoria Park. Moreover, as much of the larger green spaces happen to be on the periphery, this also means that it is less accessible to the LGB+ compared to that of the Straight community. Likewise, flats that have larger garden areas tend to also be located on the periphery, where there are below average values of the LGB+ community. As demonstrated by Figure 1, LGB+ community have access broadly to smaller parks than Straight people do. This allowed for an understanding of the contrast between the considered population and the contrast in volume of green-space available to each respective group. 

 
To further delve into the clusters, an elbow plot, as demonstrated at Figure 3, suggests that the optimal number to base the following analysis on is 4. To further assess the number of clusters, the silhouette score was calculated reduced to 'Average Garden size for flats in built up area', 'Average size of nearest park or public garden (m2)' and ', 'LGB+', from this I received a score of 0. 0.42 which is significant because it shows there it demonstrates that these variables are reasonably close to each other in relation with an optimal k-means of around 4. 




K-means in this scenario allows me to assess what Local Authority Districts would have similar values of average size of gardens, average size of parks, and percentage of population that is LGB+ together, as well as which LAD’s have small gardens, small parks, and low percentage of LGB+ population. Based on my data points, it appears that generally, with a few outliers at (3,1) and (5.2, 0.8) the if cities with smaller parks tend to also have a lower percentage of LGB+ population, in urban areas. 


In Figure 3, around the 2.8 and 3.5 value of amount percentage of LGB+ community, it may be thought to be clustering where within major cities there is similarly a large park located near a higher LGB+ population. Whereas, in Figure 4 once the data is standardised and the data is plotted based on means, we see general proximity between the clusters, when k is 4. Moreover, the centroids are visible through deriving the k-means values from the scaled data and further plotting the relationship through coordinates between the area data and the population, as demonstrated in Figure 5. 
                                              Figure 5 Centroid's based on k-means clustering






Limitations & Conclusion
Some of the inherent limitations that are associated with conducting k-means clustering subsequently effect this model. For one, the need to know the number of clusters requires an extra step of splitting the data which may not necessarily signify the original intended purpose of grouping. Additionally, because of its sensitivity to outliers, and given the geographic scope of this analysis, there is an outlier effect when it comes to having large parks or flat gardens, in areas that can allow for it in conjunction with the number of LGB+ community members. Lastly, it is important to note, that since the census question concerning identifying LGB+ is a relatively sensitive, many people may not feel comfortable self-identifying. 
Yet, based on clustering, it is reasonable to say that green space as portrayed through size and distance, is more inaccessible to LGB+ people than to that of straight people. Of course, it is important to note that clustering is not a very robust methodology and that other variables that could be explored, such as income of population near greenspace, comparing the LGB+ versus straight population to proximity to waterways, and proximity to transportation, all of which are variables that can contribute to accessibility and community. 
 
