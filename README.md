# conclusions

## 2. Codebook: Codes for sentences

If a code ends with `:iu`, this means it can have an "IU suffix".
The meaning of IU suffixes is explained in Section 4.
Actual `:iu` suffixes look for instance like this:
`:i1`, `:u2`, `:i2u1` or nothing (i.e., the suffix can also be missing). 
An IU suffix codifies subjective property counts of two properties
`i` and `u`, each with a default value of 0.

Our annotation checking script gathers the set of codes to check
for directly from the present file by looking for strings of the form
"code `something-or-other`".
Make sure all code declarations take this form and no other things do.


### 2.1 The abstracts archetype

TBD
The following will be defined in detail in subsequent sections.

The archetype: TBD

1. An abstract typically consists of three parts, in this order:
   _Introduction_, _Study Description_, and _Outlook_. 
   The _Outlook_ is sometimes missing.
2. Two turning points connect the three parts:
   - A statement of the study goals (`objective`) connects _Introduction_ to _Study Description_.
   - A generalizing statement ("take-home message", `conclusion`) 
     connects _Study Description_ to _Outlook_, but may be missing.
3. The _Introduction_ first introduces the topic area of the study and what is known (`background`)
   and then may or may not point out a gap in knowledge (`gap`) or 
   postulate a need for a certain research (`need`).
4. For an empirical article, the _Study Description_ begins with
   method description (`method`), followed by results description (`result`).
   Sometimes, this sequence occurs twice in a row, very rarely more.
5. For a design article, design description (`design`, see below) may precede the structure
   described in the previous point or may be interleaved with it.
6. Occasionally (but infrequently), _Study Description_ will end with a study summary (`summary`).
7. _Outlook_ talks about future research and states 
   what could now be done (`fposs`, for future possibilities),
   what should now be done (`fneed`),
   what the authors themselves intend to do (`fwork`), or
   what is still not known (`fgap`).
   Several of these may occur, in no particular order.

**The archetype guides the coding**: During coding, we will expect the next sentence
to be either part of the same stretch or the beginning of one
that the archetype describes as a possible successor.  
Only if the next sentence clearly defies any such interpretation will we consider
a different code for it.


### 2.2

### 2.? Suffixes (for conclusions) and others) - maybe make two sections out of this

### 2.7 Less common codes

- code `abc`:  
  description
  If position and phrasing allow it to be considered `background`, `objective`, or `conclusion`, use these.
- code `abc`:  
  description


### 2.9 Extra codes (TBD)

These codes can never occur alone, only in conjunction with one of the others.
They start with a dash to signal this and should be given last. 

- code `-hype`:  
  The sentence praises the work beyond what a factual statement might state.
  The code does not talk about the truth of the statement (which is often difficult
  to judge from the abstract alone), but about the tone in which
  the statement is made.
  Plain positive properties do not qualify ("This is helpful because..."),
  only emphasized ones do ("This is tremendously helpful because...").
  "very" does not count as hype.
  The most common places for this to occur are 
  `result`, `conclusion`, `fposs`, `need`, `method`.  
- code `-ignorediff`:  
  If the script flags a coding discrepancy that, after discussion, you and your fellow coder
  agree should be left in (because the two codings represent two different reasonable interpretations),
  add this code in one (and only one) of the codings to mark the discrepancy as resolved.
- code `-incredible`:  
  The sentence makes a statement that is very hard to believe, even after considering
  possible information that the reader of the abstract does not have.
  The most common places for this to occur are 
  `result`, `summary`, `conclusion`.  
- code `-problemstmt`:  
  The sentence formulates a statement of a problem to be solved that is more general
  than the study's `objective`. 
  Typically only (but then frequently) found in `need` statements.  
  (This code is for collecting data for a possible future research interest.
  We only want to find some examples, so not everybody needs to apply this code all the time.
  Feel free to overlook as many instances as needed to avoid slowing you down.)
- code `-timid`:  
  Applies to `conclusion` only. 
  To be used when the generalization made is overly vague or small.

In contrast to the sentence classifications, which are intended to be objective
(hence the use of two coders and the use of `-ignorediff` where objectivity reaches its limits),
the codes `-hype`, `-incredible`, and `-timid` are optional additional attributes
that are considered subjective. 
Apply them with your own good judgment and keep in mind that
"we are gentle in detecting negative aspects".


### 2.10 Codes for special circumstances (maybe even keep as is)

- code `cruft`:  
  This sentence is not part of the abstract.
  It is garbage that should have been removed during the preparation of the abstract files.
- code `X`:  
  Undecided class. The sentence needs to be revisited and classified;
  consider using `fgrep {{X}}` to find these cases.
  Use `X` only rarely and only when you cannot _yet_ make up your mind.
  Such a code will likely result in a discrepancy with your fellow coder.
  It must always eventually be replaced with a proper code.
