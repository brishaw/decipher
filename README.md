# decipher
My son came to me requesting to build a translator from his teacher's secret language. 

He had a sheet that had secret symbols that represented each letter of the alphabet. 

I scanned the sheet and traced each symbol in Photoshop, saving each symbol with the name that corresponded to the letter it represented ie; symbol_a.svg.
Then I used javascript and used a single object that maps letter → filename directly. I had started with two parallel arrays that keep in sync by position but that turned out to be to easy to accidentally misalign.

Here's how it works:

Letters → Symbols tab: type anything — letters show as symbol images with a small caption letter underneath, spaces become gaps, and anything not a-z (numbers, apostrophes, punctuation) shows as plain text so cat's 2 renders sensibly.
Symbols → Letters tab: click symbol tiles to build up a word, Space adds a space, Enter finalizes it into the decoded message below (physical keyboard Space/Enter work too), Clear resets everything.
