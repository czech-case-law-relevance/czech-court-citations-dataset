# czech-court-citations-dataset
Dear visitor, please note that this page is still under construction. Thank you.



Czech Court Citations Dataset

This is the Czech Court Citations dataset. This dataset contains citations of the court decisions extracted from texts of decisions of the three Czech apex courts - the Constitutional Court, the Supreme Court and the Supreme Administrative Court. 

For extraction of the court citations the Annotated Corpus of Czech Case Law for Reference Recognition Tasks, containing 
350 manually annotated decisions for reference extraction of the Constitutional Court, the Supreme Court and the Supreme Administrative Court, was used as a training dataset for a machine learning algorithm. 
This corpus is properly described in: HARAŠTA, Jakub, Jaromír ŠAVELKA, František KASL, Adéla KOTKOVÁ, Pavel LOUTOCKÝ, Jakub MÍŠEK, Daniela PROCHÁZKOVÁ, Helena PULLMANNOVÁ, Petr SEMENIŠÍN, Tamara ŠEJNOVÁ, Nikola ŠIMKOVÁ, Michal VOSINEK, Lucie ZAVADILOVÁ a Jan ZIBNER, 2018. Annotated Corpus of Czech Case Law for Reference Recognition Tasks. In: Petr SOJKA, Aleš HORÁK, Ivan KOPEČEK a Karel PALA, ed. Text, Speech, and Dialogue. B.m.: Springer International Publishing, s. 239–250. Lecture Notes in Computer Science. ISBN 978-3-030-00794-2. 

This corpus is freely available at LINDAT/CLARIN repository: https://lindat.mff.cuni.cz/repository/xmlui/handle/11234/1-2647.

For extraction of the court citations the dataset for Automatic Segmentation of Czech Court Decisions into Multi-Paragraph Parts, containing 
350 manually annotated decisions for segmentation of the Constitutional Court, the Supreme Court and the Supreme Administrative Court, was used as a training dataset for a machine learning algorithm. 
This corpus is properly described in: HARAŠTA, Jakub, Jaromír ŠAVELKA, Frantisek KASL a Jakub MÍŠEK, 2019. Automatic Segmentation of Czech Court Decisions into Multi-Paragraph Parts. Jusletter IT [online]. (23-Mai-2019) [vid. 2019-09-26]. Dostupné z: http://jusletter-it.weblaw.ch/issues/2019/23-Mai-2019/automatic-segmentati_f1ab10b8b5.html__ONCE.

This corpus is freely available at LINDAT/CLARIN repository: https://lindat.mff.cuni.cz/repository/xmlui/handle/11372/LRT-2901.

For extraction of the court citations the Czech Court Decisions Corpus (CzCDC 1.0), containing 
237 723 decisions of the Constitutional Court, the Supreme Court and the Supreme Administrative Court, was used as a source dataset for citations extraction using machine learning algorithm. 
This corpus is properly described in: NOVOTNÁ, Tereza a Jakub HARAŠTA. The Czech Court Decisions Corpus (CzCDC): Availability as the First Step. : arXiv:1910.09513, 2019. 8 s. ISSN 2331-8422. Dostupné z: https://arxiv.org/abs/1910.09513.

This corpus is freely available at LINDAT/CLARIN repository: https://lindat.mff.cuni.cz/repository/xmlui/handle/11372/LRT-3052.

The Czech Court Citations Dataset contains 9 files in .csv data format, 3 files for each court, divided according to the three courts. In this dataset, abbreviations of the court names are used: 'ConCo' for the Constitutional Court, 'SupCo' for the Supreme Court and 'SupAdmCo' for the Supreme Administrative Court. Files are described according to the source judicial decision (from) and the goal judicial decision (to).
For example 'ConCo-ref-SupCo' is a file containing all the extracted citations of the Supreme Court decisions from the Constitutional Court decisions.

Files contain unique rows, one citation for each row. Citations are accompanied by metadata:

source_file: the name of a source text file of the text of the decision, this file can be found in the Czech Court Decisions Corpus

docket_number: the identification of a source court decision

date: date of source decision

court: identification of court publishing the source decision in abbreviation

reference: the identification of a goal court decision

source_file2: the name of a goal text file of the text of the court decision, this file can be found in the Czech Court Decisions Corpus
