This repository  contains a set of Python notebooks to convert LDH datasets into the format that the CM expects from the UM.

There is a folder for each case study that contains:

- A `data` folder with the JSON extracted from LDH
- A notebook called `<caseStudy>Parser` that performs the transformation. 

These notebooks area customizable for some variations in case studies.

The notebooks generate some JSON files with `ugc` prefix, stored in the corresponding data folder. These data can be sent to the CM using `POST:/users/{user-id}/update-generated-content` endpoint.

Notebooks also contain examples to use these files to send POST requests.
