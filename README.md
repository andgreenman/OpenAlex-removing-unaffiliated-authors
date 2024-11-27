# OpenAlex-removing-unaffiliated-authors

Takes an OpenAlex search export and removes author data where a specified institution is not found in the affiliation string. Created to answer a question from a departmental research office about graphing intra-institutional collaboration in VOSviewer.

Due to restrictions of the data format, when an author multiple affiliations it cannot be known which affiliation belongs to which author, so all papers where the author list and affiliation list are not the same length are dropped. A more sophisticated version of this process could be to query the OpenAlex API to determine author affiliations for these papers.
