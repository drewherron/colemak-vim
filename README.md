# Vimrc for Colemak
## HNEI Mod 

Colemak's great, but the main thing holding me back from switching over was having to use it with Vim. Losing the HJKL movement keys is kind of a deal-breaker, and if I have to choose between Colemak and Vim, I'm choosing Vim.

So here's a vim setup that fixes that issue.

### What's different:
#### The four direction keys are on h/n/e/i, in the same place as QWERTY's h/j/k/l
- N (shift + ↓) goes to next search match (replaces n)
- E (shift + ↑) goes to previous search match (replaces N)
- H and L (upper-case) are unchanged 

#### Insert mode is on the L key
- l to enter insert mode
- L to insert at beginning of line
 
#### End of word is on the K key
- k/K replaces e/E
- Previous word (B) and end word (K) are next to each other

#### Help is lower-case j
- This one doesn't make much sense, but it didn't make sense on K to begin with
- Just remember "help" in Norwegian is "hjelp"


I am providing this here as a vimrc file, but it's probably easier to just paste the following lines into your own vimrc.

```
nmap n j
nmap N n
nmap e k
nmap E N
nmap i l
nmap I L
nmap j K
nmap k e
nmap K E
nmap l i
nmap L I
```
