title: Fix AnkiDroid’s negative review times
main_file: fix_negative_review_times.py
date: 2013-05-07
layout: addon
status: obsolete
status_color: yellow
status_text_color: black
abstract: "Fix negative review times."
first_image: time_fix.png
first_alt: 'Some Python code'
first_caption: "The code that is run."
ankiweb_id: 3009264632

This applies the fix for the
[AnkiDroid problem](http://code.google.com/p/ankidroid/issues/detail?id=1449)
discussed in the Google Code issue tracker. When you see negative
review times, either in AnkiDroid or in the statistics window of the
desktop client, go there for information.

This add-on simply applies the
steps
[described in the thread](http://code.google.com/p/ankidroid/issues/detail?id=1449#c23).

<blockquote class="nb">This only resets the times. It does not prevent
the same problem from occuring again.</blockquote>

It looks like AnkiDroid is no longer producing this problem, so there
seems to remain little need for this add-on.