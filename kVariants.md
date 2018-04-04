# Introduction
`kVariants.txt` is a tab separated file of CJK ideographs variants. Information 
was collected by looking up dictionary sources quoted by the Unihan Database.

# Format
The file is split into three columns:  
1. Source Ideograph  
2. Classification  
3. Destination Ideograph

There are five classifications, `wrong!`, `wrong`, `simp`, `old` and `=`.
- `wrong!`  
  Variants which are identified by their source dictionaries as incorrect
  forms of the destination character. Some dictionaries may refer to common
  systematic variants as errorenous forms; those variants are grouped into the
  `wrong` classification.

- `wrong`  
  Includes characters which one of the following:
  - systematic corruptions or variations of another character 
  - characters with non-unifiable structural differences, such as stretching of
    top 艹  
  - strict per-component transliterations of characters where the conventional
    transliteration is a single fused component
  - characters with alternate positional forms (艸 vs 艹)

- `simp`  
  The source ideograph is a simplified variant of the destination ideograph.
  Simplification may be an official simplification defined by the 《簡化字總表》,
  official and unofficial derived simplifications, or otherwise simplier forms in
  popular handwritten use. Characters which are used as both Simplified and 
  Traditional forms are excluded.

- `old`  
  Alternative shape-based transliterations of older scripts used by Han, such as
  Small Seal, "guwen 古文", etc.  Variants covered by the `wrong` classification  
  are excluded.

- `=`  
  Z-variants of existing characters, where they are unifiable and/or not readily
  distinguished by users of the Han script.

# License
Copyright (c) 2018 Henry Chan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
