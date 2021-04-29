# ProQuestHistorical

https://nyu-dataservices.github.io/2021-love-datathon/ (for details on this project)

Context: ProQuest Historical Newspapers text-as-data collection consists of machine-readable full text and accompanying metadata and the individual article level for 26 historical newspapers. All told, there are some 55 million digitized pages, most covering the 1800s and 1900s. But newspapers have always included more than just news (think classified ads, obituaries, images). One feature of newspapers that has a long history are advertisements, and in fact the ProQuest company has labeled each advertisement in its collection so that we are able to analyse them separately.

Data Format: To access the data, download each of the two folders available on this Google Drive share folder https://drive.google.com/drive/folders/1G2Z6AtIEfvU6B3gXKg5SIXCPdbFj-N_0?usp=sharing. It can take up to 30 minutes to download the larger of the two folders, about 15 minutes for Drive to zip it up and another 15 minutes to download depending on your connection. You may want to consider starting with a sample consisting of one of the zipped files inside these parent directories. 

The data is represented as XML, with each newspaper article having its own separate XML file. Each article has a unique identifier number (RecordID) which serves as the filename; metadata and full text are combined together in the single XML file. A rough data dictionary for the XML is available, and an example file here. The collection is organized by newspaper, and each newspaper’s directory consists of several hundred zipped files. Each zip file contains 2-3,000 XML files zipped together. Retrieval of an individual XML file is dependent therefore on knowing newspaper name, zip filename, and article/XML RecordID number. If you wish, you can see the digital image version of any given XML record by visiting https://search.proquest.com/docview/<RECORD-ID> (you may need to SSO into ProQuest first at https://persistent.library.nyu.edu/arch/NYU02080 beforehand).


Challenge Goal: What if we were to hold a century’s worth of newspaper advertisements and their features in one dataset? What could we learn about the companies who have advertised and the products they have presented? What would we need to do to obtain that information from unmarked text produced from OCR software? The goal set by this challenge will be to:

- Retrieve the full text of advertisements for the full run of two newspapers, the New York Times (1851-1937) and the Atlanta Daily World (1932-2003; the oldest Black-owned newspaper in Atlanta) using two delimited pre-made lists of relevant XML RecordIDs (ADW list, NYT list). The New York Times list consists of 1.8 million advertisements, and the Atlanta Daily World list over 300,000 advertisements.
- Extract the full text from the XML, as well as relevant metadata.
- Formulate a response to handling OCR errors that will be found throughout the corpus.
- Apply natural language processing techniques to extract the following:
  - Product being advertised (e.g. “car,” “musical instrument,” “perfume”)
  - Name of company who is advertising (e.g. “Avon”)
  - Address or location of the company, if provided.
  - Date of advertisement, name of newspaper it appears in.
- Design a means of measuring accuracy/success of identifying these variables
- Gather together these data points in a user-friendly dataset
- Present a concluding analysis and visualization based on the data that gives at least one conclusion about a trend identified in the data.
- Deliver a code base that will enable the above process to be performed with other newspapers (reproducible).

Known Issues: Full text strings may contain HTML escape characters, and plenty of OCR errors, extraneous whitespace, missing text, and more.


