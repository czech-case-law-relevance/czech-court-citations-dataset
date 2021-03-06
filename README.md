# czech-court-citations-dataset

## Czech Court Citations Dataset
Dear visitor,

This is the Czech Court Citations dataset. This dataset contains citations of the court decisions extracted from texts of decisions of the three Czech apex courts - the Constitutional Court, the Supreme Court and the Supreme Administrative Court. 

The Czech Court Citations Dataset contains 21 files in .csv data format, 7 files for each court, divided according to the three courts. 

This dataset is properly described in: HARAŠTA, Jakub, Tereza NOVOTNÁ a Jaromír ŠAVELKA. Citation Data of Czech Apex Courts. : arXiv:2002.02224, 2020. 7 p. ISSN 2331-8422.

### File types

The Czech Court Citations Dataset contains three different types of files: files with *linked citations* (9), files with *unlinked citations* (9) and files with citations from the *'rest' category* (3).

Files with *linked citations* are files containing citations of the three Czech apex courts that were merged with Czech Court Decisions Corpus and therefore these citations contain all the metadata.

Files with *unlinked citations* are files containing citations of the three Czech apex courts that were not merged with Czech Court Decisions Corpus and therefore these citations do not contain all the metadata, only the docket number of the cited decision (reference).

Files in the category of the *'rest' citations* are files containing citations of any other public authority then the three Czech apex courts, therefore these citations do not contain all the metadata, only the docket number of the cited decision or document (reference).

### File names

In this dataset, abbreviations of the court names are used: 'ConCo' for the Constitutional Court, 'SupCo' for the Supreme Court and 'SupAdmCo' for the Supreme Administrative Court. Files are described according to the source judicial decision (from) and the target judicial decision (to) in the form of <source>-ref-<target>[-unlinked].csv or <source>-ref-rest.csv.
For example 'ConCo-ref-SupCo.csv' is a file containing all the extracted *linked citations* (references with metadata) of the Supreme Court decisions from the Constitutional Court decisions. 

Files with '-unlinked' extension contain *unlinked citations* (references without metadata).

The dataset contains 3 files in the category of the *'rest' citations*, these files contain citations of any other public authority then the three Czech apex courts (for example 'ConCo-ref-rest.csv').

### Data statistics

References sorted by categories, *unlinked*

| Court | Supreme Court | Supreme Adm. Court | Constitutional Court | Rest |
| ----- | ------------- | ------------------ | -------------------- | ---- |
| Supreme Court cites | 153 242 | 804 | 80 658 | 112 287 |
| Supreme Administrative Court cites | 1 342 | 90 217 | 14 756 | 20 709 |
| Constitutional Court cites | 8 486 | 2 877 | 137 308 | 45 689 |

References sorted by categories, *linked*

| Court | Supreme Court | Supreme Adm. Court | Constitutional Court |
| ----- | ------------- | ------------------ | -------------------- |
| Supreme Court cites | 140 355 | 658 | 76 003 |
| Supreme Administrative Court cites | 1 191 | 84 728 | 13 473 |
| Constitutional Court cites | 7 474 | 2 168 | 133 148 |

### Content of the files

Files contain unique rows, one citation per each row. Citations are accompanied by metadata:

**source_file**: the name of a source .txt file of the text of the decision, this file can be found in the Czech Court Decisions Corpus

**docket_number**: the identification of a source court decision

**date**: date of source decision in the form of YYYY-MM-DD

**court**: identification of court publishing the source decision in abbreviation

**reference**: the identification of a target court decision

**source_file2**: the name of a target text file of the text of the court decision, this file can be found in the Czech Court Decisions Corpus (only available in files with *linked citations*)

**date2**: date of target decision (only available in files with *linked citations*) in the form of YYYY-MM-DD

**court2**: identification of court publishing the target decision in abbreviation (only available in files with *linked citations*)

### Related corpora and publications

For extraction of the court citations the Annotated Corpus of Czech Case Law for Reference Recognition Tasks, containing 
350 manually annotated decisions for reference extraction of the Constitutional Court, the Supreme Court and the Supreme Administrative Court, was used as a training dataset for a machine learning algorithm. 

This corpus is properly described in: HARAŠTA, Jakub, Jaromír ŠAVELKA, František KASL, Adéla KOTKOVÁ, Pavel LOUTOCKÝ, Jakub MÍŠEK, Daniela PROCHÁZKOVÁ, Helena PULLMANNOVÁ, Petr SEMENIŠÍN, Tamara ŠEJNOVÁ, Nikola ŠIMKOVÁ, Michal VOSINEK, Lucie ZAVADILOVÁ a Jan ZIBNER, 2018. Annotated Corpus of Czech Case Law for Reference Recognition Tasks. In: Petr SOJKA, Aleš HORÁK, Ivan KOPEČEK a Karel PALA, ed. Text, Speech, and Dialogue. B.m.: Springer International Publishing, s. 239–250. Lecture Notes in Computer Science. ISBN 978-3-030-00794-2. 

This corpus is freely available at LINDAT/CLARIN repository: https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-2647.

For extraction of the court citations the dataset for Automatic Segmentation of Czech Court Decisions into Multi-Paragraph Parts, containing 350 manually annotated decisions for segmentation of the Constitutional Court, the Supreme Court and the Supreme Administrative Court, was used as a training dataset for a machine learning algorithm. 

This corpus is properly described in: HARAŠTA, Jakub, Jaromír ŠAVELKA, Frantisek KASL a Jakub MÍŠEK, 2019. Automatic Segmentation of Czech Court Decisions into Multi-Paragraph Parts. Jusletter IT [online]. (23-Mai-2019) [vid. 2019-09-26]. Dostupné z: http://jusletter-it.weblaw.ch/issues/2019/23-Mai-2019/automatic-segmentati_f1ab10b8b5.html__ONCE.

This corpus is freely available at LINDAT/CLARIN repository: https://lindat.mff.cuni.cz/repository/xmlui/handle/11372/LRT-2901.

For extraction of the court citations the Czech Court Decisions Corpus (CzCDC 1.0), containing 237 723 decisions of the Constitutional Court, the Supreme Court and the Supreme Administrative Court, was used as a source dataset for citations extraction using machine learning algorithm. 

This corpus is properly described in: NOVOTNÁ, Tereza a Jakub HARAŠTA. The Czech Court Decisions Corpus (CzCDC): Availability as the First Step. : arXiv:1910.09513, 2019. 8 s. ISSN 2331-8422. Dostupné z: https://arxiv.org/abs/1910.09513.

This corpus is freely available at LINDAT/CLARIN repository: https://lindat.mff.cuni.cz/repository/xmlui/handle/11372/LRT-3052.

### Licence terms and contacts
This dataset is available under Creative Commons Attribution 4.0 International (CC BY 4.0) licence (available at: https://creativecommons.org/licenses/by/4.0/).

In the case of any further questions, please contact Jakub Harašta or Tereza Novotná: jakub.harasta@law.muni.cz, tereza.novotna@mail.muni.cz.
