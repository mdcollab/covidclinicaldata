# Coronavirus Disease 2019 (COVID-19) Clinical Data Repository

This is an effort to compile a repository of the clinical characteristics of patients who have taken a COVID-19 test. By sharing our schema and data, we hope that we can 1) accelerate information sharing among frontline healthcare providers and 2) facilitate studies on COVID-19 signs, symptoms, stages, and care plans.

## The Repository

The repository is maintained as [CSV files](https://github.com/mdcollab/covidclinicaldata/tree/master/data/) and in <a href="https://docs.google.com/spreadsheets/d/11IuOqJ_L0wYcbDqovmDaASR2aae79I5a9wpGVOuQ9bU/edit?usp=sharing" target="_blank">Sheets</a> and is compliant with <a href="https://www.hhs.gov/hipaa/for-professionals/privacy/special-topics/de-identification/index.html#standard" target="_blank">HIPAA Privacy Rule's De-Identification Standard</a>. Details about each field are available in the <a href="https://docs.google.com/spreadsheets/d/1p9rtv2LjVCPb54MdGe8ZqJ1zF3McIFnzq-ZhhjWgguI/edit?usp=sharing" target="_blank">data dictionary</a>.

### Refresh Cadence and Organization 

* Each file contains a week's worth of results from Carbon Health and Braid Health.  
* Each filename is prefixed with the date (mm-dd) the query was run, matching `batch_date`.
* Each row contains the clinical characteristics of a patient who has taken a COVID-19 test. 
* The first batch, prefixed with 04-07, contains a month's worth of results starting from 03-07.

### Supplementary Material

* Motivations, details, and next steps are available in this [discussion](https://twitter.com/erenbali/status/1261083321158770689?s=20) from May 2020.
* Data preparation and summarization functions are available in these [two notebooks](https://github.com/mdcollab/covidclinicaldata/tree/master/notebooks/). For example, below is a visualization of the fill rate for all variables within the data repository.

![Fill rates](images/06-16_fill_rate.png) 

## Data Contributors and Supporters

### Carbon Health — Clinical characteristics and laboratory findings

- Website: <a href="https://carbonhealth.com/coronavirus" target="_blank">Carbon Health</a>
- Twitter: <a href="https://twitter.com/CarbonHealth" target="_blank">@CarbonHealth</a>
- Email: <covidclinicaldata@carbonhealth.com>
- Notes: 
    * Carbon Health began COVID-19 testing with the SARS-CoV-2 RNA RT-PCR test on 03-04-20. 
    * The data includes **clinical characteristics** (epi factors, comorbidities, vitals, clinician-assessed symptoms, patient-reported symptoms) in addition to **radiological** and **laboratory** findings. It does not include **treatment plans**, **complications**, and **clinical outcomes**, which is collected at inpatient facilities.
    * The data includes both positive and negative test results. These include results from symptomatic patients, those in professions with a high risk of exposure, and/or those who may have been exposed through contact with a known infected person. The data also includes test results for asymptomatic patients. 
    * The data includes test results of patients with mild symptoms and asymptomatic patients. It does not include results for patients with severe symptoms. We refer such patients to ER.
    * A patient's reported age differs from their actual age by a reasonable randomized amount to protect their privacy.
    * It is important to note that our data collection is clinically-driven and therefore not systematic. This means that overall positive rates are descriptive of the Carbon Health patient population and cannot be generalized to the unobserved population. We do provide [functions](https://github.com/mdcollab/covidclinicaldata/tree/master/notebooks/data_processing.ipynb) to identify symptom severity to aid in accounting for the various admission criteria that affect positive rates.
- Acknowledgements:
  - Data Science Team: [Nosheen Moosvi](https://www.linkedin.com/in/nosheen-moosvi-82a31883/), [Rebekkah Ismakov](https://www.linkedin.com/in/rismakov/), [Pardis Noorzad](https://djpardis.com)
  - Clinical Team: [Greg Burrell](https://www.linkedin.com/in/gregburrell/),  [Haritha Atluri](https://www.linkedin.com/in/harithaatluri/), [Roger Wu](https://www.linkedin.com/in/roger-wu-md-mba-facep-b91844a/), [Caesar Djavaherian](https://www.linkedin.com/in/caesar-djavaherian/), [Sujal Mandavia](https://www.linkedin.com/in/sujal-mandavia-03664414/)
    
| ![CH Logo](contributors/logos/carbon_health.png) | <img src="contributors/samples/carbon_health_dictionary.png" width="60%"> |
|:--:| :--: |
| Carbon Health Logo | <a href="https://docs.google.com/spreadsheets/d/1p9rtv2LjVCPb54MdGe8ZqJ1zF3McIFnzq-ZhhjWgguI/edit?usp=sharing" target="_blank">Data Dictionary</a> |

### Braid Health — Chest x-rays, findings, labels, and clinician impressions

- Website: <a href="https://braid.health/www" target="_blank">Braid Health</a>
- Twitter: <a href="https://twitter.com/BraidHealth" target="_blank">@BraidHealth</a>
- Email: <vivian@braid.health> and <k@braid.health>
- Notes:
    * The data is joined with Carbon Health data using the MRN and encounter ID fields, which are then excluded from the data.
    * The data includes findings, clinician impressions, labels, and links to chest x-rays. 
    * The links direct to the Braid Health website. 
    * The website UI allows for closer inspection by researchers and radiologists. 
    * The images can be downloaded for image processing and classification studies.
    * A patient’s reported age differs from their actual age by a reasonable randomized amount to protect their privacy.
- Acknowledgements:
  - Data Engineering: [Kevin Quennesson](https://www.linkedin.com/in/qevni/), [Daniel Hasegan](https://www.linkedin.com/in/dhasegan/), [Üstün Özgür](https://www.linkedin.com/in/ustunozgur/)
  - Product Design: [Alessandro Sabatelli](https://www.linkedin.com/in/s4l4x/)
  - Clinical: [Rajni Natesan](https://www.linkedin.com/in/rajninatesan/), [Vivian Liu](https://www.linkedin.com/in/viviandliu/)

| <img src="contributors/logos/braid_health.png" width="60%"> |  <img src="contributors/samples/braid_health_c_xray.png" width="60%"> |
|:--:| :--:| 
| Braid Health Logo | <a href="https://braid.health/viewer/study/6905c8c988d201379dd932fa5ba650125d89bc5bddfa6a4df9f4338cbd2326f2?key=BIo8HvL8W_dy__4IdBFd1pxP3xoibTLfRwG4ErLo9Okog3RzXmcB0VJL-7onLz9PlL4OpSzut_hzZZGPnC6LX0&lab=sars"  target="_blank">Sample Chest X-ray</a> |

### Supporters

Special thanks to <a href="https://twitter.com/erenbali" target="_blank">Eren Bali</a>, <a href="https://braid.health/www" target="_blank">Kevin Quennesson</a>, <a href="https://profiles.stanford.edu/nigam-shah" target="_blank">Nigam Shah</a>, [Andrew Therriault](https://www.andrewtherriault.com/), [Omer Koren](https://www.linkedin.com/in/omer-koren-24a3a762/), and [Andrew Pikul](http://ajpikul.com) for their support of this effort and for their feedback.

### Call for Data 

To ensure this data is representative of cases with varying severity levels and symptoms, we are requesting data from **outpatient test centers** and **inpatient healthcare facilities** which are treating COVID-19. Please use the <a href="https://docs.google.com/spreadsheets/d/1p9rtv2LjVCPb54MdGe8ZqJ1zF3McIFnzq-ZhhjWgguI/edit?usp=sharing" target="_blank">data dictionary</a> to prepare the data. Please send data and inquiries to <covidclinicaldata@carbonhealth.com>. 

## Research Contributors

Please add your research to this section via a <a href="https://github.com/mdcollab/covidclinicaldata" target="_blank">pull request</a>.
<!-- Please keep this section consistent with the "Data Contributors" section. -->

### Call for Research 

Please share any studies on this data via email or a <a href="https://github.com/mdcollab/covidclinicaldata" target="_blank">pull request</a>. 
You can use the format below to cite the data repository in your studies.

```
@dataset{2020covidclinicaldata,
  author =       {Carbon Health and Braid Health},
  title =        {Coronavirus Disease 2019 (COVID-19) Clinical Data Repository},
  howpublished = {Accessed from \url{https://covidclinicaldata.org/.}},
  year =         2020,
  version =      {4.0}
}
```

## Data Sharing Agreement

This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"  target="_blank">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"  target="_blank"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>


