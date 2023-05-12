# Conclusions Master Thesis - CodeBook.alpha - testing the PR

&#x1F517; &#x1F517; &#x1F517; &#x1F517; &#x1F517; &#x1F517; &#x1F517; &#x1F517; &#x1F517; &#x1F517;

Smileys are used in front of the sentence/paragraph they should signalise something for. 
Sometimes there are two of them around one sentence, the sentence inside these signs is a ToDo or Memo for the task, but what follows the second smiley then is still the sentence or paragraph in question.

&#x1F517; - this section or part is identical to the qabstracts codebook

&#x1F440; - this needs to be revisited. I am not happy with the definition, description, grammar, wording or whatever

&#x1F4CC; - reminder for ToDos. May mean that an information is still missing/unclear or that I need to look something up

&#x1F6A7; - in construction, this is a code/part I've started to work on but that is not quite done yet

&#x2753; - somthing that's just barely there, very unclear and still needs a lot of work


## 2. Codebook: Codes for sentences

&#x1F4CC;I need to reduce my number of suffixes and assign levels of importance to them.&#x1F4CC; Suffixes are harder to use than Codes because the are omnipresent and would have to be remembered constantly. This is hard. To make the use easier I can make suffixes mandatory or optional. optional Suffixes are not there for quantitative analysis but to collect examples. I have to mark mandatory and optional suffixes.

&#x1F4CC;Too much Codes&#x1F4CC; I have too many codes, the amount I have makes it harder to learn all the codes and use them correctly. And most importantly the more codes we use, the lower the intercoder agreement? (was war der korrekte begriff)? will be. To reduce my codes, I'll have to differentiate between codes that will be important for the qualitative evaluation of conclusions and codes that are only there to let me grasp the structure of conclusions better, but do not influence the qualitative evaluation of coding.


### 2.1 The conclusion-sections flow 

Conclusion-sections are similar to the abstracts archetype, the sequence of stretches is similar, but the occurence of stretches is different. 

The following codes will be defined in detail in subsequent sections.

&#x1F440;The (maximum) pattern: 

1. A conclusion may consist of three parts, in this order:
   _Introduction_, _Study Description_, _Outcome_ and _Outlook_. 
   _Introduction_ and _Study Description_ are often missing, they are roughly seen in every 5th article.
   It is rare to have all stretches in a single conclusion.
2. &#x1F440;Turning points connect the parts:
   - &#x1F440;A statement of the study goals (`objective`) connects _Introduction_ to _Study Description_ or _Outcome_ .
     _Introduction_ always ends into an `objective`.
     _Study Description_ always starts with an `objective`.
     <there is almost never an objective without intro or descr - ausnahmen sind AhmMerBa und BesMarBos>
     Sometimes the `objective` is described in several connected sentences.
     In very rare cases `objective` occurs without connection to _Introduction_ or _Study Description_, but always at the start of the conclusion section 
     and is followed by _Outcomes_.
   - &#x1F6A7;not always true&#x1F6A7;A generalizing statement ("take-home message", `conclusion`) 
     connects _Study Description_, _Outcomes_ and _Outlook_.
     There are almost never `conclusion` sentences that follow each other directly.
     In very seldom cases there is no `conclusion`.
3. The _Introduction_ first introduces the topic area of the study and what is known
   and then seldomly points out a gap in knowledge (`background`).
4. For an empirical article (which are the only ones we are looking at), the _Study Description_ often begins with
   method description (`method`), followed by results description (`result`).
5. &#x1F6A7;_Outcome_ is a mixup of knowledge gained as a result of the study.
   This includes `result`, `conclusion`, `artifact`, `teaser` and any of the codes in _Outlook_.
   This stretch at its minimum consists of at least one `conclusion` or soemthing that coul've been a conclusion (`:0`).
    A `result` in this position typically explains a conclusion.
   Sometimes `result` is found in _Outlook_ and most of the times this means the authors intended a "take-home-message",
   but did not take the  last step to generalize and make it a `conclusion`.
   Lists of contributions are always a _Outcome_ stretch and are typically a mix of all codes with no certain structure. <FloMorZha und BalRal>
 6. &#x1F6A7;_Outlook_ talks about future research and states 
   what could now be done (`fposs`, for future possibilities),
   what should now be done (`fneed`),
   what will most definetly happen (`fwill`)
   what the authors themselves intend to do (`fwork`).
   Additionally there can be `conclusion`s found in between future research. &#x1F4CC;CHECK (sometimes its hard to differentiate betw conclusion and fneed)
   Several of these may occur, in no particular order. 
   This stretch always ends the conclusions. There is only one exception when _Outlook_ does not end the conclusion:
   If the conclusion has multiple subsections then _Outlook_ may be found in a seperate subsection.
 
&#x2753;**Possible patterns of conclusion sections:**&#x2753;
   - here are my outcomes!:
     The section starts directly with the _Outlook_ and focuses solely on those. 
     The section may start with _Introduction_ and give informations that make the following conclusions easier to understand.
   - like abstract/summary: 
     Has every stretch in the section, but only talks about each briefly. 
     Conclusions are ons-two sentences at most and are not more in focus than the other informations.
     Also it is quite similar to the abstract itself.
   - lure the reader in: (eig eher ein gedankenmodell, als eine spezielle art )
     This type of conclusion typically has a lot of `teasers` and few informations to take home. 
   

**The flow guides the coding**: During coding, we will expect the next sentence
to be either part of the same stretch or the beginning of one possible successor described in the flow.  
Only if the next sentence clearly defies any such interpretation will we consider
a different code for it. Also, keep the exceptions in mind.


### 2.2 Core codes for the turning points

From _Introduction_ to _Study Description_:
- code `objective`:  
  &#x1F517;one or more of this work's 
  top-level research goals,
  specific top-level research interests, or
  top-level research questions.  &#x1F517;
  Objectives sentences often contain material that is ambiguous as goal-or-method
  or as goal-or-design. &#x1F517;In those cases, assign two codes only if there is no 
  method (or design) information elsewhere in the abstract.&#x1F517;
  If the method (or design) information is too specific and concrete to be a goal,
  assign two codes in any case.
   If a study does a SLR this already counts as obhective.

From _Study Description_ to _Outlook_:
- code `conclusion`:  
  &#x1F517; A take-home message that is less specific than one or more results.
  Usually a generalization from the results, sometimes a non-obvious existence proof statement, which is non-obvious based on pre-study knowledge.
  A conclusion is written in present tense.
- conclusion suffixes `conclusion:g` XOR `conclusion:e` describe if the conclusion is a generalization (`:g`) or a an existence proof (`:e`).
- &#x1F440; conclusion suffixes `conclusion:r` XOR `conclusion:p` describe whom the `conclusion` is for.
   This Code is only used if the information of the sentence is clearly meant for only researchers (`:r`) or practitioners (`:p`).
- &#x1F6A7;conclusion suffixes `conclusion:1` XOR `conclusion:1.5` XOR `conclusion:2` XOR `conclusion:3` 
   mark how confident the authors express their `conclusion`.
  `:1` stands for the lowest confidence. This suffix is used when there are words("could", "can", "maybe", ...) that make an obvious effort to make the conclusion easy to agree. 
      `:2` stands for a rather neutral `conclusion`, which does not try to make it more agreeable or hype it up. The conclusion is firm.
      `:1.5` stands in between `:1` and `:2`. It catches all conclusions who are not perfetly firm, but also don't make an obvious effort te be agrereable, but a rather small one.
       `:3` shows the highest confidence and should be used, if authors make their conclusions seem overly true. (most unsure abt this one...) 
   (&#x2753; The definition is not done + idk if this suffix is needed &#x2753; Additionally there is a suffix `result:0` used on `result`, which is used for a result who could have been a `conclusion`.)
  
   
### 2.3 Core codes for _Introduction_

- &#x1F440;rename intro indtroduction? bc its a fusion of all introduction codes?&#x1F440; code `background`:  
  Information about the larger topic area of the work, the state-of-the-art, definitions, related work as motivation,
  the problem to be solved and what is known in general.
  Sometimes also about what was not known before the study and what research needs to be done.
  `background` sometimes. If it does it's often a block of several such sentences.


### 2.4 Core codes for _Study Description_

- code `method`:  
  Information about the approach or setup of an empirical (&#x1F440; or possibly purely mathematical) study,
  what were the steps taken to reach the objective.
      This also includes artifacts like small programs built to aid the study.
- code `result:ct`:  
  Information about the immediate outcome of a study in the form of empirical results.
  `result` is often described in past tense and can sometimes be recognized by words like "observed" or "found".
      <even though "result(s)" is often seen there too it is often seen with conclusions too which makes this a not so good indicator word>
  &#x1F6A7;`:0` signalises, that this result could've been made into a conclusion if formulated differently.
   &#x1F440; This can be the case because conclusion-like information is named, 
         but not shown (which would mean information is only superficially described, `:t`) 
   or because there is no generalization happening. 
      
      
### 2.5 Core codes for _Outlook_
      
The three codes `fposs`,`fneed`,`fwill` act like different confidence levels, confidence increasing from left to right.
      
- code `fposs`:  
  Statement about what future research is now possible (i.e., could now be done, by whoever).  
  &#x1F440; Note: Statements what practitioners can now do are `conclusion`!
- code `fneed`:  
  Statement about what future research should be done (by whoever).
  &#x1F440;hope gehört für mich zufposs, weil es weder initiative der autoren ist noch von ihnen direkt empfohlen wird. &#x1F440; Also used when authors "hope" (etc.) for certain research to be done. 
- code `fwill`: 
  Statement about what will happen in the future, the authors are certain about.
- &#x1F6A7;Brauche ich den Code? was sagt der für mich aus? ist er indiz für irgendwas?&#x1F6A7;code `fgap`:  
  Statement about what is still not known after the study.
- code `fwork`:  
  Explicit statement about what future research or research related tasks the authors intend to do.
      
      
### &#x2753; 2.6 Special code/stretch `artifact`
         
- &#x1F4CC; An `artifact` can be a guide, a taxonomy, a method. If it is a document, it is autonomous from the article.
  The content of an `artifact` is often only described in a superficial way (meaning no actual learnings are explained, `teaser`).
- &#x2753; &#x2753; &#x2753; &#x2753; &#x2753;
see Miro, I have so many unanswered questions here... Thing is an `artifact` makes my whole flow/archetype fall out. 
I'll have to look into this again to see if there are similarities between _Artifact_ stretches. Since `artifact` seldomly occurs alone.
Now I also have the problem, how to code it. Is it better to use a own code or just a suffix? what exactly is an `àrtifact`?
Should I code the information wrapped into the artifact and just make it visible this is an artiofact?
Also (unrelated) I DO KNOW, that having an artifact in the articale does not make it impossible to deliver informative conclusions next to the
artifact description / give examples that are informative an have conclusion character. So how important is it to code informations behind the artifact? But I do think it is important, bc if there are informations that are like non obvious then there must be a conclusion in the article an i even know where it is - in the artifact. And at that point I can assume that the authors could've written an informative conclusion in the conclusion but chose not to...
Also this code is in fact similar to the design code. But only in some cases. A i,portant difference is, that design is supposed to be in the _Study description_ while artifacts that could be designs are often found in between conclusions and future work.
&#x2753; &#x2753; &#x2753; &#x2753; &#x2753;
      
      
### 2.7 Less common codes

- code `limitation` &#x1F440;nur in genau einem Dokument ... (wie related work als absatz auch)- gibts da ne andere lösung&#x1F440;:  
  &#x1F517;Information about limitations, threats to validity, and the like of the study or its results. If seen, typically after `conclusion`.
- &#x1F517; code `resourcepointer`:  
  A reference to a concrete external resource such as 
  a software artifact, materials package, data package, appendix or similar item.
- &#x1F6A7; code `defensive` or suffix `:def`:  
  This stands for "defensive". It is used on sentences which deny generalizations or play down results as "minimal".
- &#x2753; code `justification`:
  A sentence which exists to make the articles results seem better or more relevant. (I.e. compare it with previous studies that did worse.)
- &#x1F440;code `teaser`:
  If authors describe some kind of information, but don't explain the information itself or give an example in the conclusion section.
  A teaser `:t` is a superficial description which lets the reader know of the existence of some information,
  but does not reveal the information in the conclusion-section itself.
  &#x1F6A7;Depending on the accuracy with which the location of the teasers is given I'd like to assign a code or suffix. I'm not sure if there are two or three levels: the highest accuracy (`-direct`) could be the name of a new theory, a pointer to some section or a pointer to some table - something that is easy to find in the document. The lowest accuracy (`-no_pointer`) would be that there is no pointer given (f.e. "We have found out X."). Now, I am not sure if the in betweens are needed (but I've seen them quite often actually). These often look like "We documented X in our study/guide" - this refers to some section rather than a single point, to find the info the reader probably has to search through the pointed section.&#x1F6A7;
         Often found when `artifacts` are described. (&#x1F6A7; or the conclusion is treated as a summary of the paper)
  
      
      
### 2.8 Suffixes 

- suffix `:0` (for `teaser` and `results`):
  There is information in this sentence which makes us think this could've been a conclusion, there are two options why.
  One option is that the generalization step is missing, meaning all informations are there but the sentence is too specific.
  The other option is that there are informations teasered which seem very likely to have conclusion character. 
  &#x1F6A7; Would it be a good idea to have different suffixes for those cases? Since they should also be viewed differently in the final analysis: 
         A missing generalization may mean the authors did not want to take any risk,
         while a teaser may mean the authors did not see the conclusion as a place to put conclusions into.&#x1F6A7;
- suffix `:unexplained` or `explained`:
  These mark an unexplained/explained abbreviation. Unexplained means it is not explained or written out in the conclusion-section itself.
  Explained means it is explained or written out in the conclusion-section itself.
- &#x2753; suffix `:explanation_sentence`:
  If a sentence gives more information to the topic of a a nearby sentence, like details, definitions or background informations.
  If a sentence is assigned this suffix, it is very likely that the code is the same as the sentence it gives extra information for.
  This suffix is more a coding helper than relevant for the later analysis. It does not need to be coded for every occurence and all the time.
       

### 2.9 Extra codes 

These codes can never occur alone, only in conjunction with one of the others.
They start with a dash to signal this and should be given last. 

- &#x1F517;code `-hype`:  
  The sentence praises the work beyond what a factual statement might state.
  The code does not talk about the truth of the statement (which is often difficult
  to judge from the abstract alone), but about the tone in which
  the statement is made.
  Plain positive properties do not qualify ("This is helpful because..."),
  only emphasized ones do ("This is tremendously helpful because...").
  "very" does not count as hype.
  The most common places for this to occur are 
  &#x1F4CC;`result`, `conclusion`, `fposs`, `need`, `method`.  
- &#x1F517;code `-ignorediff`:  
  If the script flags a coding discrepancy that, after discussion, you and your fellow coder
  agree should be left in (because the two codings represent two different reasonable interpretations),
  add this code in one (and only one) of the codings to mark the discrepancy as resolved.
- code `-timid`:  
  Applies to `conclusion` only. 
  To be used when the generalization made is overly vague or small.

In contrast to the sentence classifications, which are intended to be objective
(hence the use of two coders and the use of `-ignorediff` where objectivity reaches its limits),
the codes `-hype`, and `-timid` are optional additional attributes
that are considered subjective. 
Apply them with your own good judgment and keep in mind that
"we are gentle in detecting negative aspects".


### 2.10 Codes for special circumstances 

- &#x1F517; code `cruft`:  
  This sentence is not part of the abstract.
  It is garbage that should have been removed during the preparation of the abstract files (i.e. page headings or numbers).
- &#x1F517; code `X`:  
  Undecided class. The sentence needs to be revisited and classified;
  consider using `fgrep {{X}}` to find these cases.
  Use `X` only rarely and only when you cannot _yet_ make up your mind.
  Such a code will likely result in a discrepancy with your fellow coder.
  It must always eventually be replaced with a proper code.
- code `new`:
  Use this code for sentences where you think a new code is needed. Note the needed code below in the comments.
- code `I-give-up`:
  Use this code for sentences that you just don't understand, because they are poorly written. Maybe because of confusing grammar or wording. 
      
      
      
## Memos
         
