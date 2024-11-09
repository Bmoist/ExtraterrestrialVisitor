# Extraterrestrial Visitor
(Microtone Navigator)


## Quickstart

```lisp
load "gec-cmp.sal"
play composition()
```



## Interactive Composition

```
play demo1(auto-harmonize: #f)
```





# Core Functions

## Composition Components:

The structure of our piece a ternary form with an intro and coda.

| Intro | A | B | A' | coda|

- Intro
  - `a-intro()`
- A section:
  - `a-sect-harmony()`
  - `a-sect-main-melody()`
- B section:
  - `b-harmony()`
  - `bseg-melody()`
- A' section
  - `ap-sect-harmony()`
  - `ap-sect-main-melody()`
- Coda
  - `a-intro()`



## Key Features

### From `crazy-chords.sal`

`interval-filter`

- receives two mathematical functions (sound) as input, then calculates whether the ratio at various time points between the two functions belongs to a predefined set of ratios.

- variant: `modified-intf-func`, which will insert horizontal lines at the filtered time points to make the consonance lasts longer

`insert-hold`

- inserts a horizontal line at input sound given insertion time and duration



### From `microtone.sal`

`vl-chords`

- perform voice leading analysis on a list of input chords, then connect the voices by pitch bend.





