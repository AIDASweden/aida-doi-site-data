# aida-doi-site-data

This repo holds the data file for the aida-doi-site, *issued_dois.json*. This is the only file that has to be updated when new DOIs are issued. For each DOI, one or more links has to be defined to the data sets for which the DOI is issued. This can be For restricted access datasets, a contact email address can be specified instead of a url.

## Format
```
{
  "DOIs": {
    "10.23698/aida/PACSCODE": {
      "data-links": [
        "https://path.to/data/set"
      ],
      "access-request-links": [
        "email@address.se",
      ]
    }
  }
}
```
For ease of interaction with DICOM systems and clinicians, AIDA prefers to issue
DOIs on the form

`aida/PACSCODE`

where PACSCODE should be short and recognizable (4 characters for now).

## Acknowledgements

The AIDA DOI site was heavily inspired by [doi.nbis.se](https://doi.nbis.se).
Thank you for the [source code](https://github.com/NBISweden/doi-bils-site)!
