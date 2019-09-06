# Submission terms

Adds a submission terms object to the tender and lot objects, to describe how, when and where the tenderers must submit their bids.

## Guidance

## Legal context

In the European Union, this extension's fields correspond to [eForms BG-102 (Submission Terms)](https://github.com/eForms/eForms), although not all the fields have been implemented yet. See [OCDS for the European Union](http://standard.open-contracting.org/profiles/eu/master/en/) for the correspondences to Tenders Electronic Daily (TED).

## Example


```json

{
  "tender": {
    "submissionTerms": {
      "electronicSubmissionPolicy": "required",
      "electronicCataloguePolicy": "allowed",
      "variantPolicy": "notAllowed",
      "languages": [
        "fr",
        "es"
      ],
      "bidValidityPeriod": {
        "startDate": "2019-09-20",
        "endDate": "2019-11-20",
        "maxExtentDate": "2019-12-02",
        "durationInDays": 74
      },
      "hasRequiredGuarantees": true
    }
  }
}

```

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.
