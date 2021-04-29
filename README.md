# ProQuestHistorical

We are given a large xml file containing ads from the New York Times and Atlantic Daily World.

- Each Article or Section of a newspaper corresponds to a single XML file.
- The XML will contain full-text and metadata of the sub-section which can be an opinion, article, advertisement.
- Record Id is a unique identifier for each XML file. Basis for each file name.
- Each newspaper has a 200-300 zip file each containing 2000-3000 XML file corresponding to each article in a particular newspaper.
- Dictionaries of which Record IDs are advertisements will be provided to us.
- Find a way to efficiently retrieve them.
- https://search.proquest.com/document/
- Apply NLP to obtain full-text day of: Product being advertised, name of the company who is advertising, address/location of the company, date of advertisement, newspaper name the advertisement appears in, etc.
- Find means of measuring the accuracy/success of identifying the variables.
- Reproducible: Our code can be applied to other newspapers as well.
- Produce a User-Friendly dataset of our extracted information.
