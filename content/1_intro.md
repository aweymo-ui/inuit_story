---
title: Introduction
nav: Introduction
gallery: true
---

Hello, my name is Andrew Weymouth and I have worked with the University of Idaho Library as the [Digital Initiatives Librarian](https://www.lib.uidaho.edu/about/people/aweymouth.html){:target="_blank" rel="noopener"} in the [Center for Digital Inquiry and Learning ](https://cdil.lib.uidaho.edu/){:target="_blank" rel="noopener"}(CDIL) department since the fall of 2023. My work generally consists of creating and maintaining our digital collections, collaborating on projects with fellowship recipients, helping to rethink processes and introducing new digital scholarship tools to the department.

## Experience

I come from multi-disciplinary background, creating work about history using long form audio, video, animation and writing that compliments my current work in digital scholarship well. Before joining U of I, I worked as the Digital Media Editor for the Washington State focused digital encyclopedia, HistoryLink, where I helped add visual context to written material and ensured none of the material was copyright protected. 

{% include gallery-figure.html img="cccidaho85.gif" alt="Moving image of CCC workers throwing timber off of a trail" caption="Moving image I created manipulating elements of an archival photograph from the CCC Idaho collection as a part of the 2024 Poster Series" title="Moving image I created manipulating elements of an archival photograph from the CCC Idaho collection as a part of the 2024 Poster Series" width="100%" %}

## Continuing Education

Since moving from Tacoma to Moscow for this position, I have also become a student again, pursuing another master's, this time in history here at U of I. While taking on this workload and working as an Assistant Professor has been a huge workload, it's also helped me ground my work into creating practical applications for my digital scholarship work that can help students and researchers enhance their scholarship, such as [this workflow I've developed](https://aweymo-ui.github.io/python_obsidian/){:target="_blank" rel="noopener"} on using Python tools to pull annotations from reading materials and visualize these elements in the note taking application Obsidian.  

{% include gallery-figure.html img="py_ob_01.gif" alt="Obsidian graph view click through, adding and removing various elements." caption="Example of the graph output in Obsidian using the Python Annotation Extraction Tool mentioned above. The purple and blue nodes represent books for two different courses, the green nodes represent their tags and their proximity to one another represents their connections and contrasts." width="75%" %}

## Digital Scholarship Example

One example of a digital scholarship project I've worked on using a database that we will talk more about in a moment is using [Web of Science](https://www.webofscience.com/wos/woscc/basic-search){:target="_blank" rel="noopener"} to create Bibliometrics. This was prompted by my work creating a digital collection for the [U of I's Taylor Wilderness Research Station](https://www.lib.uidaho.edu/digital/taylor-archive/){:target="_blank" rel="noopener"}, a scientific refuge that students have been visiting in the remote Frank Church River of No Return Wilderness since the 1970s.

**Bibliometrics** are the use of statistical methods to analyze books, articles and other publications. The concept for this project was to see if there was some way to visualize all of the academic work that was produced by students and faculty members after conducting research at the station to convey a sense of the institution’s “research impact” over time. 

<div class="symbol-container">
    <p class="symbol">&#10042;</p>
</div>

{% include gallery-figure.html img="taylor.jpg" alt="Group of six standing in front of the Taylor Wilderness Research Station wearing clothes indicative of the late 1970s or early 1980s." caption="Arlow Lewis, the caretaker of Taylor Ranch for several years, far left with glasses. Kneeling on left is Jim Bennett, then a PhD student working on bighorn sheep. Carol Bennett is in the yellow top, courtesy U of I Special Collections (DSC_0360)" title="Arlow Lewis, the caretaker of Taylor Ranch for several years, far left with glasses. Kneeling on left is Jim Bennett, then a PhD student working on bighorn sheep. Carol Bennett is in the yellow top, courtesy U of I Special Collections (DSC_0360)" width="100%" %}

## Approach

This led me to consider some questions: 

* _What does it mean for a paper to be the direct product of a specific place?_ 

* _Does a work need to mention Taylor by name?_ 

* _Are we only looking at research produced by U of I?_ 

* _How long after the author visits Taylor is it still considered a product of that place?_ 

With this in mind, I decided to zoom out a bit and look at authors from U of I who were simply present in the archive, rather than specific titles.

<div class="symbol-container">
    <p class="symbol">&#10042;</p>
</div>

## Network Visualization

**After creating an author name equation** so I only needed to search for authors in seven batches of 100 names rather than a bleak 737 individual searches, this compiled Web of Science data was then exported in CSV format and then imported into [VOSviewer](https://www.vosviewer.com/), a Dutch, open-source network visualization platform with excellent documentation and an intuitive interface.

{% include gallery-figure.html img="biblio_01.gif" alt="Data visualization of multi-colored nodes against a black background labeled with the names of authors." caption="Visualization of citation impact over time of authors that contributed to work found in the Taylor Wilderness Research Station digital archive. Node size indicates the number of times the work has been cited, color and distance indicates groups formed by subject and keyword likeness and lines connecting nodes indicates shared citations."  title="Visualization of citation impact over time of authors that contributed to work found in the Taylor Wilderness Research Station digital archive. Node size indicates the number of times the work has been cited, color and distance indicates groups formed by subject and keyword likeness and lines connecting nodes indicates shared citations." width="100%" %}

I wanted to analyze: 

* [future citations](https://www.lib.uidaho.edu/digital/taylor-archive/citation.html) of specific documents 

* [co-authorship of papers](https://www.lib.uidaho.edu/digital/taylor-archive/coauthorship.html), and 

* [fields of interest](https://www.lib.uidaho.edu/digital/taylor-archive/keywords.html) over time. 

Once these three visualizations were completed, further customization was done adjusting node color to represent scientific discipline, size to represent the number of times the work has been cited, and arrangement according to when they were published. Selecting a node brings up a pane on the lower right hand corner of the screen which reveals more details on the title and, if available, creates a link to the research paper itself.

These visualizations were then embedded into our CollectionBuilder site using the [VOS-Viewer Online](https://github.com/neesjanvaneck/VOSviewer-Online) function. While these do take a short while to process the JSON data on loading, the bibliometrics add a colorful and interactive element that reduces a daunting amount of scholarly work into a single visualization.

While you may be doing more straight-forward searching using Web of Science and similar scientific databases in your work, pulling more detailed data from these databases could possibly add an interesting visual element to your final projects!