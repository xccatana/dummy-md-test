## Dummy testing for markdown

[Source of inspiration](https://github.com/jeffreytse/jekyll-spaceship/blob/master/README.md)

#### Cell Markdown

Sometimes we may need some abundant content (e.g., mathjax, image, video) in Markdown table  
Therefore, here we also make markown syntax possible inside a cell.

```markdown
| :                   MathJax \|\| Image                 : |||
| :------------ | :-------- | :----------------------------- |
| Apple         | : Apple : | Apple                          \
| Banana        | Banana    | Banana                         \
| Orange        | Orange    | Orange                         |
| :     Rowspan is 4     : || :        How's it?           : |
| ^^     A. Peach          ||    1. ![example][cell-image]   |
| ^^     B. Orange         || ^^ 2. $I = \int \rho R^{2} dV$ |
| ^^     C. Banana         || **It's OK!**                   |

[cell-image]: https://jekyllrb.com/img/octojekyll.png "An exemplary image"
```
Test

|God's creatures||Devil's creatures|||
|:---:|---|:---:|---|---|
|Mom|Dad|Homer simpson|||
|Me||Bart|Lisa|Maggy|


Code above would be parsed as:

<table>
<thead>
<tr>
<th align="center" colspan="3">MathJax || Image
</tr>
</thead>
<tbody>
<tr>
<td align="left">Apple<br>Banana<br>Orange</td>
<td align="center">Apple<br>Banana<br>Orange</td>
<td align="left">Apple<br>Banana<br>Orange</td>
</tr>
<tr>
<td align="center" rowspan="4" colspan="2">
Rowspan is 4
<br>A. Peach
<br>B. Orange
<br>C. Banana
</td>
</tr>
<tr>
<td align="center">How's it?</td>
</tr>
<tr>
<td align="left">
<ol>
<li><img width="100" src="http://latex2png.com/pngs/82b913db54a9f303bed7197d11347d74.png"></img></li>
<li><img width="150" src="https://jekyllrb.com/img/octojekyll.png" title="An exemplary image"></img></li>
</ol>
</td>
</tr>
<tr>
<td align="left"><b>It' OK!</b></td>
</tr>
</tbody>
</table>
