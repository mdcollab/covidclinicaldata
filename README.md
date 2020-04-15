# Coronavirus Disease 2019 (COVID-19) Clinical Data Repository

This is an effort to compile a repository of the clinical characteristics of COVID-19 tested patients. By sharing our schema and data, we hope that we can 1) accelerate information sharing among frontline healthcare providers and 2) facilitate studies on COVID-19 signs, symptoms, stages, and care plans.

## Data

The repository is maintained in <a href="https://docs.google.com/spreadsheets/d/11IuOqJ_L0wYcbDqovmDaASR2aae79I5a9wpGVOuQ9bU/edit?usp=sharing" target="_blank">Google Sheets</a> and as a [CSV](data/carbonhealth_and_braidhealth/ALL/4.6_carbonhealth_and_braidhealth.csv). Each row represents a COVID-19 tested patient. More details are available in the [data dictionary](https://docs.google.com/spreadsheets/d/1p9rtv2LjVCPb54MdGe8ZqJ1zF3McIFnzq-ZhhjWgguI/edit?usp=sharing).

New data from our contributors and Carbon Health will be compiled and published, weekly on Tuesdays (containing data for the previous week). The list of contributors and supporters is maintained in the section below. 

## <a name="contribs"></a> Contributors and Supporters

### Data Contributors

#### Carbon Health — Clinical characteristics and laboratory findings

- Website: <a href="https://carbonhealth.com/coronavirus" target="_blank">Carbon Health</a>
- Twitter: <a href="https://twitter.com/CarbonHealth" target="_blank">@CarbonHealth</a>
- Email: <covidclinicaldata@carbonhealth.com>
- Notes: 
    1. Each row includes the characteristics of a patient who has taken the COVID-19 test. Carbon Health began COVID-19 testing with the SARS-CoV-2 RNA RT-PCR test on 3.7.20. 
    2. The data includes **clinical characteristics** in addition to **radiological** and **laboratory** findings. It does not include **treatment plans**, **complications**, and **clinical outcomes**; this data would come from in-patient facilities.
    3. The data includes both positive- and negative-tested patient characteristics. As of 4.6.20, these include the characteristics of symptomatic patients, those in professions with a high risk of exposure, and/or those who may have been exposed through contact with a known infected person. 
    4. Clinician-assessed symptoms are sparse for data published on 4.6.20 due to some criteria having been added later. 
    5. A patient's reported age differs from their actual age by a reasonable randomized amount to protect their privacy. We remain compliant with [HIPAA Privacy Rule's De-Identification Standard](https://www.hhs.gov/hipaa/for-professionals/privacy/special-topics/de-identification/index.html#standard).

    
| ![CH Logo](contributors/logos/carbon_health.png) | <img src="contributors/samples/carbon_health_dictionary.png" width="60%"> |
|:--:| :--: |
| Carbon Health Logo | [Data Dictionary](https://docs.google.com/spreadsheets/d/1p9rtv2LjVCPb54MdGe8ZqJ1zF3McIFnzq-ZhhjWgguI/edit?usp=sharing) |

#### Braid Health — Chest x-rays, findings, and clinician impressions

- Website: <a href="https://braid.health/www" target="_blank">Braid Health</a>
- Twitter: <a href="https://twitter.com/BraidHealth" target="_blank">@BraidHealth</a>
- Email: <vivian@braid.health> and <k@braid.health>
- Notes:
    1. Findings, clinician impressions, and links to chest x-rays are included. 
    2. The links direct to the Braid Health website. This allows for closer inspection by researchers and radiologists. 
    3. The images can be downloaded for image processing and classification studies.

| <img src="contributors/logos/braid_health.png" width="60%"> |  <img src="contributors/samples/braid_health_c_xray.png" width="60%"> |
|:--:| :--:| 
| Braid Health Logo | [Sample Chest X-ray](https://braid.health/viewer/study/6905c8c988d201379dd932fa5ba650125d89bc5bddfa6a4df9f4338cbd2326f2?key=BIo8HvL8W_dy__4IdBFd1pxP3xoibTLfRwG4ErLo9Okog3RzXmcB0VJL-7onLz9PlL4OpSzut_hzZZGPnC6LX0&lab=sars) |

### Supporters

Special thanks to <a href="https://braid.health/www" target="_blank">Kevin Quennesson</a>, <a href="https://profiles.stanford.edu/nigam-shah" target="_blank">Nigam Shah</a>, and [Andrew Therriault](https://www.andrewtherriault.com/) for their support of this effort and for their feedback.

## Call for Data 

To ensure this data is representative of cases with varying severity levels and symptoms, we are requesting data from out-patient test centers and in-patient healthcare facilities which are treating COVID-19. 
Please use either one of the templates provided below and email the data to <covidclinicaldata@carbonhealth.com>. Further, please share any studies on this data via email or a <a href="https://github.com/mdcollab/covidclinicaldata" target="_blank">pull request</a>. 

### Templates for Out-patient Test Centers

Here are the available templates for out-patient test centers and clinics:

- <a href="https://docs.google.com/spreadsheets/d/18dGt8lZQsaAL0X4OPDICWVU2LtTBhRQufR2eBcLVgPA/edit?usp=sharing" target="_blank">Google Sheets</a>
- <a href="templates/outpatient/4.6_outpatient_template.xlsx" target="_blank">Excel</a>
- [CSV](templates/outpatient/4.6_outpatient_template.csv)

Details about the fields are available in the [data dictionary](https://docs.google.com/spreadsheets/d/1p9rtv2LjVCPb54MdGe8ZqJ1zF3McIFnzq-ZhhjWgguI/edit?usp=sharing).

### Templates for In-patient Healthcare Facilities

In-patient healthcare providers can contribute additional columns for **treatment plans**, **complications**, and **clinical outcomes** using one of the following templates:

- <a href="https://docs.google.com/spreadsheets/d/18dGt8lZQsaAL0X4OPDICWVU2LtTBhRQufR2eBcLVgPA/edit?usp=sharing" target="_blank">Google Sheets</a>
- <a href="templates/inpatient/4.6_inpatient_template.xlsx" target="_blank">Excel</a>
- [CSV](templates/inpatient/4.6_inpatient_template.csv)

Details about the fields are available in the [data dictionary](https://docs.google.com/spreadsheets/d/1p9rtv2LjVCPb54MdGe8ZqJ1zF3McIFnzq-ZhhjWgguI/edit?usp=sharing).

## Citation

Use the format below to cite the data repository in your studies, remembering to update your date of access.

```
@dataset{2020covidclinicaldata,
  author =       {Carbon Health and Braid Health},
  title =        {Coronavirus Disease 2019 (COVID-19) Clinical Data Repository},
  howpublished = {Accessed on yyyy-mm-dd from \url{https://covidclinicaldata.com/}},
  year =         2020,
  version =      {1.0}
}
```

## Data Sharing Agreement

This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>


