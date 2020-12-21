
<h1>Contents</h1>
<a href="#rec1_worse_is_better">Worse is Better</a>

<h2 id="rec1_worse_is_better">The Rise of Worse is Better</h2>
MIT/Stanford style of design:
- Must be *Correct* and *Consistent*.
- Must be *simple*. More important for the interface to be simple than the implementation.
- Must be as *complete* as possible. Simplicity isn't allowed to overly reduce completeness.

Worse-Is-Better philosophy: slightly different from above
- *Simplicity* is the most important consideration in a design. Implementation is more important than interface simplicity.
- Must be *correct*. Slightly less important than *simplicity*.
- Must not be *overly inconsistent*. Can be sacrificed for simplicity.
	- Better to drop parts that deal with uncommon circumstances than to break simplicity or consistency.
	- Can be sacrificed to achieve completeness if simplicity is retained. Especially worthless is consistency of interface.
- Must be as *complete* as possible. Can be sacrificed in favor of any other quality. 

Benefits of worse-is-better:
- Spread like a virus, get people hooked
- Lower uses' expectation
- Leave space for improvement, 50% right -> 100% right