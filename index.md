The intention of *matterhorn.tools* is to unite all information about Matterhorn METS and the Matterhorn RDF Data Model at one central location. The two models for archival metadata have been co-developed by Alain Dubois ([Valais State Archives](https://www.vs.ch/fr/web/culture/aev)) and Tobias Wildi ([docuteam,](https://www.docuteam.ch) now [Fachhochschule Graubünden, Swiss Institute for Information Science](https://www.fhgr.ch/sii)). The goal of the models is to improve contextualization in archival description by implementing the archival standards of the International Council on Archives (ICA) and the OAIS information model within the same metadata model. The Matterhorn data models are solely based on already existing norms and standards; we seek to improve and recombine existing work and don’t want to reinvent the wheel.

The work for Matterhorn METS started in 2008 with the goal to substantiate and implement the OAIS information model and the ICA-standards for archival metadata in one XML-based model. This model should be generic enough that it could be used not only in archival contexts but also in libraries, museums and for archiving research data. The result of this work was a specification (in german only) and a formal METS-Profile which was registered at the Library of Congress in 2012. The model could be presented at numerous conferences in Europe and is currently used by about 50 institutions in Switzerland, Germany, Austria and France.

The design work for the Matterhorn RDF Data Model started in 2015 when it became clear that an XML-based standard is not sufficient to model the relations between the different ICA-standards ISAD(G), ISAAR(CPF) and ISDF. We saw the relations between the content-, agent- and business process-description as the crucial part for improving the contextualization of archival description. Furthermore an XML-notation for ISDF was completely lacking and we saw no group in the international archival community working on this topic. This lead us to the conclusion that we had to move on to a model that was based on semantic technologies. As it was the case with Matterhorn METS we decided again to not develop our own standard or ontology, but to rely on classes and properties of already existing, widely used and well maintained ontologies. We followed closely the work of the Expert Group on Archival Description (EGAD) and Tobias Wildi became member of the EGAD in 2019. He helps to develop the [„Records in Context Ontology“, or „RiC-O“.](https://github.com/ICA-EGAD/RiC-O)

Matterhorn RDF covers not only the description of archival material, but also technical and administrative metadata that is needed to preserve material over the long run. Thus Matterhorn RDF is a combination of [RiC-O,](https://github.com/ICA-EGAD/RiC-O) the [PREMIS 3 ontology](http://www.loc.gov/standards/premis/ontology/) and the [Ebucore-ontolgoy.](https://www.ebu.ch/metadata/ontologies/ebucore/)

A data model has to be formalized in one way or another. In 2017 the W3C published their recommendations about the „Shapes Constraint Language (SHACL)“. SHACL is a language „for validating RDF graphs against a set of conditions“. These conditions are expressed in so called „Shapes“ and if a graph fits into a shape it’s a valid statement. We decided to use SHACL Shapes for the formalization of Matterhorn RDF since such shapes are at the same time human- and machine readable. The formulation of the SHACL Shapes for all classes and properties of Matterhorn RDF is the goal of our current research.

## Contact:
[Alain Dubois](mailto:Alain.DUBOIS@admin.vs.ch) (State Archive of Valais)  
[Tobias Wildi](mailto:tobias.wildi@fhgr.ch) (Fachhochschule Graubünden / University of Applied Sciences of the Grisons)  

## Matterhorn METS
Matterhorn METS is a METS-Profile on which we started to work in 2008 and registered in 2012 at the Library of Congress. It combines METS, PREMIS and EAD:
- [Specification of Matterhorn METS (German)](https://wiki.docuteam.ch/lib/exe/fetch.php?media=oais:spezifikation_matterhorn-mets_20160830_wi.pdf)
- [Matterhorn METS-Profil, registered in 2012 at the Libray of Congress](https://www.loc.gov/standards/mets/news112912.html)


### Presentations and papers of Matterhorn METS:
- [Tobias Wildi. PREMIS in METS: Die beiden Datenmodelle Matterhorn METS und Archivematica.  Nestor-Praktikertag 2018: Metadaten für die digitale Langzeitarchivierung und der Metadatenstandard PREMIS. Frankfurt am Main, 6. Juni 2018.](https://www.slideshare.net/TobiasWildi/premis-in-mets-die-beiden-datenmodelle-matterhorn-mets-und-archivematica)
- [Alain Dubois. Quelle qualité pour les archives électroniques ? Réflexions et retour d’expérience autour du processus décisionnel du Conseil d’Etat valaisan. In: Ressi, N°14 décembre 2013.](http://www.ressi.ch/num14/article_94)
- [Alain Dubois, Tobias Wildi. Vers une intégration complète des standards de description du Conseil international des Archives ?Réflexions autour du processus décisionnel du Conseil d’Etat valaisan. Forum des archivistes genevois – 17 juin 2013.](https://www.slideshare.net/TobiasWildi/presentation-geneve-20130617)
- [Alain Dubois, Tobias Wildi. Contextualisation 2.0. Le Matterhorn METS Profile : un nouveau modèle d&#8217;organisation des données et métadonnées ? Présentation au &#8222;Forum des archivistes&#8220; 22.3.2013 à Angers.](https://de.slideshare.net/TobiasWildi/contextualisation-20)

## Matterhorn RDF
- An example of the same information package encoded in RDF and a METS can be found in the [examples-section of RiC-O](https://github.com/ICA-EGAD/RiC-O/tree/master/examples/examples_v0-2/Matterhorn-Switzerland)
- When RiC-O didn't exist yet, we used a combination of existing ontologies to model the descriptive metadata. See our first, but now [obsolete Specification of Matterhorn RDF.](https://wiki.docuteam.ch/doku.php?id=docuteam:matterhornrdf)

### Paper:
- [Alain Dubois, Tobias Wildi. The Matterhorn RDF Data Model. Formalizing Archival Metadata With SHACL. Paper presented at the 16th International Conference on Digital Preservation iPRES 2019, Amsterdam, The Netherlands.](https://github.com/wildit/matterhorn/blob/main/documents/iPRES2019-Wildi-Dubois-Matterhorn%20RDF.pdf)

## Presentations
- [Alain Dubois, Tobias Wildi. Matterhorn RDF: Contextualize archival records with RiC and Premis. Referat im Rahmen der ICA International Council on Archives Virtual Conference 2021, 26.10.2021.](https://zenodo.org/record/5804872)
- Alain Dubois, Tobias Wildi. The Matterhorn RDF Data Model. Formalizing Archival Metadata With SHACL. Presentation at iPres 2019, Amsterdam 19.7.2019.
- Alain Dubois, Tobias Wildi. Le Matterhorn RDF Data Model: Description archivistique et Linked Open Data. Vers quelle convergence? Présentation au &#8222;Forum des Archivistes; 5 avril 2019, Saint-Etienne.
- [Alain Dubois, Andreas Nef. The Matterhorn RDF Data Model: Implemeting OAIS and RiC in the context of semantic technologies. ICA annual conference, 28.11.2017, Mexico.](http://www.alaarchivos.org/wp-content/uploads/2017/12/3.-Alain-Dubois-Andreas-Nef.pdf)
- [Alain Dubois, Tobias Wildi. Le Matterhorn RDF Data Model: Implémentation des modèles d’information OAIS et RiC dans le cadre des technologies sémantiques. Présentation au forum des archivistes genevois (11.9.2017).](https://de.slideshare.net/forumdesarchivistes/le-matterhorn-rdf-data-model-80360789)






