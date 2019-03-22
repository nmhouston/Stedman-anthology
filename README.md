# Stedman Anthology Dataset
A dataset of the poems published in Edmund Clarence Stedman's *A Victorian Anthology 1837-1895* (Houghton, Mifflin and Co., 1895). 

## Historical and Critical Context
The American critic Edmund Clarence Stedman was the first to use the term “Victorian” to describe British literature after 1837, in a series of essays in *Scribner's Monthly* that were later published in his 1875 book *Victorian Poets*. In 1895, Stedman edited an anthology of British poetry entitled *A Victorian Anthology 1837-1895*. 

## Data Source and Preparation
The digital source for the data files released here is the Bartleby.com edition (https://www.bartleby.com/246/) of Stedman's anthology. The four poems published as epigraphs to each section are omitted from this dataset. This dataset contains 1,284 poem files.
Data preparation included:
+ removing all HTML tags
+ saving each poem as a UTF-8 encoded plain text file 
+ splitting each of the sonnets Stedman includes from Elizabeth Barrett Browning's sequence *Sonnets from the Portuguese* into a separate file
+ removing titles and epigraphs  
+ removing line numbers 
+ removing roman numerals (used to divide poem sections) 
+ assigning author, section, and poem codes to facilitate analysis

Several digitized copies of Stedman's anthology are available. A Google-digitized copy of the 1895 edition owned by Harvard library was consulted throughout the project. (https://archive.org/details/avictorianantho00unkngoog) 

## Metadata Files

### Arrangement and Classification

Stedman's anthology is divided into four main parts. The first three are organized by historical chronology: “Early Years of the Reign,” “The Victorian Epoch,” and “Close of the Era.” The fourth category, “Colonial Poets,” contains works by poets from Australia and Canada. The first two divisions are further subdivided by genre, style, or artistic school. The section_titles.csv lists the divisions and subcategories and their assigned codes.

### Poet names

Stedman's anthology includes works by 342 named poets plus one poem credited as  Anonymous. There are 73 female and 269 male poets in this anthology, plus 1 of unknown gender (Anonymous). The author_list.csv lists the names and gender of each poet plus the assigned author code.

### Poem metadata

The Stedman_data.csv lists all the poems in the dataset and its assigned poem code. This table also lists their associated author and section codes, which can be cross-referenced with the other csv files for that additional information. 

## File naming 

The poem files in the dataset have been named so as to facilitate analysis. Each file name expresses the gender of the poet, the major division of the anthology in which the poem is published, the poet code, and the unique text code of the poem. 

The filename *F2_p11_t0700.txt* thus indicates that it is by a female poet; published in division 2 of the anthology; by poet code 11; and is text number 700. Thus 

Cross-referencing the metadata files described above indicates that this file is published indivision 2 "The Victorian Epoch," is written by the female poet Christina Rossetti, and that the poem is titled "Good-By."

## Accessing the files (if you're not familiar with Github)
This repository contains two folders, poems and metadata. From the main screen you can click the green download button to download the entire repository as a zip file. 

## About
This dataset was prepared by Natalie M. Houston in 2017-18. If you spot errors or have questions, feel free to contact me or open an issue in the repo. 
