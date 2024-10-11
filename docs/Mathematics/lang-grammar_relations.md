# Language: grammar relations

## Taxonomic

A taxonomic relation describes a hierarchical classification
where one term is a subtype or member of another term. For
example, "animal" is the taxonomic **hypernym** of "dog." The
complementary concept, **hyponym**, is a word whose definition
includes another one. These relationships are analogous to
`inheritance` in OOP.

$$X \subseteq Y$$

| Hypernym          | Co-hyponyms       |
| :---------------- | ----------------- |
| color             | red, green, blue  |
| celestial object  | sun, moon, star   |
| adjective         | brigh, loud, red  |


## Dependency

A dependency relation shows how one concept depends on another
for its definition. The object is defined in part by its
components. These relationships are analogous to `composition` in
OOP.

$$X \supseteq \{p_1, p_2, \ldots \}$$

> A sphere (hyponym) is an "orientable surface" (hypernym). A
> sphere (holonym) has a surface and an inside (meronyms).


## Associative

An associative relation exists between two words $x$ and $y$ when
there is a context $C$ that provides a meaningful connection
between them.

$$\begin{aligned}
g:(x,y) &\rightarrow C\\
g:(\text{doctor}, \text{hospital}) &\rightarrow \text{ healthcare}
\end{aligned}$$

All co-meronyms and co-hyponyms also exhibit an associative
relationship. Its common context is given by its hypernym or
holonym. However, the presence of an associative relationship
between two words does not necessarily imply a taxonomic or
dependent relationship. For example it can be argued that $g:
(\text{family}, \text{house}) \rightarrow C$. Yet each word has
its own definition that doesn't depend on the shared context $C$.


## Converseness (relational opposites)

Converseness occurs when two words describe the same relationship
from opposite perspectives. In other words, each word represents
a different role in the same situation or interaction.

$$\begin{aligned}
    \text{Linguistic Term 'converse'} &\cong \text{Mathematical Operator } \leftrightarrow \\
    P(x) &\leftrightarrow Q(y) \text{ represents a converse relationship} \\
    \text{child}(x)   &\leftrightarrow \text{parent}(y)   \text{ where } x \text{ is a child of } y \\
    \text{Hyponym}(x) &\leftrightarrow \text{Hypernym}(y) \text{ where } x \text{ is an instance of } y \\
    \text{Meronym}(x) &\leftrightarrow \text{Holonym}(y)  \text{ where } x \text{ is a part of } y \\
\end{aligned}$$

Using modal logic:

$$\begin{aligned}
    \text{Child} &\rightarrow \Box\text{Parent} \\
    \text{Hyponym} &\rightarrow \Box\text{Hypernym}
\end{aligned}$$


## Functional

Connections between two concepts where one concept invokes or
expects the existence of the other. They are directional and
dependent. Consider the following examples:

$$f: X \rightarrow {Y, \emptyset}$$

- A **question** seeks an **answer**. However, not al questions have
valid or clear answers without context. $f(question) = answer$,
where $f$ is a *partial function* that may return a valid answer
if the context allows.

- A **cause** brings about an **effect**. Some causes may have
predictable effects, while others might have multiple or
unforeseen outcomes.

- A **lock** functionally requires a **key** to perform its role
(locking/unlocking).

$$\begin{aligned}
    \text{Request}(x) &\rightarrow \diamond\text{Fulfillment}(y) \\
    \text{Stimulus}(x) &\rightarrow \diamond\text{Response}(y) \\
    \text{Question}(x) &\rightarrow \diamond\text{Answer}(y) \\
\end{aligned}$$


## NOTES

- Homonymy (equal) is co-hyponym of paronymy (similar).
- Antonymy (opposite) is the antonym of synonymy (equivalent)



