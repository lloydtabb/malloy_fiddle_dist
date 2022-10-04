# Malloy Fiddle

Malloy is an experimental language for data ([learn more about Malloy](https://github.com/looker-open-source/malloy/blob/main/README.md).

Malloy Fiddle allows you to build a web page to examine with a small static data set. By simply copying a couple of files (index.html and samples.json) into a directory on a web server along with some data and some Malloy semantic models, you can run queries using your web browser as an analytic tool.

Malloy Fiddle is implemented in Malloy, DuckDB+WASM.  The javascript program is loaded from this repository the data is served from your webserver.

Github allows you to host web pages so it is perfect for this.  You can create a repository, with a aformentioned files and be able to play with data.  

## Example Fiddles

Here are some examples running on Github

### [NTSB Example Fiddle](https://looker-open-source.github.io/malloy/fiddle/index.html?q=12+-+Line+Chart+with+two+dimension%3A+Flights+by+Month+and+Length&m=Flights&t=)
Extract of NTSB flight data from 2000-2005.  Shows how to join data and biild dashboards

### [IMDB Fiddle](https://lloydtabb.github.io/imdb_fiddle/index.html)
Educational example of an extract of the most popular movies in the IMDB dataset. [Source Code in Github Repository](https://github.com/lloydtabb/imdb_fiddle) 

### [Baby Names Fiddle](https://lloydtabb.github.io/name_fiddle/index.html)
The Social Security Administration collects baby first names and genders by state and year.  Explore this dataset.
 [Source Code in Github Repository](https://github.com/lloydtabb/name_fiddle) 

### [Querying File System Fiddle](https://lloydtabb.github.io/malloy_fiddle_dist/examples/files/index.html)
Shows how to model hierarchical data.  Creates a reasonable interface to the ways you might want to 
query it.
 [Source Code in Github Repository]https://github.com/lloydtabb/malloy_fiddle_dist/tree/main/examples/files) 


## Making a Fiddle using Github Pages

  * Load VScode and Intall the extension - [Instructions](https://github.com/looker-open-source/malloy/#readme)
  * Find some *parquet* or *csv* data and make a new Malloy Model
  * Create a separate Malloy file for queries using an `import`
  * download [samples.json](samples.json) and edit it.
  * download [index.html](index.html) into the same directory
  * take all the files an add them to a github repo
  * in Github, open Settings / Pages
    * Set Branch to Main
    * directory to Root
  * Click the Visit Site link.

  If you have a interesting public Fiddle, please let us know, we'd love to add it to this list.
