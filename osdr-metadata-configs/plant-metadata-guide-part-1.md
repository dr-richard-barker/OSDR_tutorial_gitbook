# Plant metadata guide part 1

**Age at launch** **(with unit column)** in whichever unit of time provided by submitter - \*Only include this characteristic if seeds germinated before launch. Most spaceflight studies maintain seed dormancy until after launch (in which case this column is not needed)

**Age at sample harvest (with unit column)** **(free text)**

**Characteristics**

**Container**: This is for cases where a smaller container is used within a larger hardware

For algae- This is the type of culture bag used (ex PermaLife tissue culture bag) Richard says these are important and at least one study (GLDS-265) has the bag inside the VEGGIE hardware so I needed to create a new column for the growth container inside the hardware

**Culture Media** (same as growth medium but for algae). This parameter name has an ontology. In some alga studies there is a culture medium and a distinct growth medium. If both are described enter both columns.

**Development stage - work in progress**

Older datasets only have 1 column (developmental stage) which indicates the developmental stage at time of sample collection. During normalization I will change the name to Developmental stage at time of sample collection and add a second column for Developmental stage at onset of treatment. IF the following conditions are met:

1. Before using the TAIR guidelines ([https://www.arabidopsis.org/portals/education/growth.jsp](https://www.arabidopsis.org/portals/education/growth.jsp)) to calculate developmental stage for _Arabidopsis thaliana_ Col-0 or any strain derived from Col-0 baseline you need to double check the documented phenotype of the strain/genotype of _A. thaliana_ used in the study. Even if the strain is not specifically created to have a different developmental timeline than the baseline (ex. starchless mutant) you need to check TAIR (ex. See phenotype field [https://www.arabidopsis.org/servlets/TairObject?type=germplasm\&id=1005161198](https://www.arabidopsis.org/servlets/TairObject?type=germplasm\&id=1005161198)) or the primary literature to make sure it does not have accelerated or delayed development from "hitch hiker selection". If that is not possible do not include developmental stage columns.
2. Check the study light cycle before proceeding. TAIR uses 16:8 light:dark to make predictions about developmental stage based on age. If the growth light cycle is 24 hours of light you cannot make a guess about developmental stage without checking with the PI. Similarly, developmental stage transitions in Arabidopsis are promoted by blue light and delayed by red light. For studies that use anything other than "white" or "red and blue" light during the growth stage we need to confirm the developmental stages with the PI. If that is not possible do not include developmental stage columns.
3. No developmental stage column needed for algae studies unless the dataset specifies one. Microalgae growth is most commonly described in "phases" (lag phase, exponential phase, declining relative growth phase, stationary phase, and death phase) rather than developmental stages. I don't see this as a parameter in other repos with algae datasets but I can ask the plant AWG about it.
4. If there are multiple treatments with different durations modify this parameter name to be more descriptive and have one per treatment (ex. GLDS-314 has two parameters for onset 'Developmental stage at onset of light treatment' and 'Developmental stage at onset of gravity treatment')\


**New datasets (or any dataset being revised) should have two columns (if possible):**

1. Developmental stage at onset of treatment

2\. Developmental stage at time of sample collection

\


**Angiosperms**

**Developmental Stages using a compilation of existing ontology classes:**

1. If seeds are kept in the cold/dark to prevent germination use this developmental stage '**plant embryo dormant stage**' ([http://purl.obolibrary.org/obo/PO\_0025377](http://purl.obolibrary.org/obo/PO\_0025377)). This will be a common input for "Developmental stage at onset of treatment" since most petri-dish based studies used cold stratified seeds
2. For plants that have germinated but have no adult leaves yet use: 'seedling development stage' ([http://purl.obolibrary.org/obo/PO\_0007131](http://purl.obolibrary.org/obo/PO\_0007131), A sporophyte vegetative stage (PO:0007134) that succeeds the seed germination stage (PO:0007057) and terminates with the development of the first adult vascular leaf (PO:0006340).) or any of its subclasses\
   \
   Many studies do not go beyond this stage. Only after 10 days (with LIGHT) do Arabidopsis seedlings have at least 1 set of fully formed true leaves.\
   \

3. Use one of the '**leaf production stage**' subclasses by navigating to this link and expanding the options by clicking the + button next to '**leaf production stage**' [https://bioportal.bioontology.org/ontologies/PO?p=classes\&conceptid=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FPO\_0007133](https://bioportal.bioontology.org/ontologies/PO?p=classes\&conceptid=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FPO\_0007133)
   1. Also add a "Number of leaves at onset of treatment" column and a "Number of leaves at time of sample collection" and allow for any inputs. In the future I think this could be a good use of the drop down feature. We could use this prompt and have a drop down of categories to populate it: How many leaves are present? Less than 3; 3 to 10; 11 to 100; 101 to 1,000; 1,001 to 10,000; More than 10,000;
   2. If the number of leaves is not noted and you are not confident making an estimate based on the literature just use the '**leaf production stage**' class itself (rather than a subclass)
4. If the leaf arrangement is a basal rosette (ex. Arabidopsis) do not use the '**rosette growth stage**' classes. They are less informative than the leaf production stage classes. IF you have reason to use this family for Arabidopsis, see this link [https://www.arabidopsis.org/portals/education/growth.jsp](https://www.arabidopsis.org/portals/education/growth.jsp) to determine what percentage of total rosette leaves are present based on number of leaves and days since germination
   1. Add a "Number of leaves at onset of treatment" and a "Number of leaves at time of sample collection" column and allow for any inputs. In the future I think this could be a good use of the drop down feature. We could use this prompt and have a drop down of categories to populate it: How many leaves are present? Less than 3; 3 to 10; 11 to 100; 101 to 1,000; 1,001 to 10,000; More than 10,000;\

   2. If the number of leaves is not noted and you are not confident making an estimate based on the literature just use the '**rosette growth stage**' class itself (rather than a subclass)
5. If there are unopened flower buds on the plant use '**bud development stage**' ([http://purl.obolibrary.org/obo/PO\_0025528](http://purl.obolibrary.org/obo/PO\_0025528)) Add a "Number of buds at onset of treatment" and a "Number of buds at time of sample collection" column and allow for any inputs. How many flower buds are present? Same recommendation for drop down menu.\

6. If the number of open flowers is noted use one of the '**whole plant flowering stage**' classes by navigating to this link and expanding the options by clicking the + button next to 'whole plant flowering stage' ([https://bioportal.bioontology.org/ontologies/PO/?p=classes\&conceptid=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FPO\_0007016](https://bioportal.bioontology.org/ontologies/PO/?p=classes\&conceptid=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FPO\_0007016)) Add a "Number of open flowers at onset of treatment" column and a "Number of open flowers at time of sample collection". How many flowers are present? For species in which individual flowers are clustered in flower heads, spikes or catkins (inflorescences), skip to 7. Same recommendation for drop down menu.\

7. If the number of open flowers is NOT noted but the publication/data description indicates the plant is flowering enter the '**whole plant flowering stage**' class itself (not any of the subclasses). Add a "Number of open flowers at onset of treatment" column and a "Number of open flowers at time of sample collection". Write "Not Available".\

8. If the study species produces groups of flowers (inflorescences) rather than single flowers, use the classes within '**whole plant inflorescence detectable stage**' ([https://bioportal.bioontology.org/ontologies/PO/?p=classes\&conceptid=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FPO\_0007047](https://bioportal.bioontology.org/ontologies/PO/?p=classes\&conceptid=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FPO\_0007047)).\
   Add a "Number of open inflorescences" column. How many inflorescences are present? For these species, in which individual flowers are clustered in flower heads,\
   spikes or catkins (inflorescences), simply estimate the number of flower heads, spikes or catkins and not the number\
   of individual flowers. Same recommendation for drop down menu.
9.  If fruits are present on the plant use the classes within '**whole plant fruit development stage**' ([https://bioportal.bioontology.org/ontologies/PO/?p=classes\&conceptid=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FPO\_0025500](https://bioportal.bioontology.org/ontologies/PO/?p=classes\&conceptid=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FPO\_0025500)).

    Add a "Number of fruits" column. How many fruits are present? Same recommendation for drop down menu.\

10. If the plant is senescent (in an annual plant this will occur not long after the last fruit has ripened and fallen off/been removed from the plant) use '**sporophyte senescent stage**' ([http://purl.obolibrary.org/obo/PO\_0007017](http://purl.obolibrary.org/obo/PO\_0007017))
11. Developmental stage ontologies for specific groups of plants: Cereal Plant Development Ontology: [https://bioportal.bioontology.org/ontologies/GRO-CPD?p=classes\&conceptid=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FGRO\_0007002](https://bioportal.bioontology.org/ontologies/GRO-CPD?p=classes\&conceptid=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FGRO\_0007002)

**Developmental stage at time of sample collection** (see definitions above) **(free text)**

**duration** (with unit column)( _Exposure Duration_ is to be reserved for radiation metadata) This parameter name has an ontology. \*duration should only be added if there is a treatment time that is distinct from growth time. For example if seedlings were exposed to a unique light treatment for 12 hours but the total growth time was 3 days, then it would be informative to have both Duration and Growth Time columns.

**Genotype, variety, ecotype etc.-**&#x20;

We describe the additional organism modifiers (variety, ecotype, strain, cultivar) any way the PI or data submitter wants us to. If the data is already in NCBI/GEO this preference will be noted on the sample page and if not it will be described in the associated publication. For example, if they want to call Arabidopsis thaliana "Wasselewskija" an ecotype they can, or if they want to call it a strain or a variety they can etc. Our protocol could just be to accept whatever language the data submitter uses. And if the data submitter does not provide a categorization we can refer to the definitions listed for each category in the ontology (posted below) and make a decision.

**Growth environment** **(has ontology)** (e.g. space shuttle, ISS-US Lab, Earth surface, shuttle simulator or ISSES] ) If the study was conducted on Earth but not in an environmental or shuttle simulator use "Earth surface". Most of these parameter names are linked to an ontology. If curating a radiation study this may be a duplicate column with 'vehicle' which is fine.

International Space Station (RBO) (if module unknown)

ISS-US Laboratory

ISS-Colombus

International Space Station Environmental Simulator (ISSES) (free text)

Earth's surface (has ontology) \*use for ground samples where ISSES or other simulator was not specified

**growth medium** (substrate, soil mixture description etc.) This parameter name has an ontology. \*Watch out for special characters here if copying and pasting from publication. If there are any non alphanumeric characters just delete them and retype them. "MS Media" or "MS" means Murashige and Skoog medium. It is common enough some paper's don't even write out the full name but we should.

**Growth Time** (with unit column) Some authors want to include the cold stratification period as part of the growth time but I strongly disagree with that. Arabidopsis thaliana seeds specifically cannot germinate at 4C/dark and I think we need to consider the onset of growth as the time of germination. If they try to include the cold stratification period in the growth time create two columns 'stratification exposure' and 'growth time'

**Hardware** (e.g. VEGGIE, BRIC, SIMBOX, ABRS)(free text)

**Possible values:**

Enter **Vegetable Production System (Veggie)** (exactly as written) if the hardware is listed as VEGGIE, Vegetable Production System (Veggie) or Vegetable Production System (VPS)

Enter **BRIC-PDFU (Petri Dish Fixation Unit)** (exactly as written) if the hardware is BRIC-PFU

Enter **European Modular Cultivation System (EMCS)** (exactly as written)

Enter **Kennedy Fixation Tube (KFT)** (exactly as written)

There are several different subcategories of BRIC hardware with notable differences ([https://www.nasa.gov/mission\_pages/station/research/experiments/explorer/Investigation.html?#id=697](https://www.nasa.gov/mission\_pages/station/research/experiments/explorer/Investigation.html#id=697)).\


For algae this is sometimes just a plastic tub.

**Light Color** (eg. red and blue)**(free text)** qualitative description of light quality \*\*See note above about light parameters as factors

**Light Cycle** (e.g. Light/Dark 24/0 or 12/12) (with unit column)**(has ontology)** refers to the amount of light vs. dark plants are exposed to in a 24hr period. This parameter name has an ontology. This looks different across studies but there is not a great way to homogenize it without it being excessively tedious for the data submitter. BUT if the growth hardware is a traditional BRIC-PDFU (not a BRIC-LED) then light cycle should be "dark 24" and the units column should be "hours". BRIC-PDFUs allow no light in. \*\*If the study uses light cycle as a treatment/factor such that the light cycle of the growth period is different from the light cycle of the treatment you should create two columns for light cycle: 'Growth Light Cycle' (with units column, under growth protocol) and 'Treatment Light Cycle' (with units column, under treatment protocol). If light cycle is part of the treatment remember to add 'light cycle' as a study design descriptor.

**Light Intensity** (e.g. 200umol-2) (with unit column) **(free text)** The units for this column are routinely a mess. The cells do not allow supescripts or special characters so this: µmol m-2 s-1 gets turned into some version of this umol m-2 s-1. There is currently no ontology class for it so I have asked UO to create one [here](https://github.com/bio-ontology-research-group/unit-ontology/issues/58).  Just write it out (micromole per square meter per second). PAR is photosynthetically active radiation (400-700 nm) and PPFD is photosynthetic photon flux density (µmol/m2/s). Common mistake in literature: "plants were grown at 200 µmol/m2/s of PAR". PAR is not a unit.&#x20;

\*\*If the study uses light intensity as a treatment/factor such that the light intensity of the growth period is different from the light intensity of the treatment you should create two columns for light intensity: 'Growth Light Intensity' (with units column, under growth protocol) and 'Treatment Light Intensity' (with units column, under treatment protocol). If light intensity is part of the treatment remember to add 'light intensity' as a study design descriptor.

**Light Quality** (e.g. X-Xnm) **(free text)** (with unit column) nm (nanometer) has an ontology \*\*See note above about light parameters as factors

**light regimen** **(has ontology)** Add this column if the study has a continuous light regimen or continuous dark regimen. Both terms have ontologies but you have to scroll down a bit to find them

**light source** (ex. light-emitting diode). **(has ontology)**This parameter name has an ontology. Don't use BAO ontology until were sure it works (currently links are broken)

aximum Temperature (Celsius): 24.195

Mean % Relative humidity: 34.920

**Mean Growth Temperature** (with unit column) -

Most studies provide a range of temperatures or a sd. Then we have "-" or "+/-" in the column rather than a single number. Which makes the sample table a mess for processing and make it not "AI ready". So only report the mean growth temp in the sample table. This is definitely reductionist since a wide range of temperatures could definitely influence the interpretation of the data but we already have so many parameters I am hesitant to report Max and Mean temp in the table also.&#x20;

**Mean Light Intensity,** Lux (lux is the unit measuring light intensity equal to one lumen per square meter): 610.673

**Mission- and Hardware-specific growth environment info** (retrieved from data loggers inside hardware)

**Number of seeds per container (free text)**. This should not be considered critical or minimal/required metadata but it will really help users interpret the data and should be relatively easy information for the PI's to provide

Options for taxonomy if not provided by submitter, these are all currently linked to an ontology.\
**Strain** (default)

EFO Definition: "A population of organisms that is geneticaly different from others of the same species and possessing a set of defined characteristics."EFO Definition: "A population of organisms that is genetically different from others of the same species and possessing a set of defined characteristics."

**Ecotype** (linked as synonym to strain in search)- EFO Definition: "A biotype resulting from selection in a particular habitat, e.g. the A. thaliana Ecotype Ler" \* Unfortunately I can also show you publications that refer to _A. thaliana_ Landsberg _erecta_ (L_er_) as a genotype and as a strain.

**Cultivar** (linked as synonym to strain in search)- EFO Definition: "A cultivated plant variety selected and given a name because it has desirable characteristics that distinguish it from otherwise similar plants of the same species."

**Variety** (linked as synonym to strain in search)- NCIT Definition (EFO has not entry for variety): "In botanical nomenclature, a rank below subspecies but above forma."

Accession (linked as synonym to strain in search)- EDAM Definition: A persistent (stable) and unique identifier, typically identifying an object (entry) from a database.

**Genotype** (linked as synonym to strain in search)- EFO Definition: "Information, making the distinction between the actual physical material (e.g. a cell) and the information about the genetic content (genotype). The total sum of the genetic information of an organism that is known and relevant to the experiment being performed, including chromosomal, plasmid, viral or other genetic material which has been introduced into the organism either prior to or during the experiment."

NCIT Definition: "The genetic constitution of an organism or cell, as distinct from it's expressed features or phenotype."

**Organism** (genus and specific epithet) This parameter name has an ontology. All scientific names should be present in NCBI Taxon as well.&#x20;

**Organism Part** (has ontology). **USE THIS TERM FOR TISSUE/MATERIAL TYPE**.  If you are ingesting data and the PI uses really unique parts like: "1mm root tip", "3mm root tip" or something just write exactly what they do. We don't need to shoehorn all values into those with ontologies at the risk of losing specificity. Use the "leaf" ontology if it was just one leaf and use "plant leaves" if it was multiple. . If the dataset says cotyledons (or "seed leaves" were collected please write cotyledon instead of leaf. This parameter name has an ontology.

**PARAMETERS FOR GROWTH PROTOCOL**

**Sample collection protocol**

**Quantity of growth medium** (with units column) - usually measured in mL. Only include if you are sure and if it is already reported publicly (not worth emailing the PI for). Careful with this column for algae. The quantity often changes multiple times. If this is the case skip this column

PARAMETERS FOR SAMPLE COLLECTION PROTOCOL

**Sample name**

**Sample Preservation Method** (ex. RNAlater) **(free text).** All common inputs has ontologies even if column name does not.&#x20;

**Sample Storage Temperature** (with unit column) **(free text)**

**Source Name**

**Seed Source (analogous to Animal Source)** - ex. Arabidopsis Biological Resource Center #C3210. If the seeds are the result of breeding studies within a lab list the PI here (ex. "internal lab stock maintained by Dr. Jane Smith, University of Vermont")

**soil environment exposure** ([http://purl.obolibrary.org/obo/PECO\_0007049](http://purl.obolibrary.org/obo/PECO\_0007049))    An exposure involving growing plants in soil growth media with varying contents. Use as factor for lunar or martian regolith studies.&#x20;

**stratification exposure (with unit column)**     \
A physical exposure (PECO:0007316) involving both low temperature and moist conditions to overcome seed dormancy. A stratification process is used to pretreat seeds to simulate natural winter conditions in order to overcome dormancy and allow germination. If a paper says the seeds were (for example) kept at 4C for 3 days before exposure to light but do not mention the moisture conditions it is safe to assume they are still talking about stratification exposure.

\*Asked PECO ontology maintainers for a more general definition for their 'stratification exposure' class or  a more specific subclass of 'physical plant exposure' (such as 'dormant seed exposure'?) that includes conditions to overcome seed dormancy other than cold and wet conditions. [https://github.com/Planteome/plant-experimental-conditions-ontology/issues/132](https://github.com/Planteome/plant-experimental-conditions-ontology/issues/132)

**Stratification exposure -**   \
A physical exposure (PECO:0007316) involving both low temperature and moist conditions to overcome seed dormancy. A stratification process is used to pretreat seeds to simulate natural winter conditions in order to overcome dormancy and allow germination. Arabidopsis thaliana cannot germinate at 4C ( I don't know of a plant that can) so any amount of time the seeds are at 4C should not be considered a part of the growth time. If the description says the seeds were kept at 4C but does not specify the moisture conditions (that would be unusual but possible) we can ask. But if they are plated on agar or phytagel or something that is moist we don't have to ask. If you add stratification exposure to a dataset but had to dig a little to find the information add a sentence to the growth protocol that says: "Stratification exposure (A physical exposure involving both low temperature and moist conditions to overcome seed dormancy) was calculated by GeneLab based on how long seeds were in 4C, moist conditions before the onset of growth conditions."&#x20;



**VEGGIE - APEX03 GROUND CONTROL 01/10/2015-02/11/2015**

**VEGGIE - APEX03 SPACEFLIGHT 01/10/2015-02/11/2015**

**VEGGIE - APEX04 GROUND CONTROL**

**VEGGIE - APEX04 SPACEFLIGHT**

**watering schedule (free text)** Provide a brief free text description of how the plants received water. Ex. 'bottom watered for the duration of the growth time'. This is rarely used since most studies in our repo are agar-plated



Options for taxonomy if not provided by submitter

These are all currently linked to an ontology.\


**Strain (default) EFO Definition:** "A population of organisms that is geneticaly different from others of the same species and possessing a set of defined characteristics."EFO Definition: "A population of organisms that is genetically different from others of the same species and possessing a set of defined characteristics."

**Ecotype (linked as synonym to strain in search)- EFO Definition:** "A biotype resulting from selection in a particular habitat, e.g. th_e A. thaliana_ Ecotype Ler" \* Unfortunately I can also show you publications that refer to _A. thaliana_ Landsberg _erecta_ (L_er_) as a genotype and as a strain.

**Cultivar (linked as synonym to strain in search)- EFO Definition:** "A cultivated plant variety selected and given a name because it has desirable characteristics that distinguish it from otherwise similar plants of the same species."

**Variety (linked as synonym to strain in search)- NCIT Definition (EFO has not entry for variety):** "In botanical nomenclature, a rank below subspecies but above forma."

**Accession (linked as synonym to strain in search)- EDAM Definition:** A persistent (stable) and unique identifier, typically identifying an object (entry) from a database.

**Genotype (linked as synonym to strain in search)- EFO Definition:** "Information, making the distinction between the actual physical material (e.g. a cell) and the information about the genetic content (genotype). The total sum of the genetic information of an organism that is known and relevant to the experiment being performed, including chromosomal, plasmid, viral or other genetic material which has been introduced into the organism either prior to or during the experiment."

**NCIT Definition:** "The genetic constitution of an organism or cell, as distinct from it's expressed features or phenotype."



**Number of seeds per container (free text)**. This should not be considered critical or minimal/required metadata but it will really help users interpret the data and should be relatively easy information for the PI's to provide.

**light source** (ex. light-emitting diode). **(has ontology)**This parameter name has an ontology. Don't use BAO ontology until were sure it works (currently links are broken)

**light regimen** **(has ontology)** Add this column if the study has a continuous light regimen or continuous dark regimen. Both terms have ontologies but you have to scroll down a bit to find them

**Light Quality** (e.g. X-Xnm) **(free text)** (with unit column) nm (nanometer) has an ontology \*\*See note above about light parameters as factors

**Light Intensity** (e.g. 200umol-2) (with unit column) **(free text)** The units for this column are routinely a mess. The cells do not allow supescripts or special characters so this: µmol m-2 s-1 gets turned into some version of this umol m-2 s-1. There is currently no ontology class for it so I have asked UO to create one [here](https://github.com/bio-ontology-research-group/unit-ontology/issues/58).  Just write it out (micromole per square meter per second). PAR is photosynthetically active radiation (400-700 nm) and PPFD is photosynthetic photon flux density (µmol/m2/s). Common mistake in literature: "plants were grown at 200 µmol/m2/s of PAR". PAR is not a unit.&#x20;

\*\*If the study uses light intensity as a treatment/factor such that the light intensity of the growth period is different from the light intensity of the treatment you should create two columns for light intensity: 'Growth Light Intensity' (with units column, under growth protocol) and 'Treatment Light Intensity' (with units column, under treatment protocol). If light intensity is part of the treatment remember to add 'light intensity' as a study design descriptor.

**Light Cycle** (e.g. Light/Dark 24/0 or 12/12) (with unit column)**(has ontology)** refers to the amount of light vs. dark plants are exposed to in a 24hr period. This parameter name has an ontology. This looks different across studies but there is not a great way to homogenize it without it being excessively tedious for the data submitter. BUT if the growth hardware is a traditional BRIC-PDFU (not a BRIC-LED) then light cycle should be "dark 24" and the units column should be "hours". BRIC-PDFUs allow no light in. \*\*If the study uses light cycle as a treatment/factor such that the light cycle of the growth period is different from the light cycle of the treatment you should create two columns for light cycle: 'Growth Light Cycle' (with units column, under growth protocol) and 'Treatment Light Cycle' (with units column, under treatment protocol). If light cycle is part of the treatment remember to add 'light cycle' as a study design descriptor.

