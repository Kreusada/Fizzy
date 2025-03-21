<h1 align="center">
  <br>
  <a href="https://github.com/Kreusada/Fizzy">
    <img src="https://raw.githubusercontent.com/Kreusada/Fizzy/main/fizzy.png" alt="Fizzy">
  </a>
  <br>
  Fizzy
  <br>
</h1>


Fizzy is a fun bijective text transformer. It performs base-64 encoding on a predefined charset
of unicode characters that resemble bubbles through their appearance. Each character is transformed and joined together with the Latin lower case "o" character.

Please bear in mind that not all unicode characters are compatible with all systems.
This won't have an effect on functionality.

The text transformer is **bijective**, meaning there is a one-to-one correspondence between the original and the transformed text.

I made this module for fun, it advise against using it in a practical context other than to play around with it.

## Usage

Import the module:

```py
import fizzy
```

Use the **fizz** function to make your text fizzy:

```py
>>> import fizzy

>>> fizzy.fizz("Hello world!")
'Ⓞ᧐o౦᧐o᠐᧐o᠐᧐o᪐᧐o🇴o꣐᧐o᪐᧐o᱀᧐o᠐᧐o௦᧐o𑵐'
```

Use the **defizz** function to revert fizzy text to its original form:

```py
>>> import fizzy

>>> fizzy.defizz("Ⓞ᧐o౦᧐o᠐᧐o᠐᧐o᪐᧐o🇴o꣐᧐o᪐᧐o᱀᧐o᠐᧐o௦᧐o𑵐")
'Hello world!'
```

Use the **isfizzy** function to check if the given text is fizzy:

```py
>>> import fizzy

>>> fizzy.isfizzy("ꝏ᧐o౦᧐o୦᧐o᱀᧐o౦᧐o⁰᧐")
True

>>> fizzy.isfizzy("o0o0o0o0o0o0o0")
False
```

### Further Fizz Examples

```py
>>> import fizzy

>>> fizzy.fizz("Apple")
'᧐᧐o᭐᧐o᭐᧐o᠐᧐o౦᧐'

>>> fizzy.fizz("12345")
'᮰o᱀o᱐o⁰o₀'

>>> fizzy.fizz("🚀💡🎨")
'𖫩߀૦o𑵐ꓳ૦o๐𛱄૦'

>>> fizzy.fizz("愚蠢的功能")
'߀°оo᛫🇴Ⓞo°߀ₒo૦𐓪Оo𐴰꯰Ⓞ'

>>> import string

>>> fizzy.fizz(string.punctuation)
'𑵐o᛫o୦o௦o౦o೦o൦o๐o໐o၀o᥆o᠐o0o᪀o᪐o꩐o.o𐒠o𐴰o０o𑃰o𖫩᧐o०᧐o০᧐o*᧐o੦᧐o૦᧐o🇴᧐o.᧐o𐒠᧐o𐴰᧐o０᧐'
```

## Command Line Interface

The CLI commands work in the same way as the module.

```bash
$ fizzy fizz cool text here
୦᧐o᪐᧐o᪐᧐o᠐᧐o🇴o⁰᧐o౦᧐o꤀᧐o⁰᧐o🇴o๐᧐o౦᧐o᱀᧐o౦᧐
```
```bash
$ fizzy defizz ୦᧐o᪐᧐o᪐᧐o᠐᧐o🇴o⁰᧐o౦᧐o꤀᧐o⁰᧐o🇴o๐᧐o౦᧐o᱀᧐o౦᧐
cool text here
```

## Installation

Install from pip.

```
pip install fizzy
```

## Characters

| Character   | Name                               | Code   |
|-------------|------------------------------------|--------|
| 𖫩           | Bassa Vah Letter Oo                | 16ae9  |
| ᧐           | New Tai Lue Digit Zero             | 19d0   |
| O           | Latin Capital Letter O             | 4f     |
| ꯰           | Meetei Mayek Digit Zero            | abf0   |
| °           | Degree Sign                        | b0     |
| О           | Cyrillic Capital Letter O          | 41e    |
| о           | Cyrillic Small Letter O            | 43e    |
| ₒ           | Latin Subscript Small Letter O     | 2092   |
| Ⓞ           | Circled Latin Capital Letter O     | 24c4   |
| 𐓂           | Osage Capital Letter O             | 104c2  |
| 𐓪           | Osage Small Letter O               | 104ea  |
| 𐔖           | Elbasan Letter O                   | 10516  |
| 𐖮           | Vithkuqi Small Letter O            | 105ae  |
| 𐤬           | Lydian Letter O                    | 1092c  |
| 𛱄           | Duployan Letter O                  | 1bc44  |
| ⓞ           | Circled Latin Small Letter O       | 24de   |
| Ⲟ           | Coptic Capital Letter O            | 2c9e   |
| ⲟ           | Coptic Small Letter O              | 2c9f   |
| ꓳ           | Lisu Letter O                      | a4f3   |
| ꝏ           | Latin Small Letter Oo              | a74f   |
| Ꝏ           | Latin Capital Letter Oo            | a74e   |
| Ｏ          | Fullwidth Latin Capital Letter O   | ff2f   |
| ｏ          | Fullwidth Latin Small Letter O     | ff4f   |
| 𐊫           | Carian Letter O                    | 102ab  |
| 𐌏           | Old Italic Letter O                | 1030f  |
| ᳃           | Sundanese Punctuation Bindu Cakra  | 1cc3   |
| ߀           | Nko Digit Zero                     | 7c0    |
| ०           | Devanagari Digit Zero              | 966    |
| ০           | Bengali Digit Zero                 | 9e6    |
| *           | Asterisk                           | 2a     |
| ੦           | Gurmukhi Digit Zero                | a66    |
| ૦           | Gujarati Digit Zero                | ae6    |
| 🇴           | Regional Indicator Symbol Letter O | 1f1f4  |
| 𑵐           | Masaram Gondi Digit Zero           | 11d50  |
| ᛫           | Runic Single Punctuation           | 16eb   |
| ୦           | Oriya Digit Zero                   | b66    |
| ௦           | Tamil Digit Zero                   | be6    |
| ౦           | Telugu Digit Zero                  | c66    |
| ೦           | Kannada Digit Zero                 | ce6    |
| ൦           | Malayalam Digit Zero               | d66    |
| ๐           | Thai Digit Zero                    | e50    |
| ໐           | Lao Digit Zero                     | ed0    |
| ၀           | Myanmar Digit Zero                 | 1040   |
| ᥆           | Limbu Digit Zero                   | 1946   |
| ᠐           | Mongolian Digit Zero               | 1810   |
| 0           | Digit Zero                         | 30     |
| ᪀           | Tai Tham Hora Digit Zero           | 1a80   |
| ᪐           | Tai Tham Tham Digit Zero           | 1a90   |
| ᭐           | Balinese Digit Zero                | 1b50   |
| ᮰           | Sundanese Digit Zero               | 1bb0   |
| ᱀           | Lepcha Digit Zero                  | 1c40   |
| ᱐           | Ol Chiki Digit Zero                | 1c50   |
| ⁰           | Superscript Zero                   | 2070   |
| ₀           | Subscript Zero                     | 2080   |
| 〇          | Ideographic Number Zero            | 3007   |
| ꣐           | Saurashtra Digit Zero              | a8d0   |
| ꤀           | Kayah Li Digit Zero                | a900   |
| ꧐           | Javanese Digit Zero                | a9d0   |
| ꩐           | Cham Digit Zero                    | aa50   |
| .           | Full Stop                          | 2e     |
| 𐒠           | Osmanya Digit Zero                 | 104a0  |
| 𐴰           | Hanifi Rohingya Digit Zero         | 10d30  |
| ０          | Fullwidth Digit Zero               | ff10   |
| 𑃰           | Sora Sompeng Digit Zero            | 110f0  |
