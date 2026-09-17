# Spelling Practice

A single-file spelling dictation tool for kids. The parent types in this week's word list, the app reads each word aloud, the child writes it down on paper, and the full list is revealed at the end for self-checking.

No build step, no dependencies, no framework — it's one `index.html` file.

## How to use

1. Open `index.html` in a browser (or visit the deployed link).
2. Type one word per line into the word list.
3. Adjust the speaking speed and how many times each word is said, if you like.
4. Tap **Start**. The app speaks each word; your child writes it on paper.
5. Use **Back** / **Again** / **Next** to move through the list or re-hear a word.
6. After the last word, the full list is revealed so your child can check their own spelling.

## Pictures and sentences

Each word is shown as a picture plus a fill-in-the-blank sentence, so your child has a meaning
to hang the word on rather than just a sound. A **Show the word** button reveals the answer in
the blank when they want to check themselves — tapping it again hides it.

Around 260 of the most common prep / Year 1 words (the high-frequency words most weekly lists
are drawn from) already have a sentence and a picture built in, so most lists just work.

For anything else — a name, a topic word, or if you want your own sentence — write it on the
same line, separated by `|`. Use `___` for the blank, and put an emoji last:

```
come | Please ___ and play with me. | 🧸
jetty | We fished off the wooden ___. | 🎣
```

Both the sentence and the emoji are optional. A word with neither, and not in the built-in list,
simply shows the dinosaur on its own — nothing breaks.

Note that abstract sight words ("could", "there", "should") have no picture of their own, so the
picture illustrates the *sentence* rather than the word: "I wish I ___ fly like a bird." with a bird.

Your word list, speed, and repeat settings are saved in the browser (`localStorage`) so they're still there next time you open the app.

## A note on voice quality

The read-aloud voice uses your browser's built-in text-to-speech (the Web Speech API), which depends on which system voice is installed. On a Mac, the default "compact" voices sound fairly robotic. For a much more natural voice, download an **Enhanced** or **Premium** voice under **System Settings → Accessibility → Spoken Content → Manage Voices** — the app will prefer the higher-quality voice automatically once it's installed.
