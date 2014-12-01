Reactjs Component for Facebook like photo/image grids
=====================================================

This component shows images in a neat square (or whatever dimensions you want) grid. Acts like facebooks image grids. Switches between two modes randomly (small images on right or bottom).

![How it looks](https://www.flickr.com/photos/mukeshsoni/15736005117/ "How it looks")

#Usage
```
var imageData = [
            path: 'http://lorempixel.com/400/400/'
            path: 'http://lorempixel.com/500/700/'
            path: 'http://lorempixel.com/600/500/'
            path: 'http://lorempixel.com/600/800/'
    ];
var imageGrid = (
            <ReactImageGrid
                onImageClick={handleImageClick}
                data={imageData} />
            );
React.render(imageGrid, document.getElementById('container'));
```

You can also pass gridSize as a property. It's a string which consists of width and height separated by an x. E.g. gridSize="500x500".

If you don't pass any gridSize, the grid size is chosen based on the parent's width.
