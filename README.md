This assignment was undertaken for Contexts of Information Visualization | MICA | MPS InfoVis. It represents my second attempt to develop a visualization using the D3.js library. In this instance, I have appropriated the code of Ilya Yaubovich’s Game of Thrones family tree. I have adjusted this framework to represent the taxonomy of the hominid family evolution.
Note that there are a lot of imperfections in the way the visualization is currently displayed. I aim to improve on those in future work as my skills evolve!

To view the visualization go here:

https://quantartist.github.io/quantartist.tree.github.io/

For Illya’s original work see:

http://ilyayakubovich.com/descendant_tree/#stark

http://ilyayakubovich.com/descendant_tree/book.html#stark

Referencing Yakabuvich:

You have to run this from a server (can't just open the HTML file). The easiest way to do this, if you have python installed, is to run
python -m SimpleHTTPServer this will start a python server at 0.0.0.0:8000
Use #sourcename to load a specific JSON file.

0.0.0.0:8000#stark loads json/stark.json

Trees are stored in a simple JSON format, and repeating portions can be handled using the "source" attribute.

For example, { "name":"John Smith", "source":"json/children_of_john_smith.json" }
This is useful for trees with cycles (cousins marrying each other) and multiple trees sharing the same descendants (this is common if you have trees for more than one of your ancestors).

Uses d3.js to draw the tree.

Based on Rob Schmuecker’s example: http://bl.ocks.org/robschmuecker/7880033

