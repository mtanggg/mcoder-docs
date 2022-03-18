---
description: mCODER Fields Terminology
---

# ⚙ Data Dictionary

## <mark style="color:blue;">**Patient**</mark>

### General Information

* **Patient identifier**: A unique identifier for the patient. The format of the identifier starts off with an acronym for the study\
  e.g., The study _Neurofibromatosis type 1_ would be NF-##-##
* **Study**: What is the study the patient is recruited/undergoing for
* **Date of birth**: The date of birth of the patient with only the year and month
* **Gender**: The gender of the patient
* **Race**: The racial category of the patient
* **Recruitment location: City or Postal/Zip code**_:_ The city or postal code of the location where the patient was recruited for the study
* **Institution**: The hospital/centre/clinic site where the patient was recruited for the study
* **Family ID**_**:**_ The family identifier the patient may be affiliated with

### Comorbid Condition

* **Date of evaluation**: The date the patient was evaluated with the comorbid condition
* **Comorbid condition code**_**:**_ The disease or medical condition the patient has
* **Condition clinical status**: The status as of the last update of the condition
* **Comments**: Any comments about the patient’s comorbid condition

### General Clinical Evaluation

* **Date of evaluation**: The date the patient was overall assessed
* **ECOG performance status**: Eastern Cooperative Oncology Group (ECOG) Performance Status score of the patient’s ability to function and endure therapies
* **Karnofsky performance status**: Scores measuring a patient’s ability to execute everyday tasks. The higher the Karnofsky performance status (KPS) score, the better the patient is able to complete everyday tasks.
* **Comments**: Any comments about the patient’s clinical evaluation

## <mark style="color:blue;">**Disease**</mark>

### Tumor Data

* **Date of diagnosis**: The date that first confirmed the diagnosis of the disease
* **Tumor type**: What kind of tumor is it
* **Tumor histology**: What method has the tumor been excised by, either biopsy or surgical resection, or unknown
* **Clinical status**: The status as of the last update of the condition
* **Body location code**: **** The location of the disease on the body
* **Body location side**: On which side of the body is the tumor located on
* **Oncotree code**: An Oncotree code is a unique cancer type diagnosis code. Each cancer type diagnosis name has its own OncoTree code, an abbreviation of the full cancer type name. The OncoTree code is used to standardize cancer type diagnosis; it is developed by Memorial Sloan Kettering Cancer Center (MSK).\
  For example, the OncoTree code for the cancer “Stomach Adenocarcinoma” is “STAD”.
* **Clinical stage group**: The category describing the level of the disease, following the TNM staging rules through clinical assessment
* **Clinical stage system**: The staging system used to stage the cancer
* **Pathologic stage group**: The category describing the level of the disease, following to the TNM staging rules through pathologic assessment
* **Pathologic stage system**: The staging system used to stage the cancer
* **Comments**: Any comments regarding the disease

## <mark style="color:blue;">**Outcome**</mark>

### Cancer disease status

* **Date of evaluation**: The date of the patient’s outcome was assessed
* **Disease status**: The status of the patient’s disease based on the collective tests, treatments, imaging data etc. of the trajectory of the cancer
* **Comments**: Any comments about the outcome of the patient

### Death

* **Date**: The date of death
* **Comments**: Any comments about the death of the patient



## <mark style="color:blue;">**Genomic**</mark>

### Genetic variant found

* **Date**: The date the genetic mutation test was performed
* **Test name**: The name of the genetic test that was done
* **Gene**: The gene targeted for mutation analysis. The HUGO Gene Nomenclature Committee (HGNC) gene symbol is required. For example, the official gene symbol for the human tumor suppressor gene on chromosome 10 is _PTEN_.
* **cDNA**: Complementary DNA (cDNA) – in the context of an mRNA transcript sequence. Should be in the HGVS standard
* **Protein**: Protein sequence; Should be in the HGVS standard. format expected: p####&#x20;
* **Variant found ID**: The variation identifier assigned by HGVS; a unique integer value e.g., 151003
* **Variant found NM number**: The HGVS expression (also known as the sequence variant) describes the sequence variation in genomic, DNA, and RNA coordinates. The sequence variant of the Mutation variant ID in the HGVS nomenclature standard. The format is “<mark style="color:blue;">reference</mark>:<mark style="color:orange;">description</mark>”\
  e.g. <mark style="color:blue;">NC\_000002.12</mark>:<mark style="color:orange;">g.47480740A>C</mark>
* **Variant found interpretation:** The conclusion drawn from the variant found
* **Genomic source class:** The class the variant found to be categorized as
* **Comments:** Any comments about the genetic variant found

## <mark style="color:blue;">**Treatment**</mark>

### Radiation

* **Date**: The date the radiation procedure was done
* **Location**: The hospital/clinic where the radiation procedure has taken place
* **Procedure**: The type of radiation procedure performed
* **Body site**: Where on the body the radiation procedure was done on
* **Treatment intent**: The purpose of the radiation therapy
* **Comments**: Any comments about the radiation

### Surgery

* **Date**: The date of the surgery
* **Location**: The hospital site the surgery operated at
* **Procedure**: The type of surgical procedure done
* **Body site**: The body location the surgery was performed
* **Treatment intent**: The purpose of the surgery
* **Comments**: Any comments about the surgery

### Medication

* **Medication**: The medication name
* **Period**: The period of time the medication was taken. From the first date the medication was taken to when the medication was last taken
* **Termination reason**: The reason for ending medication
* **Treatment intent**: The purpose of taking the medication
* **Comments**: Any comments about the medication

## <mark style="color:blue;">**Lab/Vital**</mark>

### General metrics

* **Date of evaluation**: The vitals assessment date
* **Location**: The hospital/clinic the blood was drawn
* **Height (cm)**: The patient’s height in centimeters
* **Weight (kg)**: The patient’s weight in kilograms
* **Blood pressure diastolic (mmHg)**: The diastolic reading referring to the blood pressure when the heart muscle is between contractions in millimeters of mercury; the relaxation phase
* **Blood pressure systolic (mmHg)**: The systolic reading referring to the blood pressure when the heart muscle is contracting in millimeters of mercury; contraction phase
* **Comments**: Any comments about the patient’s vitals

### CBC

* **Date**: The date of the Complete Blood Count (CBC) test was done
* **CBC type**: The CBC test done
* **CBC count**: The integer value of the chosen CBC type (in previous field)
* **Comments**: Any comments about the complete blood count

### CMP

* **Date**: The date of the Comprehensive Metabolic Panel (CMP) test was done
* **CMP type**: The metabolic panel test done
* **CMP count**: The integer value of the chosen CMP type (in previous field)
* **Comments**: Any comments about the metabolic panel

### Tumor test

* **Date**: The date the tumor test was done
* **Tumor test code**: The name of the tumor marker test conducted
* **Tumor test result**: The result of the tumor marker test
* **Comments**: Any comments about the tumor marker test

### Investigations

* **Date**: The date of radiology/diagnostic test performed
* **Procedure**: The type of diagnostic test done
* **Findings**: The result of the radiology/diagnostic test

## <mark style="color:blue;">**Biospecimens**</mark>

* **Date of collection**: The date the specimen was collected
* **Specimen type**: The state/form of the specimen
* **Specimen cellularity (%)**: The percentage of cellularity in the specimen
* **Location of collection**: The hospital site where the specimen was collected
* **Location of storage**: The site where the specimen was stored
* **Banking ID**: The banking identifier for the specimen
* **Is the tumor paired with blood sample?**: Whether or not the tumor specimen was associated with a blood sample
* **Is there imaging available on the date of the specimen collection?**: Whether or not there was an image available on the date the specimen was collected
* **Comments:** Any comments about the specimen

## <mark style="color:blue;">**Family Pedigree**</mark>

Fields for each family member (\*Pop out form):

* **Unique ID**: The unique identifier for the family member
* **Name**: The relationship of the family member to the patient
* **Age**: The current age of the family member
* **Year of Birth**: The birth year of the family member
* **Choices**: Male, Female, Unknown: The gender of the family member
* **Choices:** Alive, Deceased: The state of life of the family member
* **Reproduction**: The reproduction status of the family member
* **Age of Diagnosis**: State the age in which the family member was diagnosed for each of the disease listed, if applicable

## <mark style="color:blue;">**NF1 Clinical Features**</mark>

### Diagnostic

* **Date of diagnosis**: The date the patient was diagnosed with NF1
* **Clinical diagnosis**: The type of NF1 clinical diagnosis
* **Mode of transmission**: The manner in which NF1 was transmitted
* **Diagnostic criteria**: The conditions the NF1 patient has met
* **Severity (Riccardi scale)**: The Riccardi scale used to evaluate the level of severity of the disease
* **Visibility (Ablon scale)**: The level of visibility of the disease based on the Ablon scale
* **Age of puberty/menarche**: The age of the first menstruation occurrence
* **Head circumference (cm)**: The measurement around the patient’s head
* **Comments**: Any comments about the NF1 diagnosis

### Manifestations

* **Date of diagnosis**: The diagnosis date for manifestations
* **Type**: The type of NF1 manifestations
* **Evaluation**: The overall evaluation of the manifestations
* **Comments**: Any comments about the manifestations

### Skin lesions

* **Date of diagnosis**: The diagnosis date for skin lesions
* **Type**: The type of skin lesions
* **Evaluation**: The overall evaluation of the skin lesions
* **Number**: The number of skin lesion present
* **Location**: The location of the skin lesion on the body
* **Comments**: Any comments about the skin lesions





Reference:\
[http://hl7.org/fhir/us/mcode/artifacts.html](http://hl7.org/fhir/us/mcode/artifacts.html)

[https://loinc.org/89262-0/](https://loinc.org/89262-0/)

[https://www.cancer.gov/publications/dictionaries/cancer-terms/def/karnofsky-performance-status](https://www.cancer.gov/publications/dictionaries/cancer-terms/def/karnofsky-performance-status)

[https://github.com/cBioPortal/oncotree](https://github.com/cBioPortal/oncotree)

[https://mcodeinitiative.github.io/ValueSet-onco-core-TNMPrimaryTumorCategoryVS.html](https://mcodeinitiative.github.io/ValueSet-onco-core-TNMPrimaryTumorCategoryVS.html)

[http://varnomen.hgvs.org/bg-material/simple/](http://varnomen.hgvs.org/bg-material/simple/)
