# Brandeis Course Data

A series of JSON files representing the unabridged course catalogs for every
semester from academic year 2004–2005 through Fall 2018 (may be updated for
future semesters as need arises). The data is about 1.6MB compressed and 33MB
uncompressed.

Generated from [9999years/brandeis-classes].

Each JSON file is named as a year-semester pair, where the semester is a number.

Semester | Number
---------|-------
Spring   | 1
Summer   | 2
Fall     | 3

This is an internal Brandeis convention; semesters are numbered from the start
of the *year*, which is not the same as their order in the *academic year*.

They’re ordered like this so they sort correctly, though.

Each JSON file has a list of objects where each object represents a course and
looks like this:

    {
      "name": "Developmental Cognitive Neuroscience: Infancy through Adolescence",
      "class_number": 7099,
      "subject": "NPSY",
      "number": 182,
      "group": "A",
      "section": "1",
      "schedule": [
        {
          "block": "H",
          "times": "T,F 11:00 AM\u201312:20 PM",
          "location": "Goldsmith Math 226",
          "info": null
        }
      ],
      "enrolled": 15,
      "limit": 20,
      "waiting": 0,
      "enrollment_status": "Open Consent Req.",
      "syllabus": "https://moodle2.brandeis.edu/syllabus/public/7fa378ad0c1dc94d1bba90407ae50531.docx",
      "instructors": [
        {
          "name": "Snyder, Hannah",
          "id": "59a1dbb04a6ca6424acf7f393bfd9862c43ad1c8"
        }
      ],
      "uni_reqs": [
        "ss"
      ],
      "description": "Prerequisites: PSYC 10a or NPSY 11b and either PSYC 33a or NPSY 22b or permission of the instructor.\n\nCurrent research and methods in developmental cognitive neuroscience are surveyed through analysis of journal articles on language, memory, attention, executive functions, and social cognition. Infancy through adolescence are covered in both typically and atypically (Autism, ADHD, etc.) developing populations. Usually offered every second year.\nMs. Snyder",
      "notes": "See Course Catalog for prerequisites.\nInstructor's Signature Required.\nThis is an experiential learning course.",
      "semester": "Spring",
      "year": 2018
    }

Several fields may be `null`, notably `notes`, `syllabus`, and so on. This
information is provided on a best-effort basis and I can make no guarantees for
its correctness — although I’m aware of no glaring mistakes.

For use, see [9999years/brandeis-classes] which contains convenience functions
and so on for loading and manipulating this data.

[9999years/brandeis-classes]: /9999years/brandeis-classes
