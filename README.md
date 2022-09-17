# Malloy Fiddle

Malloy Fiddle allows you to build a web page to play with a data set. My simply copying a couple of files (index.html and samples.json) into a directory on a web server along with some data and some Malloy semantic models, you can run queries using your web browser as an analytic tool.

Malloy Fiddle is implemented in Malloy, DuckDB+WASM.  The javascript program is loaded from this repository the data is served from your webserver.

Github allows you to host web pages so it is perfect for this.  You can create a repository, with a aformentioned files and be able to play with data.  

## Example Fiddles

Here are some examples running on Github

[NTSB Example data](https://looker-open-source.github.io/malloy/fiddle/index.html?q=12+-+Line+Chart+with+two+dimension%3A+Flights+by+Month+and+Length&m=Flights&t=)

IMDB Fiddle - [Github Repository](https://github.com/lloydtabb/imdb_malloy)  [Fiddle](https://lloydtabb.github.io/imdb_fiddle/index.html)

## Making a Fiddle

  * Load VScode and Intall the extension - (Goto Instructions)[https://github.com/looker-open-source/malloy/#readme}]
  * Find some *parquet* or *csv* data and make a new Malloy Model
  * Create a separate Malloy file for queries using an `import`
  * download [samples.json](samples.json) and edit it.
  * download [index.html](index.html) into the same directory
  * take all the files an add them to a github repo
  * in Github, open Settings / Pages
    * Set Branch to Main
    * directory to Root
  * Click the Visit Site link.

  If you have a public Fiddle, please let us know, we'd love to add it to this list.