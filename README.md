<h2 align="center">
  19th c. Greek Corpora for NER and RE
</h2>


> In this repo, we present our Benchmark Dataset for NER and RE in 19th c. Greek corpora, which was developed for our paper:<br />
[Extracting Semantic Relationships in Greek Literary Texts]()<br />
Despina Christou and Grigorios Tsoumakas


This is the first publicly available dataset for this period in Greek and includes 3,649 samples annotated through distant supervision with six semantic relationships. Taking into account that the greatest part of digitized Modern Greek literature refers to the 19th century, we construct our dataset by aligning relation-triples from [1] to twenty-six (26) literary Greek books of the 19th century. Namely, we use the provided relation triplets (i.e., head-tail-relationship triplets) as an external knowledge base (KB) to automatically extract sentences that include the entity pairs, assuming that these sentences will also express the same relationship (distant supervision).

We make this dataset publicly available to encourage further research on 19th-century Greek literary fiction.


### Dataset
The benchmark data can be found [here](https://drive.google.com/drive/folders/1GU_PgKTiiVL7iJgiKKkjrZiiePIvZGHX?usp=sharing). Train, validation and test datasets follow a 80%-10%-10% split with all sets including the following features:

- "text": Text Instance (can include up to three consequent sentences)
- "relation": The underlying relation. (Values:"NoRel", "artAuthor", "artHero", "orgDate", "orgPlace", "pubDate", "workAt") 
- "person": Person named entity found in "text"
- "place": Place named entity found in "text"
- "org": Organization named entity found in "text"
- "date": Date named entity found in "text"
- "title": Title named entity found in "text"
- "trim_text_1": Compact form of "text". It preserves the text starting from the three preceding words of the head entity to the three following words of the tail entity.
- "trim_text_2": Compact form of "text". It preserves only the surrounding text of the head and tail entities, with surrounding text referring to the three preceding and following words of each entity.
- "h_word": Head word participating in the relation
- "h_ne": "h_word"'s named entity type
- "t_word": Tail word participating in the relation
- "t_ne": "t_word"'s named entity type


### Funding
This work was co‐financed by the European Regional Development Fund of the European Union and Greek national funds through the Operational Program Competitiveness, Entrepreneurship and Innovation, under the call RESEARCH – CREATE - INNOVATE (project code:T1EDK-05580) in the context of the ECARLE (Exploitation of Cultural Assets with computer-assisted Recognition, Labeling and meta-data Enrichment) project.


### References:
[1] Koidaki, F.; Tiktopoulou, K. Encoding semantic relationships in literary texts. A methodological proposal for linking networkedentities into semantic relations.  Ballisage: Markup Conference, 2021, pp. 28–37.

## Citations
If you use our dataset in your research or find our repository useful, please consider citing our work.

```TBA```

