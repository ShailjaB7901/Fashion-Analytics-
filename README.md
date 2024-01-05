# Fashion Analytics: unveiling cultural influences
## Introduction:

### Background:
The global fashion landscape is an ever-evolving tapestry woven with threads of diverse cultural influences. As fashion becomes increasingly interconnected, the contributions of Indian designers to major fashion weeks play a pivotal role in shaping this vibrant fabric. The fusion of traditional Indian aesthetics with contemporary trends not only reflects the dynamism of the fashion industry but also underscores the cultural significance embedded in every design.

In recent years, the spotlight has intensified on Indian designers participating in major fashion weeks, such as those held in Paris, London, and New York. These designers bring a unique perspective, blending rich cultural heritage with cutting-edge fashion trends. Recognizing the profound impact of cultural narratives in fashion, this study endeavors to dissect the nuanced interplay between tradition and modernity within the works of Indian designers on the global stage.


**Purpose Statement: Exploring the Intersection of Data Science and Fashion**

In embarking on the project exploring the global fashion landscape and the distinctive contributions of Indian designers, my purpose is rooted in the convergence of data science and the dynamic world of fashion. This project stems from a profound curiosity about the intricate patterns that weave together tradition and modernity on international runways.

1. **Fusion of Creativity and Analytics:** The intersection of creativity and analytics has always fascinated me. By delving into the fashion industry, particularly the works of Indian designers, I aim to showcase how data science can unveil underlying trends and narratives, providing a comprehensive understanding of the intricate balance between heritage and innovation.

2. **Cultural Significance:** The project's core purpose is to unravel the cultural narratives embedded in the designs showcased during major fashion weeks in Paris, London, and New York. By leveraging advanced text analytics, I aspire to shed light on how traditional Indian aesthetics merge with contemporary global trends, influencing the broader conversation in the fashion world.

3. **Recognition of Indian Designers:** Another crucial aspect of this project is to recognize and celebrate the contributions of Indian designers on the global stage. By focusing on names like Bibhu Mohapatra, Gaurav Gupta, and others, I aim to showcase their unique perspectives and emphasize their role as cultural ambassadors, influencing not just fashion trends but also fostering a deeper appreciation for diversity.

4. **Bridge Between Technology and Fashion:** As a data analyst, I see this project as an opportunity to bridge the gap between technology and the creative fields. By employing methodologies such as text analytics, I hope to contribute to the growing dialogue on how data science can enhance and complement the artistic realm, fostering innovation and pushing the boundaries of design.

In essence, this project serves as a testament to my belief in the transformative power of data science to not only analyze but also appreciate the rich tapestry of cultures woven into the fabric of global fashion. Through this exploration, I aim to inspire a greater understanding of the symbiotic relationship between data science and the creative expression inherent in the world of haute couture.

### Objective:
The primary objective of this study is to delve into the textual landscape surrounding Indian designers during Paris, London, and New York Fashion Weeks. By employing advanced text analytics, I aim to unravel the extent to which cultural heritage influences their creative expressions.

This study is like unraveling a story told by Indian designers in global fashion. By spotting shared words and themes, I am contributing insights into how tradition and modern style come together in the world of international fashion.

### Fashion designers in View:
#### Newyork:

1. Bibhu Mohapatra
2. Naeem Khan
3. Mayyur Girotra
4. Archana Kochhar

#### Paris:

1. Gaurav Gupta
2. Rahul Mishra
3. Vaishali Shadangule

#### London:

1. Harri
2. Supriya lele
3. Ashish Gupta
4. Priya Ahluwalia


## Methodology

### Previously employed methodology:

#### 1. Data Collection:
Fashion articles for 2023 from reputable sources such as Vogue, Grazia, Harper's Bazaar covering Paris, London, and New York Fashion Weeks were scraped Beautiful soup. The focus was on obtaining diverse and representative samples.

#### 2. Data Cleaning and Preprocessing:
Text data was organized and labeled as separate sentences, then underwent rigorous cleaning procedures to remove irrelevant information, and lemmatization was applied to standardize word forms for analysis. The cleaned text was converted into text files for each, Paris, NewYork and London fashion week.

#### 3. Fashion Term Compilation:
A list of 600 fashion terms was compiled, incorporating terminology associated with both traditional and contemporary fashion, including fabrics, colours, fashion cuts, textiles, patterns etc.

#### 4. Matching and Frequency Count:
The compiled fashion terms were matched with the cleaned data, and the frequency of each term was counted to identify the most commonly appearing words.
The frequency and words were plotted on bar graphs to visualise commonalities, using Matplotlib.

#### 5. Frequency Analysis:
The top N most frequent terms across all three fashion weeks were identified, indicating potential shared cultural influences.

#### However, The code for this (which I previously published) was not only extensive, but also involved a lot of manual work. As I would have to read through each article and sentence and select which ones to delete. This could result in not only important information being deleted, but also excess text from advertisements interefering with the integrity of the results. Which is why I made the following modifications:

#### 1. Using newspaper3k library for the cleaning tasks

I discovered Newspaper3k and implemented the 'Article' module to perform the cleaning tasks. This ensured only title and main article contents got scraped. There was no longer a need to read through entire document to delete irrelevant content or messy formatting. 


#### 2. Creating my own library, pyFashion.

Within the library I created a module "Fashionanalyzer" which takes provided text, lemitizes it, and matches it with the inbuilt fashion vocabulary words, and returns the frequency of each word. This shortened and made the code a lot cleaner, because there is no loner a need to write nested functions that split the text and lemmitize it. pyFashion has spacy dependencies to do it. 



## Results and discussions

*Embroidery* emerges as a prevailing trend among the works of these designers, a testament to their deep connection with Indian heritage. This rich and significant facet of the country’s cultural legacy persists and evolves, underscoring the enduring importance of this art form. Delving into the history, Indian embroidery boasts a diverse legacy spanning thousands of years. Its origins trace back to the Indus Valley Civilization (3300 BCE to 1300 BCE), and it flourished further during the Mughal period in the 16th century. The art of embroidery, a tapestry of tradition and innovation, has continued its journey through the centuries, playing a pivotal role in shaping Indian culture, particularly in the domain of fashion.

A parallel narrative unfolds with the second prominent trend — *draping*. This owes its prominence to the iconic saree, an integral element of Indian culture. Each state contributes its unique style to the art of saree draping. Additionally, the shawl, introduced to India by Persian settlers in the late 14th century, adds another layer of cultural richness.

In conclusion, the exploration of prevailing trends among Indian designers on the global stage illuminates not only their profound connection with the country's rich cultural heritage but also their ability to transcend borders and captivate international audiences. The mastery of embroidery and the art of draping, deeply rooted in India's historical tapestry, showcase the designers' commitment to preserving tradition while embracing innovation.

As these designers navigate the global fashion landscape, their influence goes beyond trends; it becomes a cultural dialogue, fostering a deeper appreciation for the diversity and craftsmanship inherent in Indian fashion. The incorporation of iconic elements like the saree and the infusion of Persian-inspired drapery exemplify the designers' artistry in blending cultural narratives seamlessly.

In an era where the fashion industry is increasingly recognizing and celebrating diversity, Indian designers shine as beacons of creativity and heritage. Their contributions not only elevate the global fashion conversation but also serve as a testament to the enduring allure of India's cultural tapestry, leaving an indelible mark on the world of haute couture. As the global fashion stage continues to evolve, the influence of Indian designers promises to be an integral and ever-expanding chapter in the narrative of global fashion.
