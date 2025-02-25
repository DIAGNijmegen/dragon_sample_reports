# Task 27: Prostate biopsy sampling
Visual (pending translation to English):

![report](/images/dutch/Task027_prostate_biopsy_ner/report.png)

Label tokenized (pending translation to English): 
```
[ ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["B-1-locatie naald"], ["I-1-locatie naald"], ["I-1-locatie naald"], ["I-1-locatie naald"], ["I-1-locatie naald"], ["O"], ["B-1-ambigu"], ["I-1-ambigu"], ["I-1-ambigu"], ["O"], ["O"], ["O"], ["O"], ["B-2-locatie naald"], ["I-2-locatie naald"], ["I-2-locatie naald"], ["I-2-locatie naald"], ["I-2-locatie naald"], ["O"], ["B-2-ambigu"], ["I-2-ambigu"], ["I-2-ambigu"], ["O"], ["O"], ["O"], ["O"], ["B-3-locatie naald"], ["I-3-locatie naald"], ["I-3-locatie naald"], ["I-3-locatie naald"], ["I-3-locatie naald"], ["I-3-locatie naald"], ["O"], ["B-3-representatief"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O" ] ]
```

Anonymous sample report (translated from Dutch using ChatGPT 4o with <a href="https://github.com/DIAGNijmegen/LLM_data_extractor/blob/2be30cb35ec58b7e3c9244411624538feecc93ca/data_extractor/prompt_templates/translation/system_prompt.txt" target="_blank">this prompt</a>):
```
##############################
DISCLAIMER: THIS REPORT HAS BEEN ANONYMIZED BY REPLACING PATIENT HEALTH INFORMATION WITH RANDOM SURROGATES.
ANY RESEMBLANCE TO REAL PERSONS, LIVING OR DEAD, IS PURELY COINCIDENTAL.
##############################
According to protocol, MRI-guided biopsies were taken from the edge of the ablation zone one year after MRI-guided cryoablation of the right seminal vesicle.

Needle 1: Medial edge of the ablation zone, right seminal vesicle: Possibly too shallow.
Needle 2: Lateral edge of the ablation zone, right seminal vesicle: Possibly too shallow.
Needle 3: Apex of the prostate/transition to medial seminal vesicles: Representative.
The histological results will be sent separately.
```

Anonymous sample report tokenized (pending translation to English):
```
["#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "DISCLAIMER", ":", "THIS", "REPORT", "HAS", "BEEN", "ANONYMIZED", "BY", "REPLACING", "PATIENT", "HEALTH", "INFORMATION", "WITH", "RANDOM", "SURROGATES", ".", "ANY", "RESEMBLANCE", "TO", "REAL", "PERSONS", ",", "LIVING", "OR", "DEAD", ",", "IS", "PURELY", "COINCIDENTAL", ".", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "Conform", "protocol", "werden", "er", "1", "jaar", "na", "MRI", "-", "geleide", "cryoablatie", "van", "het", "rechter", "vesiculum", "MRI", "-", "geleidebiopten", "genomen", "uit", "de", "rand", "van", "de", "ablatie", "zone", ".", "Naald", "1", ":", "Mediale", "rand", "ablatiezone", "zaadblaasje", "rechts", ":", "Mogelijk", "te", "ondiep", ".", "Naald", "2", ":", "Laterale", "rand", "ablatiezone", "zaadblaasje", "rechts", ":", "Mogelijk", "te", "ondiep", ".", "Naald", "3", ":", "Apex", "prostaat", "\/", "overgang", "zaadblaasjes", "mediaal", ":", "Representatief", ".", "De", "histologische", "uitslag", "wordt", "separaat", "verzonden", "."]
```
