# Image Finder

## Brief
We would like to build a JS application that displayes a set of images.

A basic service would have the following functionalities:
- Fetch data from the NASA external API: https://images-api.nasa.gov/search?q=moon
- Transform the data
- Display on the page

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

Here is what we expect to see in the page:

```
<div>
    <img src="https://images-assets.nasa.gov/image/PIA12235/PIA12235~thumb.jpg" />
    <img src="https://images-assets.nasa.gov/image/PIA12235/PIA12236~thumb.jpg" />
    <img src="https://images-assets.nasa.gov/image/PIA12235/PIA12237~thumb.jpg" />
    (...)
</div>
```

## Extensions
We could plan to extend the service by introducing:
- Test coverage or implementing directly a TDD approach
- Content stylyng using CSS/SASS

## Notes

You are free to code and run the application using any IDE/text editor of your choice.
You can search the web for information as you'd do in normal work day or ask your interviewers for help and collaboration.
