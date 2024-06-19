#obsidian To see how any formula was written in any question or answer, including this one, right-click on the expression and choose "Show Math As > TeX Commands". (When you do this, the '$' will not display. Make sure you add these: see the next point. There are also [other ways](https://math.meta.stackexchange.com/questions/659/how-to-view-latex-source-of-equations) to view the code for the formula or the whole post.)

1. **For inline formulas, enclose the formula in `$`…`$`. For displayed formulas, use `$$`…`$$`.**
	* These render differently. For example, type the following to show _inline_ mode:  
	* These render differently. For example, type the following to show _inline_ mode:  
		`$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$`
	$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$
	or type the following for display mode:  
	`$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$`$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$
2. For **Greek letters**, use `\alpha`, `\beta`, …, `\omega`: α, β, …, ω.
	* For uppercase letters, use `\Gamma`, `\Delta`, …, `\Omega`: Γ, Δ, …, Ω.
	* For other Greek capital letters, use Latin `$A,`, `B`, `E$` and so on: A,B,E.
	* Some Greek letters have variant forms: `\epsilon \varepsilon` ϵ, ε, `\phi \varphi` ϕ, φ, and others.
3. For **superscripts and subscripts**, use `^` and `_`. For example, `x_i^2`: x2i, `\log_2 x`: log2x.
4. **Groups**. Superscripts, subscripts, and other operations apply only to the next “group”. A “group” is either a single symbol, or any formula surrounded by curly braces `{`…`}`.
	* If you do `10^10`, you will get a surprise: 1010. But `10^{10}` gives what you probably wanted: 10[^10] .
	*  Use curly braces to delimit a formula to which a superscript or subscript applies: `x^5^6` is an error; `{x^y}^z` is xyz, and `x^{y^z}` is xyz. Observe the differences between `x_i^2` x2i, `x_{i^2}` xi2 and `{x_i}^2` xi2.
5. **Parentheses** Ordinary symbols `()[]` make parentheses and brackets ``(2+3)[4+4]``. Use `\{` and `\}` for curly braces {}.
	* These do _not_ scale with the formula in between, so if you write `(\frac{\sqrt x}{y^3})` the parentheses will be too small: (x√y3). Using `\left(`…`\right)` will make the sizes adjust automatically to the formula they enclose: 
	* \left(\frac{\sqrt x}{y^3}\right) is (x√y3).
		* $$\left(\frac{\sqrt x}{y^3}\right)$$
	* `\left` and`\right` apply to all the following sorts of parentheses: `(` and `)` (x), `[` and `]` [x], `\{` and `\}` {x}, `|` |x|, `\vert` |x|, `\Vert` ∥x∥, `\langle` and `\rangle` ⟨x⟩, `\lceil` and `\rceil` ⌈x⌉, and `\lfloor` and `\rfloor` ⌊x⌋. `\middle` can be used to add additional dividers. There are also invisible parentheses, denoted by `.`: use `\left.x^2\right\rvert_3^5 = 5^2-3^2` to get
		* $$\left.x^2\right\rvert_3^5 = 5^2-3^2`$$
6. **Sums and integrals** `\sum` and `\int`; the subscript is the lower limit and the superscript is the upper limit, so for example `\sum_1^n` ∑n1. Don't forget `{`…`}` if the limits are more than a single symbol. For example, `\sum_{i=0}^\infty i^2` is 
	$$\sum_{i=0}^\infty i^2$$
	* - Similarly, `\prod` ∏ `\int` ∫, `\bigcup` ⋃, `\bigcap` ⋂, `\iint` ∬, `\iiint` ∭, `\idotsint` ∫⋯∫.
7. **Fractions** There are [three ways to make fractions](https://math.meta.stackexchange.com/questions/12978/should-dfrac-be-edited-in). `\frac ab` applies to the next two groups, and produces ab; for more complicated numerators and denominators use `{`…`}`: `\frac{a+1}{b+1}` is a+1b+1
	- If the numerator and denominator are complicated, you may prefer `\over`, which splits up the group that it is in: `{a+1\over b+1}` is 
	- $${a+1\over b+1}$$
	- For continued fractions, [use `\cfrac` instead of `\frac`](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference/5058#5058).
8. **Radical signs / roots** Use `sqrt`, which adjusts to the size of its argument: `\sqrt{x^3}` x3−−√; `\sqrt[3]{\frac xy}` xy−−√3. For complicated expressions, consider using `{...}^{1/2}` instead.
9. Some **special functions** such as "lim", "sin", "max", "ln", and so on are normally set in roman font instead of italic font. Use `\lim`, `\sin`, etc. to make these: `\sin x` sinx, not `sin x` sinx. Use subscripts to attach a notation to `\lim`: `\lim_{x\to 0}`
	* $$\lim_{x\to 0}+\sin (x)$$
