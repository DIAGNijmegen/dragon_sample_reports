# Task 28: Skin histopathology diagnosis
Visual:

![report](images/Task028_skin_pathology_ner/report.png)

Label tokenized: 
```
[ ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["B-1-biopt"], ["O"], ["O"], ["O"], ["B-1-BCC"], ["O"], ["B-1-nodular"], ["O"], ["B-1-infiltrative"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"], ["O"] ]
```

Anonymous sample report (translated from Dutch using ChatGPT 4o with <a href="https://github.com/DIAGNijmegen/LLM_data_extractor/blob/2be30cb35ec58b7e3c9244411624538feecc93ca/data_extractor/prompt_templates/translation/system_prompt.txt" target="_blank">this prompt</a>):
```
##############################
DISCLAIMER: THIS REPORT HAS BEEN ANONYMIZED BY REPLACING PATIENT HEALTH INFORMATION WITH RANDOM SURROGATES.
ANY RESEMBLANCE TO REAL PERSONS, LIVING OR DEAD, IS PURELY COINCIDENTAL.
##############################
MACROSCOPY:
07-03, in formalin.
I: Skin punch biopsy with a diameter of 0.5 cm and a depth of 0.2 cm. The skin surface appears smooth, with a white-gray aspect. Unsectioned. T.I. 1b. RGer

MICROSCOPY:
Skin biopsy extending into the subcutaneous fat tissue, containing a basal cell carcinoma with a nodular and infiltrative growth pattern. The tumor extends to approximately halfway through the dermis.

CONCLUSION:
Skin biopsy from the left jawline: Basal cell carcinoma, nodular and infiltrative type, extending to the mid-dermis.

HISTOLOGY REMARKS / REQUESTED EXAMINATION:
Basal cell carcinoma? Morbus Bowen? Actinic keratosis?

UMCA IP PATHOLOGY CLINICAL INFORMATION:
On the jawline, near the left corner of the mouth, there is an approximately 5 mm erythematosquamous plaque with several centrally located, slightly shiny papules. Dermoscopic examination reveals telangiectasias.

UMCA IP PATHOLOGY METHOD OF SAMPLE COLLECTION:
Biopsy.

UMCA IP HISTOLOGY SPECIMEN JAR I:
3 mm HE-stained biopsy from the lesion.
```

Anonymous sample report tokenized:
```
["#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "DISCLAIMER", ":", "THIS", "REPORT", "HAS", "BEEN", "ANONYMIZED", "BY", "REPLACING", "PATIENT", "HEALTH", "INFORMATION", "WITH", "RANDOM", "SURROGATES", ".", "ANY", "RESEMBLANCE", "TO", "REAL", "PERSONS", ",", "LIVING", "OR", "DEAD", ",", "IS", "PURELY", "COINCIDENTAL", ".", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "#", "MACROSCOPIE", ":", "07", "-", "03", "Op", "formaline", ".", "I", ":", "huidstans", "met", "een", "doorsnede", "van", "0", ",", "5", "cm", "en", "1", "diepte", "van", "0", ",", "2", "cm", ".", "Huidoppervlak", "glad", "witgrijze", "aspect", ".", "Onaangesneden", "t", ".", "i", ".", "1", "b", ".", "RGer", "MICROSCOPIE", ":", "Huidbiopt", "tot", "in", "vetweefsel", "met", "hierin", "een", "basaalcelcarcinoom", "met", "nodulaire", "en", "sprieterige", "groeiwijze", ".", "Deze", "reikt", "tot", "ca", ".", "halverwege", "de", "dermis", ".", "CONCLUSIE", ":", "Huidbiopt", "kaakrand", "links", ":", "basaalcelcarcinoom", ",", "nodulaire", "en", "sprieterige", "type", ",", "reikend", "tot", "halverwege", "de", "dermis", ".", "HISTOLOGIE", "OPMERKING", "\/", "GEWENST", "ONDERZOEK", ":", "basaalcelcarcinoom", "?", "M", "Bowen", "?", "Actinische", "keratose", "?", "UMCA", "IP", "PATH", "KLIN", "GEGEVENS", ":", "op", "kaakrand", ",", "thv", "linker", "mondhoek", "een", "circa", "5", "mm", "grote", "erythematosquameuze", "plaque", "met", "centraal", "enkele", "wat", "glanzende", "papels", "met", "bij", "dermatoscopisch", "onderzoek", "teleangiectasieen", ".", "UMCA", "IP", "PATHO", "VERKRIJGINGSWIJZE", "HISTO", ":", "biopt", "UMCA", "IP", "HISTOLOGIE", "POTJE", "I", ":", "3", "mm", "HE", "biopt", "uit", "afiwjking"]
```