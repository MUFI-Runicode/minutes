# MUFI Runicode Subpanel Meeting

- Monday 6th November, 10am–6pm
- Økern, Kabelgata 34, Oslo; 1st floor, seminar room Vollebekk

## Attendance

### Present in person:
- Elisabeth Magin
- Marcus Smith
- Harald Tveiten

### Present via video link:
- Tarrin Wills

### Apologies:
- Alessia Bauer
- Marco Bianchi
- Odd Einar Haugen
- Alessandro Palumbo
- Alex Speed Kjeldsen
- Beeke Stegmann
- Kristel Zilmer
- Christiane Zimmerman

## Agenda

### 10:00

- Coffee & tea
- Welcome and Housekeeping

### Choice of chair and secretary for the meeting

- Chair: Elisabeth Magin
- Secretary: Marcus Smith

### 10:20

- Presentation of the chairs of the sub-panel – Marcus Smith and Elisabeth Magin
- Name of the runic sub-panel – "Runicode".
This is a sub-panel of the Medieval Unicode Font Initiative (MUFI). At the workshop on Unicode and runes in Uppsala in March 2023, it was agreed that further work was needed on the topic, and that this should, to begin with, be organised under the umbrella of MUFI. In a subsequent email exchange between workshop participants, it was agreed that Marcus Smith and Elisabeth Magin would act as co-chairs for this Runic sub-panel within MUFI. We have chosen the name "Runicode" for the runic sub-panel.
- Information: Website of the sub-panel: <https://mufi.info/q.php?p=mufi/runic> ; and on GitHub: <https://github.com/MUFI-Runicode>

#### Information/Discussion: Working practice of the sub-panel

- Transparency: minutes of meetings are published on the panel's GitHub pages (and website?); that includes this meeting.
- This particular meeting is "closed" (invitation-only) based on discussions and interest from the Uppsala meeting in March.
- The chairs propose that future meetings be open to all, but with the aim of participation from the principal centres of runological research to ensure proper representation and community buy-in.
- The question is raised as to whether there should be a specific use-case that ties in with Elisabeth's project, that would also benefit Tarrin's dictionary? Something we can start with that builds on current work.
- It is suggested that we start with smaller divisions, concrete use-cases, to solve: a solution for encoding medieval runes, a solution for the elder futhark, etc

### 10:45

#### Discussion: Goals, scope and remit for the sub-panel – proposed scope follows:
- Focused primarily on the *encoding* of runic characters
- Potentially also covering the *graphical description* of runic characters
- This will likely require a (comprehensive) *character inventory* and an (at least partial) *glyph inventory*, with a mapping between them
- *Not* focused on fonts. These must come later, as a display solution. However, our work should bear in mind the needs and typesetting practicalities of runologists.
	- Tarrin points out that people need fonts, if only to check their work. Some kind of font work has to be included, even if it's not the main focus.
	- Marco may be able to help here, in parallel with the spec that the sub-committee produces.
- The most realistic short-term goal is likely to produce a MUFI spec for the encoding of runic texts that builds upon the Unicode standard (e.g. restrict use to a subset of characters; assign PUA codepoints for unassigned characters, with a view to possible future standardisation; define variation selector sequences or similar for glyph variants; etc)
- Long-term there may be the possibility of taking this further as a proposal to Unicode to revise the existing standard (e.g. declare certain character pairs canonically equivalent/deprecated; define variation selector sequences; assign public codepoints for unassigned characters; etc) How realistic is this, and what would be required?
	- Tarrin: What's missing within MUFI is the evidence base for the characters: any Unicode proposal must include examples of use. And secondly, the distinction between different levels within MUFI is blurred: is it a glyph-variant, or a variant that carries phonological value?
	- Add to working practices: documentation of primary and secondary provenance information: where do these forms occur and how are they used?

#### Graphical encoding/description of runic forms

- Furthermore, in addition to specs focused on the Unicode Runic range, other methods of digitally representing the *forms* of runic characters may be explored (e.g. a spec for describing the vertical and diagonal branches of runic forms, orthogonal to the Runic range).
- Tarrin demonstrated the work he's been doing on describing the runic forms, using the stroke descriptor on the MUFI website: <https://mufi.info/q.php?p=mufi/runic/strokeselect> However there is still much that cannot be encoded using this tool. Alessia and Wilhelm in München have a system that is simpler than that of Kiel, that describes only the bistaves. This could be a promising avenue to pursue.
- An alternative is to not represent this in a font at all, but to generate graphical characters from the data.
	- Marcus: this should probably not be a font or a character encoding, but rather a protocol for describing runic forms (with an associated file format) with rendering support in SVG?
- Elisabeth demonstrated the need for a purely graphical encoding method using an example of an ambiguous inscription from the Bergen corpus which can be read in multiple ways: ⟨ᛐᛁᚢᛐᚱ⟩ There is a need to be able to describe these visual forms *before* any interpretation as to which runes they represent is made.
- Tarrin demonstrates marking up runic texts on images, to mark up the shape/graphical form; individual strokes can also be marked as being uncertain; this can then be mapped to the Unicode characters, to produce a list of the glyph forms that occur for each character.
- Tarrin continues that there is an even lower level of interpretation of what has been carved in to the object
- Tarrin lists the levels of interpretation:
	- identifying the object, 
	- describing the marks that occur on the object,
	- mapping that to an abstract rune,
	- mapping that to an actual character-variant,
	- mapping that something that has linguistic significance
- Tarrin warns that a limitation of the Kiel system is that it's a Windows proprietary application. Elisabeth adds that, furthermore, there is no plan for what will happen to the data once the project has concluded, which raises concerns of long-term sustainability.
- Tarrin adds that a development of a graphical encoding system (potentially along the lines of the stroke descriptor, and informed by the work of Alessia, Wilhelm, Alessandro *et.al.*) would be a solution not just for the digital recording of runic inscriptions, but also as a method of documenting provenance of forms within the sub-panels's broader work.
- Elisabeth remarks that the prevalence of transliteration in runology is problematic, because we're not immediately dealing with the runic characters themselves, and their forms.

#### Further discussion

- Marcus: this level of visual recording (that Tarrin has described) is absolutely necessary, for recording and interpretation, but the core issue here is the middle stages of interpretation, namely the mapping – and encoding – of runic characters and glyph-variants.
- Elisabeth: for *character encoding* we need to begin with a minimal subset of Unicode runic – including eliminating dotted runes in favour of combining dots – that can then be augmented with levels of glyph-variant nuance.
- Tarrin & Marcus: the goal should not be to make the character inventory as small a possible for smallness' sake, but rather to eliminate duplication.
- Elisabeth: there is a lot of education to be done within the community because runologists understand the distinction between graphemes and glyphs in the abstract but not in the context of Unicode or technology.

#### Consensus

- **Tarrin, Marcus, and Elisabeth are agreed: that the distinction between recording the graphical and the linguistic is meaningful and important, and that specifications for the recording of both is within the remit of the sub-panel.**

- A point is added to the mission statement to include accessibility applications.
- The place of fonts and typefaces in the scope of work was discussed, and the relevant line in the mission statement revised.

### 12:00
#### Break for lunch

### 13:00
#### Reconvene

Harald Tveiten is absent for the afternoon session.
We continue with discussion of the nature of the the guidelines for graphical/visual forms, and update the mission statement concerning mappings to characters accordingly.

We discuss the need to encode distinct characters *and* the specific graphical variation. We agree that the need is real, but that the solution is not clear and requires further work. Options include the use of variation selectors (which is unlikely to be approved by Unicode); the relegation of form-variants to fonts and display only (using font stylistic sets, perhaps standardised, but which exists "out of band" and is not searchable or interoperable); or the use of non-variation selector. Both approaches argue for a minimal character set which does not distinguish between e.g long-branch and short-twig forms, but upon which such variations can nonetheless be encoded. How this is to be done is the subject of future work.

There is a general consensus that for the *graphical* encoding, attempting to do this as a character encoding is probably not desirable both technically and from a usability perspective, and is unlikely to be accepted by Unicode should we wish to standardise. A bespoke encoding, with graphical software support for composition and display, is a better choice.

---

### Proposed work packages:

1. Review and evaluate current:
   - solutions,
   - technologies,
   - research (runic graphemics, Unicode/MUFI… etc)
2. Character and glyph inventory, including provenance.
3. Develop a solution
   - Are the two levels identified (graphical and linguistic) necessary and sufficient?
   - What potential solutions are available (runic "Meccano"/stroke descriptors; rich text/stylistic sets; variations selectors; in-band codes)?
4. Implementation – providing something workable (interface, fonts).

3 & 4 mostly to wait until 1 & 2 are complete.

**Action item:** 1. – review and evaluate current state of the art – to be carried out in collaboration between Marcus, Elisabeth, Tarrin and Marco. Tarrin to lead.
**Action item:** Elisabeth does 2. – character and glyph inventory – the medieval Bergen material as part of her Marie-Cure project
**Action item:** Elisabeth to ask Alessandro if he has something similar for the Swedish material (perhaps in his PhD database)
**Action item:** Tarrin to collate glyphs from runic fonts and look at connecting them to provenance data
**Action item:** Marcus to get in touch with Deborah Anderson at Unicode to check in with them on the existence of the sub-panel and the potential/process for changes to Unicode based on the direction we're thinking in (possibly to be a new work package, if response favourable). *(Edit: In conversations subsequent to the meeting, we agreed first that this item should be struck from the list, then that Tarrin will instead make contact with Deborah to establish communication with Unicode.)*

### Updated mission statement draft approved

We agree to an online check-in in two months (late jan/early feb 2024), and future meetings open meetings online or in-person per the working practices agenda item from the morning.

Meeting concluded 14:30.
