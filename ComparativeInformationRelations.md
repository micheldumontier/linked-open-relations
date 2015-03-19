# Introduction #

A comparison of a certain quality of two particualrs results in an information about this comparison which can be assigned to the two compared objects with a binary Comparative Information Relation. These relations assign information (or hold) about the comparison of a quality (precisely their respective quality values) of two particulars. They can either represent the equality of individuals with regard to these values or their difference and further specify this inequality.

A generic comparative relation is _comp_(a, b, qa, qb, m, n, i=0) with a, b particulars with their associated qualities qa, qb and their values m of qa and n of qb, i is the upper limit of a "similarity-tolerance interval" (if not given it is 0).

The main problem remains to state in the descriptions of relations **what** exactly is compared, how the n-ary relational parts are decompose ("mapped") to associated components in a structured and reproducible way(_has qualifier_, _has value_, _related to_) and to specify meaningful names.


---


---


# Details #

## **equals** ##

**Complement**: unequals

**Axioms:**
  * specificly, relates the values of a certain quality of two particulars
    * hence, relates a specific quality of two particulars
      * hence, relates two particulars
        * hence, the domain and range are: (value region, quality, particular)/(value region, quality, particular)
  * **Algebraic properties:** transitive, reflexive, symmetric

**Definition:** The binary relation _equals_ holds iff two compared particulars are "equal". This equality can either be quantitative which is a numerical equality  or qualitative which is the categorial equality of the two particulars.

**Examples:**
  * equals(speed\_car1, speed\_car2)
  * equals(animal\_1, animal\_2) => (example which might be well defined in a given local context but must be disambiguated for global use)

**Issues:**
  * The meaning of the comparative results for all of these binary generic comparative relations for particulars can be exactly specified for most scale types (see details below) and is only an issue for certain categorial qualities (e.g. color).
  * The _main issue_ of all af these generic comparative relations is disambiguation of _what_ exactly is related to each otherm where not specified. Hence, the problem is **how** to define the exact **application** and give rules for that:
    * e.g. the quality which is compared when particulars are compared
    * local vs. global (semantic web) use. In a defined local scenario the context may clearly disambigute the related


---


## **unequals/ "different from"** ##

**Complement**: equals

**Axioms:**
  * domain/range considerations as for equals
  * **Algebraic properties:** intransitive, irreflexive, symmetric

**Definition:** Unequals is the complement of _equals_. The binary relation _unequals_ holds iff two compared particulars are "unequal" or "different".

**Examples:**
  * unequals(speed\_car1, speed\_car2)
  * unequals(animal\_1, animal\_2) => (example which might be well defined in a given local context but must be disambiguated for global use)


---


## **alike/ "similar to"** ##

**Superrelation:** unequals

**Axioms:**
  * tolerance intervall/ qualitative tolerance specified
  * **Algebraic properties:** intransitive, irreflexive (without equality), symmetric

**Definition:** The binary relation _alike_ holds iff two compared particulars are "similar" but not "equal" (or "too different"). The given definition might differ from common sense (or intuitive) usage of "similarity" which often includes "equality". The qualitative or quantitative similarity is usually defined as _unequality_ but "near to equality" with a given deviation (tolerance intervall, qualitative tolerance).

**Examples:**
  * alike(speed\_car1, speed\_car2)
  * alike(animal\_1, animal\_2) => (example which might be well defined in a given local context but must be disambiguated for global use)

**Issues:**
  * Besides the general considerations above (_equals_) the a further issue is, **how** and **where** to define the assumed tolerance interval which has been applied to derive the result of the comparison.



---


## **"larger than"** ##

**Superrelation:** unequals

**Inverse:** "smaller than"

**Axioms:**
  * Only defined for quantities and categorial qualities which can be ordered (-> quanitative quality on ordinal scale)
  * **Algebraic properties:** transitive, irreflexive, asymmetric

**Definition:** The binary relation _"larger than"_ holds iff two compared particulars are different so that the first particular is "larger" than the second particular. The qualitative or quantitative distance between the particulars is usually defined as numerical or qualitative difference. If this difference between the first and second particular is positive the relation holds for this pair.


**Synonyms:** dependent on the quality, e.g. before/ after (timepoints), shorter/ longer (durations), etc... (can be Subrelations dependent on domain [we can define domains](if.md))

**Examples:**
  * "larger than"(speed\_car1, speed\_car2)
  * "larger than"(animal\_1, animal\_2) => (example which might be well defined in a given local context but must be disambiguated for global use)

**Issues:**
  * For categorial qualities without ordering this relations are not defined.


---


## **"alike or equal"/ "larger than or equal"** ##

**provide a single section of each of these relations**

**Complement:** unlike/ "smaller than"
**Inverse:** none/ "smaller than or equal"

**Axioms:**
  * as specified for _alike_ and _"larger than"_
  * _alike_ OR _equals_
  * _"larger than"_ OR _equals_
  * **Algebraic properties:**
    * "alike or equal": intransitive, reflexive, symmetric
    * "larger than or equal": transitive, irreflexive, antisymmetric [domain/range: values] or asymmetric [domain/range: qualities, particulars]

**Definition:** These relations are intuitively defined as the disjunction of the _equals_ relations with on of the unequals relations _alike_ resp. _"larger than"_. They are used frequently but their algebraic properties render their application "dangerous" with the consequence of "unintended meaning".


---


---


#= Components =
#
#  **in relation to -> indicates the reference object / part / quality
#** has qualifier -> increased, decreased, etc.

# Background #

A prototypic n-ary comparative relation could be modelled as a re-ified comparison entity related with two (ordered) "ingoing" values, one optional upper bound of an tolerance interval, one qualitative quality and an optional quantitative quality (for the exact meaning of the parameters and qualities see below). To _directly_ "associate" the ingoing values of the compared entities with the comparison is a shortcut for convenience (Can we directly use "values" in an information object?). See the proposal for a ternary process model of comparison for a probably more correct ontological representation from Ward below. (Change in the direction of the two left branches with compared entities and apply "participation", but gain deeper indirection).

<img src='http://www.imbi.uni-freiburg.de/ontology/lore/comparison.png' width='80%'>

Now reduce, flatten and simplify this model and arrive at a pragmatic working model under the following assumptions: We are only interested in the same quality of the two compared particulars. The original values are not longer of interest (could be retrieved from the objects) and are already compared. The comparison result is known as qualitative value (set of values is given, names of "smaller/ larger" can change for different qualities, e.g. "earlier/ later", "before/ after") and were applicable as additional measurement (difference in ranks and on intervall/ ration scales and ratio on ratio scale). Vagueness/ tolerance of comparison can be specified (results in equal/ similar/ different).<br>
<br>
<img src='http://www.imbi.uni-freiburg.de/ontology/lore/comparison_reduced.png' width='50%'>

Now de-ify <i>Comparison</i>, and arrive at a reduced set of sound binary comparative relations :-) . If this "working model" is our agreement, we can define a schema how we derive binary relations. E.g. just use the values from <i>qual-res</i> and define: <i>equals</i>, <i>differs</i>, <i>alike</i>, <i>smaller</i>, <i>larger</i> over Thing:a, Thing:b and all sets of <i>qual</i> qualities were these relations can be meaningful defined either with or without tolerance interval. Where comparative terms with more specified quality definitions are availale corresponding relations definitions are easier: <i>before</i> and <i>after</i> over Perdurant:a Perdurant:b with Quality<-TimePoint:tpa and :tpb. For relations with numerical results or more complex domain and range restrictions components for a re-reification must be defined. For me, it is not so much a problem to define realtions but of communication to the users. How can we arrive at a description of relations that is easy to understand and to apply, covers nearly all interesting cases and is <b>unambiguous</b>.<br>
<br>
<h4>functional "definitions"</h4>

<ul><li>numerical comparison: <i>compn</i>(m, n)<br>
<blockquote>m, n are numbers on nomial, ordinal, interval, ratio scales. <i>compn</i> is one of: <i>equalsn, unequalsn</i> for all scale types of m, n with m=n for <i>equalsn</i> and m!=n for <i>unequalsn</i>. <i>unequalsn</i> is on of <i>larger thann/ smaller thann</i> for m, n on ordinal, inverall and ratio scales with m>n for <i>larger thann</i> and m<n for <i>smaller thann</i>. <i>difference ofn</i> is defined as quantification of inequality for intervall and ratio scales as |m-n| (and as <i>rank difference ofn</i> for ordinal scales), <i>ratio ofn</i> is only defined for ratio scales as m/n.</blockquote></li></ul>

<ul><li>numerical comparison: <i>compn</i>(m, n, i)<br>
<blockquote><i>aliken</i> is defined as <i>smaller thann</i>(<i>differencen</i>(n, m), i) with n, m on ordinal, intervall and ration scales and i an intervall width > 0 on ordinal, intervall and ratio scales. With i=0 (not given) <i>comp</i>(m, n)</blockquote></li></ul>


<ul><li>generic comparison: <i>comp</i>(a, b, qa, qb, m, n, i)<br>
<blockquote>For particulars a, b of generic type with qualities qa, qb having values (or regions) m of qa and n of qb, the following <i>comp</i> relations can be defined: <i>comp</i>(a, b, qa, qb, m, n, i) -> <i>compn</i>(m, n, i) for all comparisons on numeric values m, n, i (names of the relations of <i>compn</i> without postfix "n"). For comparisons on qualities with discrete qualitative values either a transformation on ordinal numerical scale is sufficient <b>or</b> the two relations <i>equals</i> and <i>alike</i> must be defined in terms of the specific qualities and their respective values.</blockquote></li></ul>

<ul><li>generic comparison with triangulation: <i>comp</i>(a, b, qa, qb, m, n, c, qc, p, i)<br>
<blockquote>[Don't know if we should follow this] For particulars, qualities and values (regions) as above the generic reference particular c with quality qc and its value p, the following <i>comp</i> relations can be defined:<br>
</blockquote></li></ul><blockquote><i>onesided</i> (<i>larger thann</i>(m, p) AND <i>larger thann</i>(n, p) OR <i>smaller thann</i>(m, p) AND <i>smaller thann</i>(n, p)), <i>twosided</i>(NOT <i>onesided</i>), <i>residual diff</i>(<i>differencen</i>(<i>differencen</i>(m,p), <i>differencen</i>(n, p)), residual ratio<i>(</i>ration<i>(</i>differencen<i>(m,p),</i>differencen<i>(n, p))</blockquote></i>

<h3>(non exhaustive) list of what should be covered by comparational relations</h3>

<ul><li>similarity/ equality vs. dissimilarity/ inequality<br>
</li><li>(quality of distinction (color, tone))<br>
</li><li>direction of difference (ordering)<br>
</li><li>(absolute) size of difference (magnitude, scale)<br>
</li><li>algebraic properties of differences (ratio is meaningful, scale, inversity, symmetry, reflexivity?, transitivity?)<br>
</li><li>intended precision of similarity (explicit vagueness)<br>
</li><li>relational system specified (normative element(s) stated)<br>
</li><li>etc.</li></ul>


<h1>Questions</h1>

<ul><li>Possibly, some of the information relations are (ternary) comparative: has_rank  is comparative. One can have only have a rank in comparison to other individuals (so this is the assignment of a number depending on the comparison)???</li></ul>

<h1>Examples</h1>

<ul><li>'is similar to'<br>
</li><li>'is different from'<br>
</li><li>'has high plasma membrane amount' / 'has low plasma membrane part'<br>
</li><li>'has high plasma membrane part' / 'has low plasma membrane amount'</li></ul>

<h1>n-ary relation model in OWL DL (proposal by Ward)</h1>

An OWL-expressible n-ary model is proposed, that can reify binary relation arcs (triples), that use level 1 comparative relations, as relational individual:<br>
<br>
In general:<br>
<ul><li>subject-individual 'is-level-1-compared-to' object-individual</li></ul>

<=><br>
<br>
<ul><li>subject-individual 'is subject of' relational-individual<br>
</li><li>object-individual 'is object of' relational-individual<br>
</li><li>relational-individual rdf:type owl:Thing<br>
</li><li>relational-individual rdf:type comparison<br>
</li><li>comparison rdf:type owl:Class</li></ul>


Consider two comparanda C1 and C2, which are particulars that are compared. Consider a particular quality Q1.<br>
<br>
E.g. C1 and C2 are stars (like Alfa Centauri and Sirius). Q1 is brightness magnitude.<br>
<ul><li>C1 is decreased in magnitude relative to C2</li></ul>

<=><br>
<br>
<ul><li>C1 'is subject of' individ_compar_123<br>
</li><li>C2 'is object of' individ_compar_123<br>
</li><li>individ_compar_123 rdf:type owl:Thing<br>
</li><li>individ_compar_123 rdf:type comparison<br>
</li><li>comparison rdf:type owl:Class<br>
</li><li>individ_compar_123 rdf:type numerical_comparison<br>
</li><li>individ_compar_123 rdf:type is_smaller_than_comparison<br>
</li><li>individ_compar_123 rdf:type ratio_10_intervalled_comparison<br>
</li><li>individ_compar_123 'is in relation to' Q1</li></ul>

This assumes the introduction of the following binary relations:<br>
<ul><li>is subject of (has subject)   (has subject is functional)<br>
</li><li>is object of (has object)   (has object is functional)<br>
</li><li>is in relation to (?) (maybe 'is bearer of'?)</li></ul>

The rest of the n-ary model can be created as classes, which is mostly outside the scope of LORE.<br>
<br>
Problem: this n-ary model may be valid OWL DL, but some important expressivity that can be applied to binary relations, cannot be applied to this model. In practical terms: quantification of class level relations: every dwarf star is decreased in magnitude relative to some red giant star. Also transitivity, chains and many other interesting things may only be assigned to level-1-relation.<br>
<br>
Possible solution: accept those level-1-relations for attaching algebraic properties that work in OWL, but provide LORE for definitions that are stricter than natural language.