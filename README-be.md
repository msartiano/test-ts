# Image Finder

## Brief
We would like to build a JS application that exposes organised data.

A basic service would have the following functionalities:
- Fetch data from the NASA external API: https://images-api.nasa.gov/search?q=moon
- Transform the data to a list of images
- Expose the data via an API

Here is an excerpt from https://images-api.nasa.gov/search?q=moon:

```
{
  "collection": {
    "href": "https://images-api.nasa.gov/search?q=moon",
    "version": "1.0",
    "items": [
      {
        "href": "https://images-assets.nasa.gov/image/PIA12235/collection.json",
        "data": [ ... ],
        "links": [
          {
            "href": "https://images-assets.nasa.gov/image/PIA12235/PIA12235~thumb.jpg",
            "render": "image",
            "rel": "preview"
          }
        ]
      }
    ]
  }
}
```

Here is what we expect as a response:

```
/api/getImages?q=dog
Response:
[
    https://images-assets.nasa.gov/image/PIA12235/PIA12235~thumb.jpg,
    https://images-assets.nasa.gov/image/PIA12235/PIA12236~thumb.jpg,
    https://images-assets.nasa.gov/image/PIA12235/PIA12237~thumb.jpg
]
```

## Extensions
We could plan to extend the service by introducing:
- Test coverage or implementing directly a TDD approach
- Security and Caching on API Endpoints
- Frontend service that fetches the data from the API created, and shows in a page

## Notes

You are free to code and run the application using any IDE/text editor of your choice.
You can search the web for information as you'd do in normal work day or ask your interviewers for help and collaboration.
