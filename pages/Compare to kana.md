title: Compare to kana
id: comparekana
main_file: Compare to kana.py
type: addon
status: working
status_color: green
status_text_color: white
abstract: When typing in Japanese readings, remove the kanji bit from the correct text, so that the red and green coloring of the answer works correctly.
first_image: compare_to_kana.png
first_alt: The typed-in answer was compared to the kana only.
ankiweb_id: 4091556602

A typical model for learning Japanese has a field called “Reading”. In
that field, the reading (kana) is stored *along with the kanji*. For
example, in a fact defining the Japanese word for police station, the
reading field would look like 「警[けい]察[さつ]署[しょ]」. Like this,
the standard templates `{{furigana:Reading}}` and `{{kana:Reading}}`
work.

But this causes a problem when you use the type-answer
feature. Normally, you would type just the kana, but they are then
compared to the whole stored answer, including the kanji and square
brackets. So, even when you type the answer correctly, a large part
will be marked in red. This add-on does a filtering of the correct
answer like the kana template and compares the typed text only with
the kana part of the stored text.

## Setup

The kanji are removed when the model name contains the word “Japanese”
and the field name contains “Reading”. Use `{{type:Reading}}` or
`{{type:NN Reading}}` in your cards.

## “Correct answer was:”

<figure style="width:410px;"><img
src="images/compare full reading.png" alt="Correctly typed reading and
lots of red.">
<figcaption>Even though the reading was typed correctly there is a lot
of red and extra text.</figcaption></figure>

With this add-on, when typing Japanese readings, the “Correct answer
was:” text is not shown at all. This is partly due to the way the
add-on operates, but i see this as a bonus, not a problem. At this
time, people who really want this text could possibly add it to their
own copy of the add-on. (In other words,
[UTSL](http://www.jargon.net/jargonfile/u/UTSL.html).)