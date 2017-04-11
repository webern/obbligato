# *Obbligato*
### A file format for simplified music notation exchange.

#### Purpose

A great number of text-based languages for encoding music notation have been created.  MusicXML is the most ubiquitous.  Some of the others are Guido, MuseData, Humdrum, MEI, and the forthcoming MNX.  Many of these are specified with a great deal of flexibility.  The flexibility afforded by these languages produces, as a side-effect, a large implementation surface.

To describe the choices faced in creating a music notation encoding format, the MNX team described a triangle, similar to the [project management triangle](https://en.wikipedia.org/wiki/Project_management_triangle).  The MNX team substituted "semantics, interoperability, generality" for “fast, cheap, good” and suggested that the community could pick two, but not three of these.

*Obbligato* would like to propose a triangle slightly altered from that of MNX, “expressiveness/generality, interoperability, ease-of-implementation”.

              interoperability
                     ^
                    / \
                   /   \
                  /     \
                  -------
    expressiveness       ease-of-implementation     
    
*Obbligato* strives to provide interoperability and ease-of-implementation.  Where necessary, *Obbligato* sacrifices expressiveness and generality.  It takes some inspiration from the Guido's notion of "adequacy".  But in this case adequate means that *Obbligato* strives to describe the semantics and visual appearance of common western music notation.

As to what constitutes common western music notation.  A great deal could be written about this and much debate would ensue.  For the time being, the notion of adequacy will extend to the definition of common western music notation.  Like Justice Potter Stewart, *Obbligato* will say, "I know it when I see it".  To some extent the decision about what is and is not common western music notation will depend upon how contorted the specification must become to properly support it.  For example, adding a glyph is simple, and would likely be included.  Specifying chords whose note members are of differing durations would cause undue contortion of the spec only to support rare cases and thus will be excluded.

Here are the top priorities of *Obbligato*
* Clarity of Music Notation Semantics
* Specificity of the Visual Representation of Notated Music
* Syntactic Specificity
* Clarity of Document Validity
* Simplicity of Parsing
* Extremely Accurate Exchange of Music Notation between Applications

Here are the things that *Obbligato* is willing to sacrifice:
* MIDI Information
* Audio and Mixing Information (e.g. Pan, Volume)
* Extensibility
* Human Readibility