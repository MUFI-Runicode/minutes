# MUFI Runicode Subpanel Meeting

- Monday 6th November, 10am–6pm
- Økern, Kabelgata 34, Oslo; 1st floor, seminar room Vollebekk

## Presesnt

In person:
- Elisabeth Magin
- Marcus Smith
- Harald Tveiten

Via Link:
- Tarrin Wills

## Agenda

### 10:00

- Coffee & tea
- Welcome and Housekeeping

## Choice of chair and secretary for the meeting

- Chair: Elisabeth
- Secretary: Marcus

### 10:20

- Presentation of the chairs of the sub-panel – Marcus Smith and Elisabeth Magin
- Name of the runic sub-panel – "Runicode". This is a sub-panel of MUFI **(take from updated info)**
- Information: Website of the sub-panel – <https://mufi.info/q.php?p=mufi/runic> ; and on GitHub <https://github.com/MUFI-Runicode>
- Information/Discussion: Working practice of the sub-panel
	- Transparency: minutes of meetings are published on the panel's GitHub pages (and website?); that includes this meeting.
	- This particular meeting is "closed" (invitation-only) based on discussions and interest from the Uppsala meeting in March.
	- The chairs propose that future meetings be open to all, but with the aim of participation from the principal centres of runological research to ensure proper representation and community buy-in.
	**(again supplement from updated info)**
	- Should there be a specific use-case that ties in with Elisabeth's project? That would also benefit Tarrin's dictionary?
	- It is suggested that we start with smaller divisions, concrete use-cases, to solve: a solution for encoding medieval runes, a solution for the elder furthark, etc
	- Tarrin points out that this should not 
	


### 10:45

- Discussion: Goals, scope and remit for the sub-panel – proposed scope follows:
	- Focused primarily on the *encoding* of runic characters
	- Potentially also covering the *graphical description* of runic characters
	- This will likely require a (comprehensive) *character inventory* and an (at least partial) *glyph inventory*, with a mapping between them
	- *Not* focused on fonts. These must come later, as a display solution. However, our work should bear in mind the needs and typesetting practicalities of runologists.
	  - Tarrin: people need fonts, if only to check their work. Some kind of font work has to be included.
	  - Marco may be able to help here, in parallel with the spec we produce.
	- The most realistic short-term goal is likely to produce a MUFI spec for the encoding of runic texts that builds upon the Unicode standard (e.g. restrict use to a subset of characters; assign PUA codepoints for unassigned characters, with a view to possible future standardisation; define variation selector sequences or similar for glyph variants; etc)
	- Long-term there may be the possibility of taking this further as a proposal to Unicode to revise the existing standard (e.g. declare certain character pairs canonically equivalent/deprecated; define variation selector sequences; assign public codepoints for unassigned characters; etc) How realistic is this, and what would be required?
		- Tarrin: What's missing within MUFI is the evidence base for the characters - any Unicode proposal must include examples of use. And secondly, the distinction between different levels within MUFI is blurred: is it a glyph-variant, or a variant that carries phonlogical value?
		- Add to working practices: documentation of primary and secondary provenance information (where do these forms occur and how are they used?)
	- Furthermore, in addition to specs focused on the Unicode Runic range, other methods of digitally representing the *forms* of runic characters may be explored (e.g. a spec for describing the vertical branches of runic forms, orthogonal to the Runic range)
	  - Tarrin demonstrated the work he's been doing on describing the runic forms, using the stroke descriptor on the MUFI website **(link here)** There is still much that cannot be encoded. Christiane and ??? have a system that is simpler than that of Kiel, that describes only the bistaves.
	  - An alternative is to not represent this in a font at all, but to generate characters from the data
	  - Marcus: this need not be a font or a character encoding, but rather a protocol for describing runic forms (with an associated file format) with rendering support in SVG?
	  - Elisabeth demonstrates the need for a purely graphical encoding method **(photos)**
	  - Tarrin demonstrates marking up runic texts on images, to mark up the shape/graphical form; individual strokes can also be marked as being uncertain; this can then be mapped to the Unicode characters, to produce a list of the glyph forms that occur for each character;
	  - Tarrin continues that there is an even lower level of interpretation of what has been carved in to the object
	  - Tarrin: levels of interpretation: identifying the object, describing the marks that occur on the object, mapping that to an abstract rune; mapping that to an actual character-variant; mapping that something that has linguistic significance
	  - Tarrin: the Kiel system at least is that it's a Windows proprietary application; Elisabeth: and there is no plan for what will happen with the data post-project
	  - Tarrin: this a solution not just for the digital recording of runic inscriptions, but also as a method of documenting provenance of forms within the sub-panels's work.
	  - Elisabeth: the prevalence of transliteration in runology is problematic, because we're not dealing with the runic characters themselves, and their forms.
	  - Marcus: This level of visual recording (that Tarrin has described) is absolutely necessary, for recording and interpretation, but the core issue here is the middle stages of t interpretation, namely the mapping – and encoding – of runic characters and glyph-variants
	  - Elisabeth: for character encoding we need to begin with a minimal subset of Unicode runic – including elminating dotted runes in favour of combining dots – that can then be augmented with levels of glyph-variant nuance
	  - Tarrin & Marcus: the goal should not be to make the character inventory as small a possible for smallness' sake, but rather to eliminate duplication.
	  - Elisabeth: there is a lot of education to be done within the community because runologists understand the distinction between graphemes and glyphs in the abstract but not in the context of Unicode or technology.

- **Agreed: that the distinction between recording the graphical and the linguistic is meaningful and important, and that specifications for the recording of both is within the remit of the sub-panel.**

- Point added to mission statement to include accesibility applications
- The place of fonts and typefaces in the scope of work was discussed, and the relevant line revised.
- 

### 12:00

Lunch provided by the subpanel

### 13:00

Harald has left us for the afternoon session.
We continue with discussion of the nature of the the guidelines for graphical/visual forms, and update the mission statement concering mappings to characters accordingly.

We discussed the need to encode distinct characters *and* the specifical graphical variation. We agree that the need is real, but that the solution is not clear and requires further work. Options include the use of variation selectors (which is unlikely to be approved by Unicode); the relegation of form-variants to fonts and display only (using font stylistic sets, perhaps standardised, but which exists "out of band" and is not searchable or interoperable); or the use of non-variation selector. Both approaches argue for a minimal character set which does not distinguish between e.g long-branch and short-twig forms, but upon which such variations can nonetheless be encoded. How this is to be done is the subject of future work.


### Proposed work packages:

1. Review and evaluate current:
   - solutions,
   - technologies,
   - research (runic graphemics, Unicode/MUFI… etc)
2. Character and glyph invetory.
3. Develop a solution
   - Are the two levels identified (graphical and linguistic) necessary and sufficient?
   - What potential solutions are available (runic meccano, rich text/stylistic sets, varations selectors, in-band codes)?
4. Implementation – providing something workable (interface, fonts).

**Action item:** 1. – review and evalutate current state of the art – to be carried out in collaboration between Marcus, Elisabeth, Tarrin and Marco. Tarrin to lead.
**Action item:** Elisabeth does 2. – character and glyph inventory – the medieval Bergen material as part of her Marie-Cure project
**Action item:** Elisabeth to ask Alessandro if he has something similar for the Swedish material (perhaps in his PhD database)
**Action item:** Tarrin to collate glyphs from runic fonts and look at connecting them to provenance data
**Action item:** Marcus to get in touch with Deborah ??? at Unicode to check in with them on the existence of the sub-panel and the potential/process for changes to Unciode based on the direction we're thinking in (possibly to be a new work package, if response favourable).

3 and 4 mostly to wait until 1 & 2 are complete.


### Updated mission statement draft approved

**Per agrement this morning, online check-in in two months (late jan/early feb 2024) 

Meeting concluded 14:30.
