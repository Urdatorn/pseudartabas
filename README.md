# Pseudartabas

Note to self: use https://github.com/charmbracelet/vhs to create a nice gif here.

# Why?

In his comedy _Acharnenses_, Aristophanes has the Persian Ψευδαρτάβας speak before the Athenian assembly and say (Olson 2002):

> ἰαρταμανεξαρξαναπισσονασατρα.

There are two remarkable things about the line. First off, this pseudo-Persian gibberish[^1] can be scanned as a perfectly well-formed iambic trimeter. Indeed, not a trivial line, but one that forces us to get our prosody straight:

> ἰαρτᾰμᾱν|εξαρξᾰνᾱ|πισ(σονᾰ)σᾰ[τρα.

Prosodical notable features represented here are:
- six (!) dichrona with only one possible length for the scan to go through (five if we remove the acute that forces the ultima to be short),
- resolution of longum: (σονᾰ). Resolution sometimes indicates onomatopoeia or "sound" as opposed to speech, as the chirping birds in *Aves*. 
- homosyllabic *muta cum liquida* typical of comic dialogue: σά[τρ

Speaking of which, a nice warm-up exercise would be to explain why the outlier reading of manuscript R is non-metrical:

> ἰαρταμανεξαρξασαπισόναστρα.

The second and more noteworthy aspect is the vowel sequence that strongly outlines the metre even without caesurae (a strong argument against bothering with editorial wordbreaks):

> ιαᾰᾱ εαᾰᾱ ιοαᾰα

As a Panini and Pindala fanboy, these two sets of restraints (prosodical and phonological) got me thinking: Can we formalize what it is to be a well-formed Pseudartabasian string? How many such strings are there? Can we generate them?

For simplicity's sake, let's boil the restrictions down to the following:

A string `s` is Pseudartabasian iff
- P1: `s` is in *scriptio continua* iambic trimeter
- P2: `s` uses only valid Ancient Greek syllables, i.e. no triple consonants 'κκκα', string-end '-ζ' etc.
- P3: `s` has only homosyllabic *muta cum liquida*
- V1: the nine vowels making up the final three vowels of every metron of `s` are identical, length notwithstanding.
- V2: Chiasma: the first vowel of the first metron is identical to that of the last metron.


[^1]: Some editors divide it into ἰαρταμὰν ἐξάρξαν ἀπισσόνα σάτρα (Wilson, Hall & Geldard 1907) or ἰαρταμὰν ἐξάρξ' ἀναπισσόνα σάτρα (as the author of [this translation](https://www.perseus.tufts.edu/hopper/text?doc=Perseus%3Atext%3A1999.01.0240%3Acard%3D100)) to tease out pseudo-Greek syntax, which is another fun. A prosodist can only comment that since the trimeter tends to have either a penthemimeral or hepthemimeral caesura, and if not then at least a trithemimeral, the former would be unusual.
