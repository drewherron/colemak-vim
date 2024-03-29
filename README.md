# Vim for Colemak
## HNEI Mod 

Colemak's great, but the main thing holding me back from switching over was having to use it with Vim. Losing the HJKL movement keys was kind of a deal-breaker for me, so here's a Vim setup that fixes that issue.
<p align="center">
 <img src="https://raw.githubusercontent.com/drewherron/colemak-vim/main/colemak-vim-hnei.png" width="50%" height="50%">
 <br>
 (Click to enlarge)
 </p>

### What's different:
#### The four direction keys are on h/n/e/i, in the same place as QWERTY's h/j/k/l
- H is unchanged
- N (shift + ↓) goes to next search match (replaces n)
- E (shift + ↑) goes to previous search match (replaces N)
- I (shift + →) moves cursor to bottom of screen (same location as QWERTY, different letter)

#### Insert mode is on the L key
- l to enter insert mode
- L to insert at beginning of line
 
#### End of word is on the K key
- K/k replaces E/e
- Previous word (B) and end word (K) are next to each other

#### Help is on lower-case j
- This one doesn't make much sense, but it didn't make sense on K to begin with
- Just remember "help" in Norwegian is "hjelp"


I am providing this here as a vimrc file, but it's probably (definitely) easier to just paste the following lines into your own vimrc:

```
noremap n j
noremap N n
noremap e k
noremap E N
noremap i l
noremap I L
noremap j K
noremap k e
noremap K E
noremap l i
noremap L I
```
If you use Vimium in your browser, you can add these lines to your custom key mappings:
```
map n scrollDown
map N performFind
map e scrollUp
map E performBackwardsFind
map i scrollRight
map I goForward
map j showHelp
```

If I've made mistakes or if you can add any improvements, feel free to send in pull requests.
