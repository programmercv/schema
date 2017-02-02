### prtfl.io Résumé Schema

The prtfl.io Résumé Standard is an open source [JSON Schema](http://json-schema.org/) Definition to store résumé data.

It is heavely influenced by the existing resume standards [FRESCA](https://github.com/fresh-standard/FRESCA) and [JSONResume](https://github.com/jsonresume/resume-schema), then cherry-picked and adopted to the needs and requirements of [prtfl.io](https://prtfl.io) and [RésuméExporter](https://github.com/prtflio/resume_exporter).

## Why?

![standards](http://imgs.xkcd.com/comics/standards.png)

Not really intended to set *the standard* for résumés, nor to replace existing ones. In fact, prtfl.io and RésuméExporter are designed to work with FRESCA- and JSONResume-based schemas. But both schema definitions were missing some elements, and we needed a clearly defined schema definition for [prtfl.io](https://prtfl.io) and the prtfl.io jekyll theme (coming soon), in a public place, where people can read, understand, discuss, change and use it.

- [**prtfl.io Resume Schema Definition**](schema.json)
- [**Example Resume**](resume.json)

Structure Overview:

```javascript
{
  "meta": {
    "format": "",
    "version": ""
  },

  "basics": {
    "name": "",
    "label": "",
    "image": "",
    "summary": "",
    "contact": {
      "email": "",
      "phone": "",
      "website": "",
      "location": "",
      "social": [{
        "network": "",
        "user": "",
        "icon": "",
        "url": ""
      }]
    }
  },

  "employment": {
    "summary": "",
    "history": [{          
      "employer": "",
      "position": "",
      "url": "",
      "start": "",
      "end": "",
      "summary": "",
      "location": "",
      "highlights": [""],
      "keywords": [""]
    }]
  },

  "education": {
    "summary": "",
    "history":[{
      "title": "",
      "institution": "",
      "fieldOfStudy": "",
      "degree": "",
      "start": "",
      "end": "",
      "grade": "",
      "url": "",
      "summary": "",
      "location": ""
      "curriculum": [""],
      "highlights": [""],
      "keywords": [""]
    }]
  },

  "projects": {
    "summary": "",
    "history": [{
      "title": "",
      "description": "",
      "url": "",
      "repo": "",
      "start": "",
      "end": "",
      "images": [{            
        "thumbnail": "",
        "big": ""
      }],
      "highlights": [""],
      "keywords": [""]
    }]
  },

  "openSource": {
    "summary": "",
    "history": [{
      "title": "",
      "description": "",
      "summary": "",
      "role": "",
      "url": "",
      "repo": "",
      "start": "",
      "end": "",
      "highlights": [""],
      "keywords": [""]
    }]
  },

  "skills": {
    "summary": "",
    "history": [{
      "name": "",
      "description": "",
      "keywords": [""]
    }]
  },

  "qualifications": {
    "summary": "",
    "history": [{
      "category": "",
      "title": "",
      "date": "",
      "from": "",
      "summary": "",
      "url": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "recognition": {
    "summary": "",
    "history": [{
      "category": "",
      "title": "",
      "date": "",
      "from": "",
      "summary": "",
      "url": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "writing": {
    "summary": "",
    "history": [{
      "title": "",
      "category": "",
      "date": "",
      "url": "",
      "summary": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "reading": {
    "summary": "",
    "history": [{
      "title": "",
      "category": "",
      "url": "",
      "author": "",
      "date": "",
      "summary": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "speaking": {
    "summary": "",
    "history": [{
      "title": "",
      "event": "",
      "location": "",
      "date": "",
      "summary": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "patents": {
    "summary": "",
    "history": [{
      "title": "",
      "url": "",
      "number": "",
      "status": "",
      "description": "",
      "date": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "languages": {
    "summary": "",
    "history": [{
      "language": "",
      "level": "",
      "years": ""
    }]
  },

  "interests": {
    "summary": "",
    "history": [{
      "name": "",
      "description": ""
    }]
  },

  "extracurricular": {
    "summary": "",
    "history": [{
      "title": "",
      "activity": "",
      "location": "",
      "start": "",
      "end": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "affiliation": {
    "summary": "",
    "history": [{
      "category": "",
      "organization": "",
      "role": "",
      "url": "",
      "start": "",
      "end": "",
      "summary": "",
      "location": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "governance": {
    "summary": "",
    "history": [{
      "summary": "",
      "category": "",
      "role": "",
      "organization": "",
      "start": "",
      "end": "",
      "keywords": [],
      "highlights": []
    }]
  },

  "service": {
    "summary": "",
    "history": [{
      "category": "",
      "organization": "",
      "position": "",
      "url": "",
      "start": "",
      "end": "",
      "summary": "",
      "location": "",
      "highlights": [],
      "keywords": []
    }]
  },

  "references": {
    "summary": "",
    "history": [{
      "name": "",
      "role": "",
      "summary": ""
    }]
  },

  "disposition": {
    "summary": "",
    "history": [{
      "travel": "",
      "authorization": "",
      "commitment": [],
      "remote": true,
      "relocation": {
        "willing": "",
        "destinations": []
      }
    }]
  },
}

```