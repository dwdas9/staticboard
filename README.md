![](images/excalidraw_shawshank_redemption.jpg)

# StaticBoard

I wanted an Excalidraw-style whiteboard that I could use on machines where I could not install software or paste sensitive information into an online service.

Running Excalidraw locally is possible, but it still requires some setup. I wanted something simpler: one HTML file that I could download, open in a browser, and use offline.

That became StaticBoard.

## Run it

1. Download `index.html`.
2. Open it in your browser.

There is nothing to install and no server to start.

## Features

StaticBoard includes the drawing tools I use most often:

- Shapes, arrows, text, and freehand drawing
- Images and screenshots
- Undo and redo
- Zoom and canvas navigation
- PNG and SVG export
- Editable Excalidraw file support
- Local saving in the browser

It also includes a few changes for working with screenshots:

- Paste screenshots directly onto the board
- Add a soft shadow to an image
- Draw arrows from inside an image to the surrounding canvas

## What is not included

StaticBoard does not have:

- User accounts
- Real-time collaboration
- Cloud storage
- Team administration
- Backend services

The board is meant for local, individual use.

## How it fits into one file

StaticBoard is built with React and uses Excalidraw as its drawing engine.

A normal web application keeps its JavaScript, CSS, and other files separately. In StaticBoard, the application code and styling are bundled into `index.html`, so the browser can run it directly from that file.

Images are processed in the browser, and the current board is saved locally. StaticBoard does not send your drawings to its own server.

## Credits

StaticBoard uses the open-source Excalidraw editor as its drawing engine.

The purpose of this project is to make that drawing experience easier to carry and use on machines where installing or hosting a full application is not practical.

## Project status

StaticBoard is still being improved. The main idea will remain the same: download one file, open it, and start drawing.