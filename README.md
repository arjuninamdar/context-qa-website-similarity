# ContextQA Test for Similarity

One issue facing ContextQA's testing automation platform was, upon running a previously saved test on a given website, how do you run that same test when the HTML elements are altered through the development process? What parts of the HTML element do you look like to determine the corresponding element on a "new" iteration of the same website, and what techniques do you use to most effectively analyze these parts of the element? 

The code provided in this repo sought to provide an understanding of what to look for when determining this corresponding element. Using the Wayback Machine, new and old iterations of many of the same sites were scraped. Elements on each of the "old" sites were randomly selected, and their "new" versions were found by hand. From there, a variety of tests were run comparing the "old" element to all elements on the new site, including: 

- Cosine similarity for all parts of a given HTML element
- Jaccard indexing for the attributes of a given HTML element
- etc. 

From here, the data from each of the tests were compiled and analyzed. Effective methods when determining a corresponding "new" element would have relatively large average score differences when comparing the actual new element and the other new elements.

The data collected from a small dataset is provided in the repo. 
