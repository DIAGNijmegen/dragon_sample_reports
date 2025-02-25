# Task 25: Anonymization
Visual (pending translation to English):

![report part 1](/images/dutch/Task025_anonymisation_ner/report-part1.png)
![report part 2](/images/dutch/Task025_anonymisation_ner/report-part2.png)
![report part 2](/images/dutch/Task025_anonymisation_ner/report-part3.png)

Label tokenized (pending translation to English):
```
['O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-<PERSOON>', 'I-<PERSOON>', 'O', 'O', 'O', 'B-<DATUM>', 'I-<DATUM>', 'O', 'O', 'O', 'B-<DATUM>', 'I-<DATUM>', 'I-<DATUM>', 'I-<DATUM>', 'I-<DATUM>', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-<PERSOON>', 'I-<PERSOON>', 'I-<PERSOON>', 'I-<PERSOON>', 'B-<PLAATS>', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-<DATUM>', 'I-<DATUM>', 'I-<DATUM>', 'O', 'O', 'B-<PERSOON>', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-<RAPPORT-ID>', 'I-<RAPPORT-ID>', 'I-<RAPPORT-ID>', 'I-<RAPPORT-ID>', 'O', 'O', 'O', 'O', 'O', 'B-<RAPPORT-ID>', 'I-<RAPPORT-ID>', 'I-<RAPPORT-ID>', 'I-<RAPPORT-ID>', 'O', 'O', 'O', 'B-<DATUM>', 'I-<DATUM>', 'I-<DATUM>', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-<PERSOON>', 'B-<DATUM>', 'I-<DATUM>', 'I-<DATUM>', 'I-<DATUM>', 'I-<DATUM>', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-<PERSOON>', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-<DATUM>', 'I-<DATUM>', 'I-<DATUM>', 'O', 'O', 'B-<PERSOON>', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-<DATUM>', 'I-<DATUM>', 'I-<DATUM>', 'O', 'B-<TIJD>', 'I-<TIJD>', 'I-<TIJD>', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-<ACCREDATIE_NUMMER>', 'I-<ACCREDATIE_NUMMER>', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-<PLAATS>', 'O', 'O', 'O', 'O', 'B-<ACCREDATIE_NUMMER>', 'I-<ACCREDATIE_NUMMER>', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-<ACCREDATIE_NUMMER>', 'I-<ACCREDATIE_NUMMER>', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O']
```

Anonymous sample report (translated from Dutch using ChatGPT 4o with <a href="https://github.com/DIAGNijmegen/LLM_data_extractor/blob/2be30cb35ec58b7e3c9244411624538feecc93ca/data_extractor/prompt_templates/translation/system_prompt.txt" target="_blank">this prompt</a>):
```
##############################
DISCLAIMER: THIS REPORT HAS BEEN ANONYMIZED BY REPLACING PATIENT HEALTH INFORMATION WITH RANDOM SURROGATES.
ANY RESEMBLANCE TO REAL PERSONS, LIVING OR DEAD, IS PURELY COINCIDENTAL.
##############################
Pathologist: Violet Marinus
Date Received: October 2
Date of Report: October 4, 2024
Specimen Type: Brain tissue
Clinical Information: Resection procedure performed. Suspected intracerebral left parafalcine lung metastasis.
Clinical Question: Determination of tissue nature.
Pulmonologist: G. Van Veen (Bethesda)
Biobank Material: No
Submitted Tumor: Yes

Note: This report was generated electronically using a speech recognition system and has been electronically authorized.

Conclusion
Excision of a clinically suspected tumor, intracerebral left parafalcine region: findings consistent with a metastasis from a non-small cell carcinoma. The immunohistochemical staining pattern is indicative of an adenocarcinoma with a primary origin in the lung.

October 4, 2024 – Additional Findings (Lbu):

PD-L1 Immunohistochemistry: Positive (>50%)
ALK Rearrangement: Negative
For DNA mutation analysis: See T24-817623
For fusion gene analysis: See T24-817631
Macroscopy (October 2, 2024)
Specimen Received: Fresh, with a fragment set aside for NEOt before fixation in formalin.
Macroscopic Description: An irregular, elastic biopsy with mixed beige and brown areas, measuring 2.2 cm × 1.9 cm × 1.6 cm. One side of the fragment is encapsulated by a thin membrane, under which a dark blue discoloration is observed. Sectioned into four slices.
Microscopy
Histology:
Brain tissue containing a partially viable tumor composed of confluent clusters of epithelioid cells with predominantly abundant eosinophilic cytoplasm and enlarged, sometimes highly pleomorphic nuclei, some with prominent nucleoli.
In certain areas, there is a suggestion of glandular formation.
Tumor cells exhibit immunohistochemical staining for CK7 and TTF1.
October 4, 2024 – Additional Findings (Lbu):

PD-L1 (22C3 DAKO) Staining: Shows membranous, diffuse staining in approximately 80% of tumor cells.
ALK Rearrangement: Negative.
Additional Findings Communicated: Treating pulmonologist was informed by phone on October 4 at 13:45.
Quality and Accreditation
The Pathology Laboratory is accredited according to ISO 15189 (RvA_TESTEN_M123).
Molecular analyses are partly conducted at Genomic Diagnostics Groningen, also accredited under ISO 15189 (M321).
Molecular microbiological investigations are outsourced to the Medical Microbiology Laboratory, accredited under ISO 15189 (M456).
Any non-accredited tests will be explicitly mentioned.
```

Anonymous sample report  tokenized (pending translation to English):
```
['#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', 'DISCLAIMER', ':', 'THIS', 'REPORT', 'HAS', 'BEEN', 'ANONYMIZED', 'BY', 'REPLACING', 'PATIENT', 'HEALTH', 'INFORMATION', 'WITH', 'RANDOM', 'SURROGATES', '.', 'ANY', 'RESEMBLANCE', 'TO', 'REAL', 'PERSONS', ',', 'LIVING', 'OR', 'DEAD', ',', 'IS', 'PURELY', 'COINCIDENTAL', '.', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', '#', 'SAMENVATTING', ':', 'Patholoog', ':', 'Violet', 'Marinus', 'Datum', 'ontvangst', ':', '2', 'okt', 'Datum', 'antwoord', ':', '4', '/', '10', '/', '2024', 'Aard', 'materiaal', ':', 'hersenen', 'Klinische', 'gegevens', ':', 'Verkrijgingswijze', 'resectie', 'Klinische', 'gegevens', 'verdenking', 'long', 'metastase', 'intracerebraal', 'links', 'parafalcien', 'Vraagstelling', 'aard', 'van', 'het', 'weefsel', '.', 'Longarts', ':', 'G', '.', 'Van', 'Veen', 'Bethesda', 'Materiaal', 'voor', 'biobank', 'Nee', 'Inzending', 'I', 'tumor', 'Ter', 'informatie', ':', 'dit', 'verslag', 'is', 'elektronisch', 'aangemaakt', 'middels', 'een', 'spraakherkenningsysteem', 'en', 'elektronisch', 'geautoriseerd', '.', 'CONCLUSIE', ':', 'excisie', 'klinisch', 'tumor', ',', 'intracerebraal', 'links', 'parafalcien', ':', 'beeld', 'passend', 'bij', 'een', 'metastase', 'van', 'een', 'niet', '-', 'kleincellig', 'carcinoom', ',', 'met', 'immunohistochemisch', 'aankleuringspatroon', 'passend', 'bij', 'adenocarcinoom', 'met', 'primaire', 'origine', 'in', 'de', 'long', '.', '4', 'okt', '2024', 'AANVULLING', '(', 'Lbu', ')', ':', 'PD', '-', 'L', '1', 'immunohistochemisch', 'positief', '(', '>', '50%', ')', '.', 'ALK', 'rearrangement', 'immunohistochemisch', 'negatief', '.', 'Voor', 'DNA', 'mutatieanalysen', ',', 'zie', 'T', '24', '-', '817623', '.', 'Voor', 'fusiegenanalysen', ',', 'zie', 'T', '24', '-', '817631', '.', 'MACROSCOPIE', ':', '2', '10', '2024', 'Jaar', 'I', ':', 'vers', 'ontvangen', ',', 'fragment', 'voor', 'NEOt', 'waarna', 'op', 'formaline', '.', 'Macro', 'volgt', '.', 'Jbo', '3', '/', '10', '/', '2024', 'In', 'formaline', '.', 'I', ':', 'onregelmatig', ',', 'elastisch', ',', 'deels', 'beige', 'deels', 'bruine', 'biopt', 'van', 'maximaal', '2', ',', '2', 'cm', 'x', '1', ',', '9', 'cm', 'x', '1', ',', '6', 'cm', '.', 'Aan', 'een', 'zijde', 'is', 'het', 'fragment', 'afgekapseld', 'met', 'een', 'dun', 'vlies', ',', 'waaronder', 'een', 'donkerblauwe', 'verkleuring', '.', 'In', '4', 'lamellen', '.', 'T', '.', 'i', '.', '3', 'c', '.', 'Hja', 'MICROSCOPIE', ':', 'hersenweefsel', ',', 'met', 'hierin', 'een', 'deels', 'vitale', 'tumor', ',', 'opgebouwd', 'uit', 'in', 'confluerende', 'velden', 'gelegen', 'epithelioide', 'cellen', 'met', 'overwegend', 'ruim', 'eosinofiel', 'cytoplasma', 'en', 'vergrote', 'soms', 'sterk', 'polymorfe', 'kern', ',', 'deels', 'met', 'prominente', 'nucleoli', '.', 'Hierbij', 'op', 'enkele', 'plaatsen', 'suggestie', 'van', 'buisvorming', '.', 'Deze', 'tumorcellen', 'kleuren', 'aan', 'in', 'de', 'CK', '7', 'en', 'TTF', '1', 'kleuring', '.', '04', '.', '10', 'AANVULLING', '(', 'Lbu', ')', ';', 'PD', '-', 'L', '1', '(', '22', 'C', '3', 'DAKO', ')', 'toont', 'immunohistochemisch', 'membraneuze', ',', 'diffuse', 'aankleuring', 'in', 'ca', '80%', 'van', 'de', 'tumorcellen', '.', 'ALK', '-', 'rearrangement', 'immunohistochemisch', 'negatief', '.', 'Aanvullende', 'bevindingen', 'telefonisch', 'medegedeeld', 'aan', 'behandelend', 'logarts', 'op', '04', '.', '10', ',', '13', 'u', '45', '.', 'ISO', ':', 'Het', 'laboratorium', 'voor', 'pathologie', 'is', 'geaccrediteerd', 'volgens', 'ISO', '15189', 'RvA', '_', 'TESTEN', '_', 'M', '123', '.', 'Voor', 'de', 'moleculaire', 'analyses', 'wordt', 'deels', 'gebruik', 'gemaakt', 'van', 'faciliteiten', 'van', 'Genoomdiagnostiek', 'Groningen', 'onder', 'ISO', '15189', 'accreditatie', 'M', '321', '.', 'Moleculair', 'microbiologisch', 'onderzoek', 'wordt', 'uitbesteed', 'aan', 'Laboratorium', 'Medische', 'Microbiologie', 'onder', 'ISO', '15189', 'accreditatie', 'M', '456', '.', 'Bij', 'niet', 'geaccrediteerde', 'testen', 'wordt', 'dit', 'expliciet', 'vermeld', '.']
```