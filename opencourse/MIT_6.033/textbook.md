<link rel="stylesheet" type="text/css" href="textbook.css">

# Contents
1. <a href="#1">Systems</a>
	1. <a href="#1.1">Systems and Complexity</a>
	2. <a href="#1.2">Sources of Complexity</a>

<h1 id="1">Systems</h1>
<h2 id="1.1">Systems and Complexity</h2>
Common Problems of Systems in Many fields
- emergent properties
	Only occurs after combining components into a system. Careful prior analysis may not help.
- Propagation of effects
	An important requirement in most system designs is to limit the impact of failures.
	There are no small changes in a large system.
- incommensurate scaling
	Different parts of the system exhibt different orders of growth.
- trade-off
	Push down on one problem, cause another problem to pop up somewhere else.

It's difficult to describe a constructive theory for computer systems, so the author use case theories to convey numerous design principles.

System: a set of interconnected components that has an expected behavior observed at the interface with its environment.
Environment: all except those belonging to a certain system
Component: defined with purpose and granularity

**Complexity**
- Large number of components
- Large number of interconnections
- Many irregularities
- A long description
- A team of designers, implementers, or maintainers

<h2 id="1.2">Sources of Complexity</h2>

1. Cascading and interacting requirements
<div class="principle">
Principle of escalating complexity: adding a requirement increases complexity out of proportion
</div>
**Generality**: meeting many requirements with a single design.
<div class="principle">
Avoid excessive generality: if it's good for everything, it's good for nothing.
</div>

2. Maintaining High Utilization
<div class="principle">
The law of diminishing returns: the more one improves some measure of goodness, the more effort the next improvement would require
</div>

<h2 id="1.3">Coping with Complexity</h2>

1. Modularity

<div class="principle">
The unyielding foundations rule: it is easier to change a module than to change the modularity
</div>

Changing an interface would lead to change in all connected modules; thus it's easier to change the internal implementation.