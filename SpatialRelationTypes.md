#Spatial relations for LORE.

General comments: we understand "space" in a most general sense. It is not restricted to material objects; it includes all kinds of entities related by spatial predicates that are used in language, including fictional entities, information entities etc.

As long as these relation are asserted between non-processual (non-temporal) entities they are time-related. This is not made explicit in a binary Subject-Predicate-Object representation. The truth value of an expression like S ‘is part of’ O may be TRUE at t1 and FALSE at t2


# Spatial relations #

  * is part of
  * has part

  * is located in
  * is location of

  * is contained in
  * contains

  * is directly connected to

  * is connected to

  * is before
  * is after


# Definitions #

**Name:** is part of

**Definition:** For individual entities S and O, it holds that ‘S is part of O’, if and only if 1) S and O are within the same mereologically dimensioned area (like space, time, space-time, or any ordered space including abstract space like in information entities), 2) S is a part of O.

**Examples:** Crete is part of Europe, this morning is part of today, my skin is part of my body, this third chapter is part of this book.

**Problems:**
#‘is part of’ has a broader application compared to other mereological relation types like ‘is located in’, since it is also used for time. It is still left open whether we will distinguish this temporal meaning of ‘is part of’ by a different name.
#‘is part of’ in ordinary speech is often understood to exclude reflexivity

**Algebraic properties:** reflexive, transitive, Rule: if S is part of O and O is a spatial entity, then S is located in O, Inverse relation: 'has part'

**Alternative names:** is part of, part of



---

**Name:** has part

**Definition:** For individual entities S and O, it holds that ‘S has part O’, if and only if 1) S and O are within the same mereologically dimensioned area (like space, time, space-time, or any ordered space including abstract space like in information entities), 2) O is a part of S.

**Examples:** Europe has part Crete, today has part this morning, my body has part my skin, this book has part this third chapter.

**Problems:**
#‘has part’ has a broader application compared to other mereological relation types like ‘is location of’, since it is also used for time. It is still left open whether we will distinguish this temporal meaning of ‘has part’ by a different name.
#‘has part’ in ordinary speech is often understood to exclude reflexivity

**Algebraic properties:** reflexive, transitive, Rule: if S has part O and O is a spatial entity, then S is location of O, Inverse relation: 'is part of'

**Alternative names:** has part


---


**Name:** is located in

**Definition:** For particular entities S and O, it holds that ‘S is located in O’, if and only if 1) S and O are within the same spatially dimensioned area, 2) O has a (not necessarily convex) outside border or envelope and 3) the space occupied by S is part of the space occupied by the outside borders of O.

**Examples:** Pete is located in his car, Iceland is located in Europe.

**Problems:** the application of ‘is located in’ depends on the definition of the outside borders of O. If the beaches of La Palma define the outside borders of the Atlantic Ocean, then La Palma is not located in the Atlantic Ocean, otherwise it is. Somewhat counterintuitively, a wheel is located in a car and a chimney is located in a house.

**Algebraic properties:** reflexive, transitive, inverse relation 'is location of', Rule: if S is part of O and O is a spatial entity, then S is located in O

**Alternative names:** is in, has location, has as location, is located by


---


**Name:** is location of

**Definition:** For particular entities S and O, it holds that ‘S is location of O’, if and only if 1) S and O are within the same spatially dimensioned area, 2) S has a (not necessarily convex) outside border or envelope and 3) the space occupied by O is part of the space occupied by the outside borders of S.

**Examples:** Pete's car is location of Pete, Europe is location of Iceland.

**Problems:** the application of ‘is location of’ depends on the definition of the outside borders of S. If the beaches of La Palma define the outside borders of the Atlantic Ocean, then the Atlantic Ocean is not a location of La Palma, otherwise it is. Somewhat counterintuitively, a car is location of a wheel and a house is location of a chimney.

**Algebraic properties:** reflexive, transitive, inverse relation 'is located in', Rule: if S has part O and O is a spatial entity, then S is location of O

**Alternative names:** locates


---


**Name:** is contained in

**Definition:** For entities S and O, it holds that ‘S is contained in O’, if and only if 1) S and O are within the same spatially dimensioned area, 2) O has an associated container volume defined by the outside borders of O (like a convex envelope, or a convex envelope minus the volume of O) and 3) space occupied by S is part of the space occupied by the associated container volume of O.

**Examples:** some water is contained in a glass, La Palma is contained in the Atlantic Ocean. A wheel that is part of a car, and therefore located in that car, is not contained in the car.

**Problems:** the application of ‘is contained in’ depends on the definition of the associated container volume of O. This definition may often be very similar as the definition of the outside borders for ‘is located in’.

**Algebraic properties:** reflexive, transitive

**Inverse relation: 'contains'**

**Alternative names:...**


---


**Name:** contains

**Definition:** For entities S and O, it holds that ‘S contains O’, if and only if 1) S and O are within the same spatially dimensioned area, 2) S has an associated container volume defined by the outside borders of S (like a convex envelope, or a convex envelope minus the volume of S) and 3) space occupied by O is part of the space occupied by the associated container volume of S.

**Examples:** a glass contains some water, the Atlantic Ocean contains La Palma. A car that has part a wheel, and therefore is location of that wheel, does not contain the wheel.

**Problems:** the application of ‘is contained in’ depends on the definition of the associated container volume of S. This definition may often be very similar as the definition of the outside borders for ‘is location of’.

**Algebraic properties:** reflexive, transitive

**Inverse relation: 'is contained in'**

**Alternative names:...**


---


**Name:** is directly connected to

**Definition:** For entities S and O, it holds that ‘S is directly connected to O’, if and only if 1) S and O are components within the same network (abstract, spatial or mereological), consisting of components and connections between the components and 2) S and O share a connection

**Examples:** Germany is directly connected to France, Brussels Airport is directly connected to Vienna Airport, the paint is directly connected to the wall

**Problems:** The use of 'is directly connected to' depends on the precise definition of a network in which S and O are viewed as components. Entities may not be directly connected in reality, but they are directly connected on a network which is an abstraction of reality.
According to the characteristics of the network, entities can be connected to themselves.

**Algebraic properties:** symmetric, subtype of 'is connected to'


**Alternative names:...**


---


**Name:** is connected to

**Definition:** For entities S and O, it holds that ‘S is connected to O’, if and only if 1) S and O are components within the same network (abstract, spatial or mereological), consisting of components and connections between the components and 2) there is a series of connections and network components between S and O.

**Examples:** Germany is connected to Greece, Trondheim Airport is connected to Pago Pago International Airport, the wheel is connected to the steerwheel

**Problems:** The use of 'is connected to' depends on the precise definition of a network in which S and O are viewed as components. Australia and Canada, viewed as components in a network of roads, are not connected. Viewed in a network of harbours, they are. Entities that are not directly connected to anything else, are not connected to themselves, otherwise they are.

**Algebraic properties:** symmetric, transitive



---


**Name:** is before

**Definition:** For entities S and O, it holds that 'S is before O', if and only if 1) S and O are entities within the same 1-dimensional ordered space, including the time-axis and 2) S is ordered before O (where order goes from early to late, close to far, low to high, small to large and few to many)

**Examples:** World War I is before World War II, the runner that arrived first is before the runner that arrived second, 3 is before 5, on the trip from Paris to London, Calais is before Dover

**Problems:** The definition of the defined order may depend on a specific context, like in the trip from Paris to London.

**Algebraic properties:** transitive, inverse relation: is after


---


**Name:** is after

**Definition:** For entities S and O, it holds that 'S is after O', if and only if 1) S and O are entities within the same 1-dimensional ordered space, including the time-axis and 2) S is ordered after O (where order goes from early to late, close to far, low to high, small to large and few to many)

**Examples:** World War II is after World War I, the runner that arrived second is after the runner that arrived first, 5 is after 3, on the trip from Paris to London, Dover is after Calais

**Problems:** The definition of the defined order may depend on a specific context, like in the trip from Paris to London.

**Algebraic properties:** transitive, inverse relation: is before