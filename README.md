Frontend test
===========
You should create simple shopping basket prototype. All data needed to complete this goal is presented in the current repository.

Project structure
--------------------
```
Destination           | Description
--------------------- | ----------------------
data/                 | 
   categories.json    | List of all categories
   galleries.json     | List of all galleries
   products.json      | List of all products
images/               | Dir with galleries
   gallery1/          |
   gallery2/          |
   ...                |
   galleryN/          |
lib/                  | 3rd party libraries go here
src/                  | Your source goes here
index.html            | Application entry point
README.md             | This readme
```

Data structure
-----------------

- Project **HAS ONE** Category specified by ```category_id``` field
- Project **HAS ONE** Gallery specified by ```gallery_id``` field
- Gallery **CONSISTS OF** multiple images

Gallery structure
--------------------
If we have next gallery:
```json
{ 
  "galleries": [
    {
      "id": "some_gallery_id",
      "images": [
        "1.jpg",
        "2.png"
      ]
    }
  ]
}
```

it means that pictures should be loaded by next pathes:
 
```
images/some_gallery_id/1.jpg
images/some_gallery_id/2.png

etc...
```
