# Conclusions Master Thesis - CodeBook.alpha

&#x1F4CC; - reminder for smaller tasks. May mean that an information is still missing/unclear or that I need to look something up

&#x1F6A7; - in construction, this is a code/part I've started to work on but that is not quite done yet

&#x2753; - somthing that's just barely there, very unclear and still needs a lot of work


## 2. Codebook: Codes for sentences


### 2.1 The conclusion-sections commmon flow

Conclusion-sections are similar to the abstracts archetype, the sequence of stretches is similar, but the occurence of stretches is different. 

The following will be defined in detail in subsequent sections.

The common flow: 

1. A conclusion may consist of three parts, in this order:
   _Introduction_, _Study Description_, and _Outlook_. 
   _Introduction_ and _Study Description_ are often missing, they are roughly seen in every 5th article.
   It is rather rare to have all three parts in one conclusion.
2. Two turning points connect the three parts:
   - A statement of the study goals (`objective`) connects _Introduction_ to _Study Description_.
     Sometimes the `objective` is described in several connected sentences.
   - A generalizing statement ("take-home message", `conclusion`) 
     connects _Study Description_ to _Outlook_.
     There are almost never `conclusion` sentences that follow each other.
     In very seldom cases there is no `conclusion`.
3. The _Introduction_ first introduces the topic area of the study and what is known (`background`)
   and then seldomly points out a gap in knowledge (`gap`) or 
   postulates a need for a certain research (`need`).
4. For an empirical article (which are the only ones we are looking at), the _Study Description_ often begins with
   method description (`method`), followed by results description (`result`).
4.5 `result` is sometimes seen out of _Study Description_. 
   Sometimes `result` slides into `conclusion` and makes the turning point longer. 
   A `result` in this position typically explains a conclusion.
   Sometimes `result` is found in _Outlook_ and most of the times this means the authors intended a "take-home-message",
   but did not take the  last step to generalize and make it a `conclusion`.
5. _Outlook_ talks about future research and states 
   what could now be done (`fposs`, for future possibilities),
   what should now be done (`fneed`),
   what will most definetly happen (`fwill`)
   what the authors themselves intend to do (`fwork`), or
   what is still not known (`fgap`).
   Additionally there can be `conclusion`s found in between future research. CHECK (sometimes its hard to differentiate betw conclusion and fneed)
   Several of these may occur, in no particular order. 
   This stretch always ends the conclusions. There is only one exception when _Outlook_ does not end the conclusion:
   If the conclusion has multiple subsections then _Outlook_ may be found in a seperate subsection.
   _Outlook

**exceptions to the flow**: List and `artifact`. 
- Lists are often introduced as "contributions". Typically these are a mix of outcomes(`result`,`conclusion` and _Outlook_ codes) with no certain structure. <FloMorZha und BalRal>
- &#x1F4CC; `artifact` are XXXX . `artifact` typically occur after _Introduction_ and _Study Description_.
  The content of an `artifact` is often only described in a superficial way (meaning no actual learnings are explained, `teaser`).
  If an `artifact` is described the above flow is no longer working until the description is over.

**The flow guides the coding**: During coding, we will expect the next sentence
to be either part of the same stretch or the beginning of one
that the archetype describes as a possible successor.  
Only if the next sentence clearly defies any such interpretation will we consider
a different code for it.


### 2.2 Core codes for the turning points

The turning points are the most informative sentences
in an abstract: 
The first describes what the study is about, 
the second describes what it found.

From _Introduction_ to _Study Description_:
- code `objective`:  
  one or more of this work's 
  top-level research goals,
  specific top-level research interests, or
  top-level research questions.  
  Objectives sentences often contain material that is ambiguous as goal-or-method
  or as goal-or-design. In those cases, assign two codes only if there is no 
  method (or design) information elsewhere in the abstract.
  If the method (or design) information is too specific and concrete to be a goal,
  assign two codes in any case.

From _Study Description_ to _Outlook_:
- code `conclusion`:  
  A take-home message that is less specific than one or more results.
  Usually a generalization from the results, sometimes a non-obvious existence proof statement(&#x1F4CC;seen from after/before the study).
  A conclusion is often written in present tense, never in past tense. (&#x1F4CC;CHECK AGAIN)
- `the suffixes for `conclusion:g/e:(p/r):0/1/1.5/2/3:` describe:
   - what kind of `conclusion` it is: either a generalization (`:g`) or a an existence proof (`:e`).
   - whom the `conclusion` is for. This Code is only used if the information of the sentence is
     clearly meant for only researchers `:r` or practitioners `:p`.
   - how confident the authors express their `conclusion`. &#x1F6A7;
     `:1` stands for the lowest confidence. This suffix is used when there are words("could", "can", "maybe", ...) that make an obvious effort to make the conclusion easy to agree. 
      `:2` stands for a rather neutral `conclusion`, which does not try to make it more agreeable or hype it up. The conclusion is firm.
      `:1.5` stands in between `:1` and `:2`. It catches all conclusions who are not perfetly firm, but also don't make an obvious effort te be agrereable, but a rather small one.
       `:3` shows the highest confidence and should be used, if authors make their conclusions seem overly true. (not sure abt this one...)
       &#x2753;is this the right place for this? `:0` is actually never used on `conclusions`....but on `results` that could've been `conclusions`
  
   
### 2.3 Core codes for _Introduction_

- &#x1F6A7; code `background`:  
  Information about the larger topic area of the work, the state-of-the-art,
  related work, what is known, definitions. This occurs sometimes, if it does it often occurs in blocks with several sentences only about `background`.
   <ich hab related work bisher eigen codiert, brauche ich das so oder nicht?>
- code `gap`:  
  A statement of what is not yet known or 
  what is so far difficult to achieve in research or in practice
  which directly leads over to the topic of the present work (the `objective`).
- code `need`:  
  A postulate about what research needs to be performed
  which directly leads over to the topic of the present work (the `objective`). Occurs almost never.
      

### 2.4 Core codes for _Study Description_

- code `method`:  
  information about the approach or setup of an empirical (&#x1F4CC; or possibly purely mathematical) study.
- &#x1F6A7;code `design`&#x1F6A7; &#x2753;:  Kann fast komplett raus, glaube ich - habe keinen Code design göaube ich?
  To be used only if the article is artifact-centric instead of purely empirical, i.e., 
  if the article's main contribution is an artifact or the knowledge how to build it,
  not the empirical results obtained with its help.
  A `design` statement provides information about the design, design process, and designed features of 
  an artifact, such as software, a process, or a method.  
  We call articles where the abstract contains a design statement "design articles"
  (or artifact-centric articles). 
  - Such articles will typically also contain some empirical contribution and `method`/`result` are used
    for its description.  
  - The "designed features" mentioned above are known at design time
    and classified as `design`.
    This is in contrast to emerging features,
    which can only be determined empirically and are classified as `result`.
  - Top-level design _goals_ (and non-goals) are classified as `objective`.
    Subordinate design goals and non-goals are classified as `design`.
  - Statements about the design of subordinate artifacts, 
    that do not represent the main contribution but rather only aid an empirical study, 
    are classified as `method`.
- code `result:ct`:  
  Information about the immediate outcome of a study in the form of empirical results.
  `result` is often described in past tense and can be recognized by words like "observed", "&#x1F4CC;" 
  &#x1F6A7;`:c` signalises, that this result could've been made into a conclusion if formulated differently. &#x1F6A7;
   This can be the case because conclusion-like information is named, but not shown (which would mean information is only superficially described, `:t`) 
   or because there is no generalization happening. 
  &#x1F6A7;See `claim:iu`.
- code `summary`: &#x2753; I have this code, but it's unclear in my coding rn &#x2753;
  A statement that summarizes several results, but does not provide new information.
  A summary statement does not generalize beyond the immediate results.
      
      
### 2.5 Core codes for _Outlook_
      
The three codes `fposs`,`fneed`,`fwill` act like different confidence levels, confidence increasing from left to right.
      
- code `fposs`:  
  Statement about what future research is now possible (i.e., could now be done, by whoever).  
  &#x2753; Note: Statements what practitioners can now do are `conclusion`! - WHY &#x2753;
- code `fneed`:  
  Statement about what future research should be done (by whoever).
  Also used when authors "hope" (etc.) for certain research to be done. &#x2753; ich have hope immer zu fposs zugeteilt - villeicht habe! ich die codes ander genutzt....&#x2753;
- code `fwill`: 
  Statement about what will happen in the future. 
- code `fgap`:  
  Statement about what is still not known after the study.
- code `fwork`:  
  Explicit statement about what future research the authors intend to do.
      

### 2.6 Less common codes - &#x1F6A7; &#x1F6A7; &#x1F6A7; &#x1F6A7; &#x1F6A7; &#x1F6A7; &#x1F6A7; &#x1F6A7; &#x1F6A7; &#x1F6A7; &#x1F6A7; &#x1F6A7;

- code `limitation`:  
  information about limitations, threats to validity, and the like
  of the study or its results.
- code `resourcepointer`:  
  A reference to a concrete external resource such as 
  a software artifact, materials package, data package, appendix,
  or similar item.
      
      
### 2.? Suffixes (for conclusions) and others) - maybe make two sections out of this

### 2.? Less common codes

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
