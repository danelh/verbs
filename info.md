---
layout: default
title: info
---
# Latin Verb Trainer

## Table of Contents

- [Intro](#intro)
- [The Verbs](#the-verbs)
- [Verb Selection](#verb-selection)
- [Level](#level)
  * [Frequencey](#frequencey)
- [Inflection selection](#inflection-selection)
- [Missing mutations](#missing-mutations)
- [Practice and exam modes](#practice-and-exam-modes)
- [Save session's parameters](#save-session-parameters)
- [Contact information](#contact-information)

## Intro 
This trainer was created mainy to allow the user to practive Latin verbs inflections. Each inflection (or mutation as reffered in this Trainer) consisted of the verb-root and the tense-inflection. The user is given a mutation and is required to inflect it. For example for the verb "_amo_" and "_indicative active present 1st plural_", the correct inflection is _amamus_.

The correct answers were taken from Wiktionary. In several cases there is more than one attested option for inflection. For example, according to Wiktionary for "[_amo_](https://en.wiktionary.org/wiki/amo#Latin)" and "_indicative active perfect 2nd singular_" there are two options: _amavisti_ and _amasti_. The Trainer will always take the first option listed as correct. Usually, those first options also happen to be the regular forms. 

## The Verbs

The Trainer uses 5371 verbs from wiktionary. This is by no means the attested number of Latin verbs; yet, a verb missing from the Trainer is probably quite rare.

Several different verbs might have the same verb-root. [_Volo_](https://en.wiktionary.org/wiki/volo#Latin), for example, has two distinct conjugation tables: one of the first conjugation (meaning to fly) and a second of irregular conjugation (meaning to wish). As long as the verb has different conjugation types, as with _volo_, the Trainer distinguishes between them by adding parentheses containing the conjugation types. Hence the Trainer does not have the verb _volo_, but has instead two distict verbs: _volo(first)_ and _volo(irregular)_.

Unfortunately, the cases different conjugation of the _same_ type, are overlooked by the Trainer. Example to this is the verb [_edo_](https://en.wiktionary.org/wiki/edo#Latin) that has two different  conjugation tables of the third conjugation-type. In such cases the Trainer will have only one verb with parentheses, and will take the correct answer from the **second** table, so for" _edo(third)_" and "_indicative active perfect 1st singular_" the correct answer would be _edidi_ (meaning I produced) and not _edi_ (meaning I ate).

To sum everything up, we can look at the verb [_sero_](https://en.wiktionary.org/wiki/sero#Latin) which has 3 distinct conjugations: two of them of the third type, while the remaining one is of the first. The Trainer will split this verb into two: one of the first conjugation-type and the other of third conjugation-type (the second table will be selected).

## Verb Selection
There are 3 ways to select verb to practice on:

 1. **Manual selection from list**:  in the list you can search for your verbs from the Trainer list, and select them.  Selecting a verb from the list, will append it to already selected verbs displayed in the box. 
 2. **Writing directly in the verbs box**:  it is possible to write the verbs directly in the selected-verbs box. Make sure to have the verbs comma separated.  This option is recommended only in cases you have predefined list of verbs - for example when you saved the verbs from previous session - you can simply paste them in the box. **In this way you can load your verbs easily**. [Note that you may enter a verb which will be ultimately removed from the Trainer if it's missing from the list:  _volo_ , for example, will be removed because it is missing from the list - Trainer expected _volo(first)_ or _volo(irregular)_ .
3. **Automatic generator**: you can tell the Trainer to automatically generate verbs. To use this option you should specify 1) how many verbs you want to be generated 2) the level. Then you should click "Generate". The generated verbs will override  the current selected verbs.

## Level

In order to use the automatic generator, you have to specify a  _level_ . The _level_ parameter basically tells the automatic generator which verbs are entitled to be generated.  The goal of this parameter is to generate verbs that the user is likely to be familiar with, rather than complete random verbs from the list. To achieve this, the verbs were sorted by **frequency** . Thus, selecting "Top 10%" option means that the verbs will be generated from 10% of the verbs which are the most frequent (pool of 537 verbs). The beginner may find this tool helpful for increasing his vocabulary of frequent verbs.   

### Frequencey

The verbs were sorted by frequency using the [Perseus Vocabulary Tool's](http://www.perseus.tufts.edu/hopper/vocablist?lang=la) _weighted frequency_ attribute. the documents pool contained docs of prominent authors ([full list](docs_names.txt)).In terms of frequency, the Trainer does not distinguish between differnt verbs of the same root like _volo(irregular)_ and _volo(first)_: they both have the same frequency for the Trainer. (the highest of the two).

## Inflection selection

Inflection selection is quite straight-forward. It should be noted, however, that the inflections which regularly  use the _perfect passive participle_ (such as _indicative passive perfect_), are missing from the Trainer for all verbs, and can't be selected. To practice those, you can use the participle itself. 
You can select more than one inflection.

## Missing mutations

Many verbs cannot be inflected in all forms. The verb [_placeo_](https://en.wiktionary.org/wiki/placeo#Latin), for example,  is missing imperatives, or the verb [_fido_](https://en.wiktionary.org/wiki/fido#Latin), is missing supine. The Trainer will not ask this mutations from the user, and will note those missing inflections in the window. Note that deponent verbs like [_for_](https://en.wiktionary.org/wiki/for#Latin) are missing  the inflections which using the _perfect passive participle_ (like  _indicative **active** perfect_). To practice those, you can use the participle itself.

In case a verb was selected, which is not in the Trainer list, it will be noted in the window. It can happen either when the verb is simply not existing in the Wiktionary, or that Trainer [expects parentheses](#the-verbs) for this verb.

## Practice and exam modes

The Trainer has two modes of operation: practice or exam. The two modes are similiar in nature: in both the user is given mutation and required to inflect it correctly. The user should submit his answer by pressing Enter key. After an answer was submitted, the Trainer will indicate the user wheather he was correct. When the user is correct, the correct answer will be displayed in green, else the correct answer will be in red. Moreover, at the right side, the user can see his stats so far, as well as the "mutations left" which indicate the number of different mutations that might be displayed to show the user how far he is from completing the practice or the exam. To change mode, the user should click on the mode switch.

In **practice mode**, the mutation in question is selected semi-randomally (bias towards mutations the user was wrong in recently). In this mode a given mutation might be asked many times without limit; thus, theoritically, the practice might last ad infinitum. **It is under the user responsibity to prevent a mutation from being asked again**: to do so, instead of submitting an answer, he should press the right arrow key (→). After pressing (→) the user should see appropiate message, and the number of "mutations left" (in the right side) going down. The user is adviced to do so when he is sure of the correct answer (The Trainer will tell the user to consider pressing (→) after he was right three times in a row, yet the final descision is always under the user discretion: he might do so before or after that). Ideally, the practice will end when the user pressed (→) to all the mutations, but the user might switch to exam mode or select other verbs/inflection any time he wishes. The user is encouraged, especially in this mode, to click on the verb in question when he is unsure of the meaning of the verb or want to see the full conjugation table.

**Exam mode** should be used when the user feels confident about the inflections of the selected verbs, and he wants to test his level. In this mode every mutaion is asked only once (no need to press (→). At the end of the exam the user wil see his final score.


## Save session's parameters

Selecting the inflections and auto verbs-generation settings might be tedious, especially when we are using them for long.  In order to avoid re-selection of those parameters each time we open the Trainer,  the selected parameters are saved in address bar of the browser. Every change of the selected inflections or every click on "generate" button, will trigger a change in the address bar that will contain the newly-selected parameters. If you want to save the settings, simply copy the line of the address bar and save it for future use. When you use that link, the Trainer will be opened with the selected parameters, and with the verbs already generated - so you can start practice right away.

If you want to save the verbs themselves (rather than the verbs-generation parameters), you should copy the text in the [verbs box](#verb-selection), and save this text for future use. To use the saved list, you have to paste it in the verbs box.

## Contact information 

[See here](https://danelh.github.io/about)
