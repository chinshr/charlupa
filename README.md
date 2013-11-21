Charlupa
========

Description
-----------

Charlupa is a simple natural language processing API written in Python. It interprets English sentences, extracts information and returns JSON structures, that contain the extracted information in a machine digestible format.

Examples
--------

Request:

    [GET]  http://charlupa.herokuapp.com/api/extract?phrase=taking+a+day_off_tomorrow

Response:

    { "category": "TIMEOFF", 
      "action": "CREATE_REQUEST",
      "entities": {
        "daterange": [{"start": "2013-11-21", "end": "2013-11-21"}],
        "message": ["day off"],
        "keywords: ["vacation"]
      }, 
      "context": {
        "language": "en"
      }
    }

Resources
---------

* Installing Django -- https://docs.djangoproject.com/en/dev/intro/install/
* Restless: REST API framework -- github.com/dobarkod/django-restless
* Restless: documentation -- http://django-restless.readthedocs.org
