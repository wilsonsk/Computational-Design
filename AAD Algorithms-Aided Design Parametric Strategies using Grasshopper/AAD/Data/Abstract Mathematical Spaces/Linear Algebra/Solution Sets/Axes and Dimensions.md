# Axes and Dimensions
##### Axis
An **axis** is an independent **set of possible values** corresponding to a variable or coordinate in a space, where each value in this set represents a potential position or state (of being) corresponding to a single type of variation (i.e. **axis or dimension**).
##### Dimension
Is an independent type of set of possible values, or type of variation. 
	I.e. A **dimension** is an abstract concept representing a distinct, independent **degree of freedom** or **variable of variation** within a system or set.
		 It refers to the number of independent parameters or factors needed to uniquely describe elements or states within that system.
			Each dimension describes a specific aspect or characteristic of the system that can change without influencing other dimensions.

In set theory, dimension can be interpreted as the **cardinality** of the set of independent variables or parameters needed to describe the system. 
	For instance, in a vector space, the number of vectors required to span the entire space (the **basis vectors**) represents the number of dimensions.
	
The axis provides one **degree of freedom** in which values can vary, and it is typically **unconstrained** unless a relationship or constraint is imposed upon it.
##### Variable 
A **variable** is a **symbol** or **placeholder** that represents an unknown or changing **quantity** within a set of possible values.
	A **variable** represents the **instance** of that dimension's possible values. 
		For instance, the variable $x$ refers to a specific point or value within the set of all possible $x$-values in the $x$-dimension.

Both **dimensions** and **variables** define **types of sets** of possible values, where each dimension or variable corresponds to a specific **type** or **aspect** of variation within the space or system
## Starting at Universal Superset (Set of all Real Numbers $\mathbb{R}$)
Before there are axes or dimensions there is simply the [[Abstract Mathematical Spaces#The Universal Superset as the Most Fundamental Mathematical Object|Universal Superset]].
	Which encompasses every possible number, whether positive, negative, rational, irrational, or infinite.
		It represents a space of **total freedom** where no values are excluded or constrained. Every possible value is included in this universal set.

- - - 
## Constraints
**Constraints** (whether in the form of inequalities or equations) simply **restrict** or **structure** the relationships between the values on these axes, but they do not force the axes to behave like domains or codomains.
	Instead, they just define **how values can interact** within the space.
### Constraining the $\mathbb{R}^1$ (i.e. $x$-axis) Internal vs. External/Expansive
#### Internal Constraints (Constraining within a Space) are Limiting
In formal terms, these types of constraints are often referred to as **subsets** or **restricted subsets** within a space.
	  They describe a smaller set of allowable values within the original set.
 
**Internal constraints** are those that apply **within a set or space**, typically through the use of **equations** or **inequalities** that restrict the set of possible values on an axis (or axes). 
	In $\mathbb{R}^1$, for example, an internal constraint limits the possible values of xxx within the one-dimensional space.
		They reduce the number of possible values by applying equations or inequalities that restrict the range of valid values within the given space.
			These constraints make subsets within the original space.
##### Equations as Constraints
###### in $\mathbb{R}^1$ Constrain the Possible Values of $x$
An equation like $x^2−4=0$ constrains $x$ to the specific values where the equation holds true, i.e., $x = \pm 2$.
	 This means we are still working within $\mathbb{R}^1$, but we’ve **internally constrained** the values of xxx to just $\{-2, 2\}$.
		 If the constraint is an equation (like $x=2$), we often talk about a **solution set** or a **locus** of points that satisfy the equation. 
			 If the constraint is an inequality, we speak of **intervals** or **regions** that satisfy the inequality.
###### Equations in $\mathbb{R}^1$ Constrain the Possible Values of $x$ to a Single Value
In the context of equations, the set of solutions to an equation is often called the **solution set** or **locus** (the set of all points satisfying the equation).
	In $\mathbb{R}^1$, this solution set contains a single value as an element.
		This is because **Equations** specify exact values where the condition is met.
##### Inequalities as Constraints
###### in $\mathbb{R}^1$ Constrain the Possible Values of $x$
An inequality like $\LARGE 0 \le x \le 10$ restricts the set of possible values of $x$ within $\mathbb{R}^1$ to an **interval**.
	Again, this is an **internal constraint** that limits the values on the x-axis but doesn’t move us out of the space $\mathbb{R}^1$.
###### Inequalities in $\mathbb{R}^1$ Constrain the Possible Values of $x$ to a Interval
That is a solution set containing elements sequenced by an interval.
###### Interval 
Is a **set of values** between two endpoints, where the interval can be either **open**, **closed**, or **half-open/half-closed** depending on whether the endpoints are included.
###### Bounds
**Bounds** refer to the **minimum and maximum limits** of a set of values. 
	In the case of an interval like $0 < x < 10$, the bounds refer to the endpoints, but the critical point is whether or not those endpoints are **included**.
###### Types of Intervals
**Open interval**:  The endpoints (i.e. bounds) are **not included**.
$$\LARGE (a,b) \quad \text{where}\quad a < x < b$$
**Closed interval**: The endpoints (i.e. bounds) are **included**.
$$\LARGE [a,b] \quad \text{where} \quad a \leq x \leq b$$
**Half-open interval**: Only one of the endpoints (i.e. bounds) is included.
$$\LARGE [a,b) \text{ or } (a,b]$$
##### Functions as Constraints
###### Constrain the Set of Possible Values (i.e. Axis) to a Range
Assuming the Function is not a [[Mapping#A Transformation as a Subset of Multi-Variable Composite Functions Composite Functions ($1 1$, $m 1$)|transformation]], the Codomain is then the same "set" or "space" as the Domain. 
	I.e. The function transforms the input values from the domain into values that lie **within** the codomain.
###### Codomain
The codomain is the set of **possible output values** that the function can map to.

However, the functions still constrains the Domain to a specific subset of possible values **within** this Domain (and thus set of potential values) called the **range**.
###### Range
Refers to the **set of possible output values** of a function or system. 
	When you're discussing the **range** in the context of a function, it refers to the **values that the function produces**.
		Again, if the functions is **not a transformation**, then the Codomain and thus the Range are subsets of and within the Domain. 
#### External Constraints Extend A Set or Space
##### Dimension Extension (Common Term)
**External constraints** refer to the process of **expanding a space** by introducing **[[Abstract Mathematical Spaces#The Additional Structure|additional new structure]]** (such as a new axis) which adds **extra degrees of freedom** or **additional axes** (i.e. sets of possible values), which creates a higher-dimensional space where each axis corresponds to a new **set of possible values**. 
	This process is often called **dimension extension** or **embedding**.
		These new axes allow for **greater flexibility** in describing positions or relationships, effectively moving from a lower-dimensional space (like $\mathbb{R}^1$) to a higher-dimensional space (like $\mathbb{R}^2$ or $\mathbb{R}^3$).
			It is not constraining the values in the traditional sense; you’re **expanding** the system to accommodate new dimensions of freedom.
				These constraints add new possibilities, leading to more complex structures, not less.
					In this process, the original space is preserved along the new axes, meaning points from the lower-dimensional space remain valid in the new, higher-dimensional space.
##### Cartesian Product Extension (Formal Term)
In formal set-theoretic terms, **Cartesian product extension** is another way to describe the process of adding new axes or dimensions to a space. When you extend from R1\mathbb{R}^1R1 to R2\mathbb{R}^2R2, you are effectively taking the **Cartesian product** of R1\mathbb{R}^1R1 with another copy of R\mathbb{R}R (the new axis).

- For example, R2\mathbb{R}^2R2 can be seen as R×R\mathbb{R} \times \mathbb{R}R×R, which is the Cartesian product of two sets of real numbers, one for each axis.
    
- Similarly, R3=R×R×R\mathbb{R}^3 = \mathbb{R} \times \mathbb{R} \times \mathbb{R}R3=R×R×R is the Cartesian product of three sets of real numbers, representing the x-axis, y-axis, and z-axis.
- R1 is the set of all real numbers (points on a line),
- R2\mathbb{R}^2R2 is the Cartesian product of two sets of real numbers (points in a plane),
- R3\mathbb{R}^3R3 is the Cartesian product of three sets of real numbers (points in three-dimensional space).

In this sense, the **new axes** that are added correspond to **additional sets of possible values** being combined through the Cartesian product, which produces a higher-dimensional space.

###### Examples
- **Expanding from R1\mathbb{R}^1R1 to R2\mathbb{R}^2R2**:
    - Introducing a second variable, say yyy, creates a new axis, and the set of possible values is no longer constrained to just the x-axis. Now, we have the **x-axis** and the **y-axis**, and each point is described by a pair of values (x,y)(x, y)(x,y).
    - This transformation isn’t just a constraint on the x-values; it’s the introduction of a **new dimension** of freedom, resulting in a space where both the x-values and y-values can vary independently.
- **Expanding from R2\mathbb{R}^2R2 to R3\mathbb{R}^3R3**:
    - Similarly, moving from R2\mathbb{R}^2R2 (a plane) to R3\mathbb{R}^3R3 (a 3D space) involves the introduction of a third axis (the z-axis). This adds a third degree of freedom and allows us to describe points in a three-dimensional space using triples (x,y,z)(x, y, z)(x,y,z).
###### Terminology
The process of moving to a higher-dimensional space by introducing additional degrees of freedom is often described as **embedding** or **expanding** the space. 
	The term **dimension extension** is also used to describe this shift from a lower-dimensional space (like R1\mathbb{R}^1R1) to a higher-dimensional space (like R2\mathbb{R}^2R2 or R3\mathbb{R}^3R3).
    
**Embedding** specifically refers to placing one space (like R1\mathbb{R}^1R1) into a higher-dimensional space (like R2\mathbb{R}^2R2) in a way that preserves the structure of the original space while adding more dimensions.

- - - 
### The First Constraint (Producing the First Axis, $\mathbb{R}^1$ (Sub)Set)
An Axis is simply a [[Abstract Mathematical Spaces#The Universal Superset as the Most Fundamental Mathematical Object|Subset]] of some lower level Set which itself can be derived back to the initial and "singular", Parent Superset (i.e. absolute).

A **constraint** in the form of an **[[Abstract Mathematical Spaces#Equality (and thus Inequality) as the Most Fundamental Notion $ LARGE (=)$|inequality]]** applied to the Universal Superset is what **restricts** or **filters** this vast set, creating a **subset** of possible values.
	This subset is called **$\mathbb{R}^1$** is the set of all real numbers along a single axis, commonly called the $x$-axis.
		This subset is (or corresponds to) a single axis, in this case, called the $x$-axis.
			It is an **independent set** of **possible values** in this $\mathbb{R}^1$ set.
				Any value in the set $\mathbb{R}^1$ can be represented by a variable $x$.
###### Elements of $\mathbb{R}^1$: Individual real numbers $\LARGE x \in \mathbb{R}$.
Where $x$ represents a possible, single value in the $x$-axis/set of $\mathbb{R}^1$.
	In $\mathbb{R}^1$ if the possible value of $x$ on the axis (or in the set of possible values) is not constrained by an equation (and thus can be any element in the axis/set of $\mathbb{R}^1$), then it has $1$ degree of freedom.
		This axis or set of possible values directly corresponds to a **[[Degrees of Freedom|degree of freedom]]**.
			In **$\mathbb{R}^1$**, there is only **one degree of freedom** (one axis), so any point is defined by a single value.


### The Second Constraint (Producing the Second Axis (i.e. 2-Axis space), $\mathbb{R}^2$ (Sub)Set/Space)

#### Forming R2\mathbb{R}^2R2 Through the Cartesian Product

##### Understanding the Cartesian Product

- **Definition**: The **Cartesian product** of two sets XXX and YYY is the set of all ordered pairs (x,y)(x, y)(x,y) where x∈Xx \in Xx∈X and y∈Yy \in Yy∈Y.
- **Mathematical Representation**: R2=X×Y={(x,y)∣x∈R,y∈R}\mathbb{R}^2 = X \times Y = \{ (x, y) \mid x \in \mathbb{R}, y \in \mathbb{R} \}R2=X×Y={(x,y)∣x∈R,y∈R}.

##### Combining Axes to Form R2\mathbb{R}^2R2

- **Elements of R2\mathbb{R}^2R2**: Ordered pairs (x,y)(x, y)(x,y) where both xxx and yyy are real numbers.
- **Visualization**: A plane where each point is determined by a pair of real numbers, one from the xxx-axis and one from the yyy-axis.
#### Formal Set-Theoretic Explanation

##### Sets Involved
- **Set XXX**: The set of all real numbers along the xxx-axis, X=RX = \mathbb{R}X=R.
- **Set YYY**: The set of all real numbers along the yyy-axis, Y=RY = \mathbb{R}Y=R.
##### Cartesian Product
- **Definition**: R2=X×Y={(x,y)∣x∈X,y∈Y}\mathbb{R}^2 = X \times Y = \{ (x, y) \mid x \in X, y \in Y \}R2=X×Y={(x,y)∣x∈X,y∈Y}.

#### **Elements of R2\mathbb{R}^2R2**

- **Ordered Pairs**: Each element is a pair (x,y)(x, y)(x,y), not just individual numbers.
- **Distinct from Elements of R1\mathbb{R}^1R1**: The elements xxx and yyy are individual real numbers, but (x,y)(x, y)(x,y) is a single element in R2\mathbb{R}^2R2.
#### How the New Axis Is Added to the Structured Set

##### Understanding Sets and Elements

- **Original Set (R1\mathbb{R}^1R1)**:
    - **Elements**: Real numbers xxx.
    - **Structured Set**: The xxx-axis.
- **New Axis (yyy-Axis)**:
    - **Elements**: Real numbers yyy.
    - **Structured Set**: The yyy-axis.

#### **Combining Elements to Form R2\mathbb{R}^2R2**

- **Process**:
    1. **Pairing Elements**: For each element xxx in R1\mathbb{R}^1R1, we pair it with every element yyy in the yyy-axis set.
    2. **Creating Ordered Pairs**: Each combination (x,y)(x, y)(x,y) becomes an element of R2\mathbb{R}^2R2.
- **Result**: The set R2\mathbb{R}^2R2 consists of all possible ordered pairs formed from elements of R1\mathbb{R}^1R1 and the yyy-axis.
#### Introducing a New Axis: The yyy-Axis

##### **Defining the yyy-Axis**
- **yyy-Axis as a Set**: Another copy of the real numbers, Y=RY = \mathbb{R}Y=R.
- **Elements of YYY**: Individual real numbers y∈Ry \in \mathbb{R}y∈R.
- **Visualization**: A line perpendicular to the xxx-axis, extending infinitely in both directions.
- - -
## [[Abstract Mathematical Spaces#Change/Differentiation Through Constraint as the Foundational Notion|Change/Differentiation Through Constraint as the Foundational Notion]]
Change is differentiation.
	The initial change is that from the undifferentiated, absolute to the first duality or relational existence of two interdependent states. 
		The states being most simply "**is**" and "**is not**", that is "**equality**" and "**inequality**".
			Which through the notion of value expressed as quantity which is expresses as numbers, can be described as $\LARGE 1$ and $\LARGE 0$.
### Change/Constraint Described by Equality/Inequality Derives Identity (i.e. Interdependent States of Being/Not Being)
The assignment of a value is dependent on a the notion of **equality** and thus **inequality**.
	Which define states of "being".
		But this **state of being** is implicitly and necessarily defined relative to a **state of not being.**
			These interdependent States of Being/Not Being are what produce Identity.
				That is a distinct entity, i.e. the differentiation between entities (i.e. states of being).
#### Equality/Inequality Establish a State of Being
This **state of being** is Interdependent with its corresponding state of what it is not.
	I.e. This **state of being** is implicitly and necessarily defined relative to a **state of not being.**

Equality establishes the identity between objects. When we say $a=b$, we assert that $a$ and $b$ are the same in all relevant aspects.

An axis is a **conceptual dimension**, where the "value" along the axis corresponds to a **state** or outcome of a system. 
##### Interdependent State of Being/Not Being Express an Identity
These interdependent States of Being/Not Being are what describe Identity.
	That is a distinct entity, i.e. the differentiation between entities (i.e. states of being).

- - -
## Identity: Values, Quantities, and Numbers
### Identity
A state of being defined by differentiation.
	That differentiation is described by set of characteristic(s) or property/properties that make an object or entity distinct from others.
#### Relational Identity
##### Identity Is Relational
Philosophically, an object's identity can be understood not only by its intrinsic properties but also by how it relates to other objects.
	See [[Abstract Mathematical Spaces#Equality (and thus Inequality) as the Most Fundamental Notion $ LARGE (=)$|how equality is the basis of defining something, but implicitly defines this something relative to what it is not (i.e. inequality)]].
		- **Equality Involves Comparison**: Equality is about determining whether two entities are the same in some respect.
		- **[[#Value|Qualities as Basis for Equality]]**: To assess equality, we often compare the **qualities** or **properties** of the entities involved.
###### Values as Identifiers (i.e. Representation of Properties/Qualities/Attributes)
- **Relative Existence**: The identity of an object emerges from the values of its attributes/properties/qualities in relation to others.
	- **Example**: A color may be perceived differently depending on surrounding colors, with its value defined relative to others.
#### Symbolic Representation
##### Values as Symbols
- **Abstract Representation**: Values symbolize the properties of objects, allowing us to manipulate and understand complex concepts.        
- **Communication of Identity**: By expressing values, we convey information about an object's identity.
### Value
is the an identifying characteristic that defines an entity and thus differentiates it from another.
	In mathematics and broader contexts, a **value** is a numerical or qualitative measure assigned to a variable, object, or concept. 
		It represents a specific magnitude (i.e. quantity or attribute) that characterizes something.
#### Relative Identity
An object's identity can be understood in relation to others through the values of its attributes.
#### Role of Values in Identity
- **Uniqueness**: Values help define the unique properties of an object.
- **Comparison**: By comparing values, we can differentiate one object from another.
#### Values Describing Identity Relative to Others
##### Relative Comparison
###### Values Enable Differentiation
Values allow us to compare and contrast objects based on their properties.
- **Example**: If one car has a speed of 60 mph and another 80 mph, the speed value differentiates the two cars.
#### Values in Defining Relationships
##### Establishing Relationships
###### Ratios and Proportions
- **Example**: If two ingredients are mixed in a ratio of 2:1, the values describe the relationship between the quantities used.
###### Equations and Inequalities
- **Equality ($=$)**: States that two values are identical, establishing a direct relationship.
- **Inequality ($\ne, <, >$)**: Indicates how values differ, defining the relative identities.
##### Identity Through Difference
###### Understanding Differences
- **Value Difference**: The difference between values quantifies how one object relates to another.	
	- **Example**: A building 100 meters tall is twice as tall as one that is 50 meters, with the height value defining this relationship.
###### Contextual Identity
- **Role and Function**: An object's identity may depend on its value relative to others in a system.
	- **Example**: In a network, a node's value (like bandwidth capacity) determines its role relative to other nodes.

- - -
### Quantity
Quantity is a value of magnitude that exists relative to and within an implicitly sequenced set.
	Therefore, Quantity is a magnitude value describes **relational differentiation** within a sequence.

At its most abstract, **quantity** can be seen as a fundamental concept that inherently involves **relational differentiation**—in other words, any notion of quantity must be understood **relative** to another quantity. 
	This **relative nature** leads to the idea of **sequenced sets**. 
		Sequenced sets naturally lead to the idea of **location** or **position**, which in turn implies the existence of a **plane or space**.
#### Quantity as a Fundamental Form of Relational Differentiation
At its core, **quantity** is not just an isolated value but something that exists **in relation** to other quantities.
	A number like "2" only has meaning when it's understood in relation to "1" or "3." 
		The act of **assigning a quantity** involves **differentiating** that quantity from others.
			For example, when we say there are **2** apples, we mean that **2** is the **difference** between having **1 apple** or **3 apples**. 
				**2** does not exist on its own; it exists **relative** to other quantities.

This idea of **relational differentiation** between quantities is what gives rise to **sequence**. If one quantity is understood relative to another, then you automatically have a **series** or **sequence** of values: for instance, 1, 2, 3, 4,..., each differing from the previous one.
#### Quantity Facilitates the Notion of Sequenced Sets and Order
##### Order Refers to the Arrangement or **Sequence** of Elements in a **Set**
It is based on the **relative relationships** between the elements rather than their **physical placement** in space.
- **Order** tells us **which element comes before or after** another in a sequence.
- For example, in the set of **natural numbers** {1,2,3,4,… }\{1, 2, 3, 4, \dots \}{1,2,3,4,…}, the **order** is what determines that **1 comes before 2**, and **2 comes before 3**.

In this way, **order** is abstract and relies on the **relation between elements** in a sequence. 
	**It can exist without any sense of spatial dimensions**.
		 You can think of order in **temporal** or **logical** sequences as well, such as steps in a process or events in time.
			**2** is greater than **1**, and **3** is greater than **2**, but this only reflects their **place in the sequence**.
				This sense of **before** and **after** in a sequence gives rise to the idea of **ordering**, but it does not imply a specific **position in space**.

Because quantity is always understood in **relation** to other quantities, we naturally group quantities into **sets** where each value in the set is **sequenced** relative to others. 
	This creates an ordered set of values.
		For example, the **natural numbers** $\{1, 2, 3, 4, \dots\}$ are a **sequenced set**. 
			Each number is distinct because of its **order** in the sequence — $2$ follows $1$, and precedes $3$, and so on.
#### Position Requires a Sequence with a Spatial Component (i.e. a "plane" or "space").
**Order** is not the same as **position**.
	**Position** implies "spatiality".
#### Quantities Can Represent Qualities (i.e. attributes/properties)
By mapping (i.e. assigning/corresponding) a quality to a quantity, qualities can then be described simply by a quantity (i.e. a numerical value).
##### Distinguish Between Entities
Quantity allows us to tell things apart based on "how much" or "how many."
- **Example**: If you have **3 apples** and someone else has **5 apples**, the quantities **3** and **5** differentiate the two collections.
##### Compare and Contrast
Quantities enable us to compare different entities numerically, providing a clear metric for difference.
- **Example**: Understanding that **5** is greater than **3** allows us to comprehend that one collection is larger than the other.
##### Measure Magnitude
Quantities give us a way to measure the magnitude of things, from physical dimensions to abstract concepts.
- **Example**: Measuring lengths in meters or weights in kilograms quantifies physical properties, differentiating them by magnitude.
##### Sequenced Sets Give **Potential** for Location or Position
Once you have a **sequenced set** (a structured collection of quantities), each quantity in the set has an implicit **location** or **position** relative to the others. 
	In other words, each quantity **occupies a specific position** in the sequence.
		For example, in the set {1,2,3,4}\{1, 2, 3, 4\}{1,2,3,4}, the number **3** has a clear **position**: it is **after 2** and **before 4**. Its **location** is defined by its place in the sequence.
			This concept of **location** or **position** in a sequence naturally leads to the idea of a **coordinate**—each quantity can be thought of as having a **coordinate** that places it within the sequence.

- - -
### Numbers
At the most abstract level, **numbers** are not just isolated quantities — they are **relational differentiators** that mark **positions** in a **sequence**.
#### Numbers are Abstract Representations of Quantity
At the most abstract level, **numbers** represent **quantities** by expressing the **difference** or **relation** between elements in a set or system.
	**Numbers don’t just exist in isolation**; they only have meaning because they differentiate one quantity from another. 
		For example, the number **2** is understood by how it differs from **1** and how it relates to **3**.
		    In this sense, a number is a **symbol** that represents **where** a quantity stands in relation to others, whether in a **sequence** or in **comparison** (greater, less, equal).

This relational differentiation is what gives numbers their power as representations of quantity. 
	They allow us to describe not just amounts, but how amounts are **related** to one another.
#### Numbers as Encoded Order and Sequence
##### Numbers Inherently Represent a Sequence
That is, an ordered structure, where each number has a place relative to others.
	For instance, the natural numbers (1, 2, 3,...) form a **sequence** where each number follows a defined order. 
		This sequencing is crucial for describing not just the amount of something but also the **relationship between things**.

Numbers inherently represent **order** and **sequence**. 
	When we think of numbers in this way:
		**Quantity** facilitates the creation of a **sequence** or ordered set of values.
			 Numbers are the **symbols** that allow us to encode this order.
				  For example, the number **3** doesn’t just represent "three things"; it represents the position in a sequence after **2** and before **4**.
    
Numbers are **abstract markers** that represent a **point** in a sequence or order.
	The number **3** could represent a step in a process, a moment in time, or a value in a sequence of quantities. 
		It encodes the idea of **progression** and **position** in an ordered structure.

This abstraction is crucial because it allows numbers to represent **quantity** not just as a count or measurement, but as part of a broader **system of order**.
#### Numbers and the Concept of Space
Numbers give rise to the concept of **space** because they allow us to describe **positions** and **relationships** between different points in a structured framework. 
	In the context of a **coordinate system**:
		Numbers allow us to define a point’s **location** relative to an origin or reference point (e.g., (x,y)(x, y)(x,y)).
		Numbers represent the **distance** or **difference** between points, giving us the ability to measure **relationships** in space.
#### Addition and Subtraction: Moving Through the Sequence
Numbers facilitate and describe sequenced quantities, but also facilitate the operation of addition which enables the descriptions of how a value relates to another by way of equalities and inequalities. 

Addition allows us to describe how numbers **relate to one another** by **moving through the sequence**:
- **Addition** tells us how to move **forward** through the sequence: 2+1=32 + 1 = 32+1=3 means we move one step forward to the next number.
- **Subtraction** tells us how to move **backward**: 3−1=23 - 1 = 23−1=2 means we move one step back to the previous number.

This relational movement through the sequence of numbers is crucial to understanding how quantities are **differentiated** and connected.
	Each number represents a step, and **addition** and **subtraction** describe how we move between these steps.
#### Numbers as Abstract Containers of Meaning (i.e. symbols mapping to meaning)
At the highest level of abstraction, **numbers** are not merely representations of **how many** but are **containers of meaning** that allow us to encode the **structure of relationships** and **positions** within a system:
	**$1$** doesn’t just represent a single unit; it represents the **first order** in a sequence, the **identity element** in multiplication, or the **scale factor** in transformations.
		**$0$** is more than just "nothing"; it represents a **neutral position** or the **origin** in a coordinate system, a point of reference from which other numbers are measured.
#### Why Numbers are so Fundamental to Understanding Reality 
The reason **numbers** are so central to humanity’s understanding of reality is that **reality itself is structured in terms of space (i.e. sequence with a spatial component), and logic (i.e. sequence, and causality)**. 
	Everything we observe and experience involves relationships between objects, events, and quantities. Numbers allow us to:
		- **Describe** these relationships precisely (e.g., the position of an object, the distance between two points, or the amount of energy in a system),
		- **Measure** change and structure (e.g., the passage of time, the arrangement of objects in space),
		- **Organize** our thoughts and understanding of the world through logical sequences (e.g., chains of cause and effect, scientific models, mathematical proofs).

Numbers are inherent in our pursuit of understanding because they provide a **formal system** for representing the patterns and structures we observe in reality.
	**Space**, for example, is defined by positions (which we represent with numbers), and **time** is understood through sequences of events (which are also modeled numerically).
##### Numbers as Representing Order -> Sequence -> Position/Location -> Space
The physical world we inhabit is fundamentally a **spatial structure**—it’s made up of objects with positions and locations relative to each other.
	These positions are described in terms of **coordinates** (numbers) that place each object within the framework of space.

The notion of Quantity derives the hierarchy of Order -> Sequence -> Position/Location -> Space.
	Therefore, Numbers through their inherent expression as a code of symbols (i.e. symbols mapping to meaning), can be employed to represent this fundamental notion of Order -> Sequence -> Position/Location -> Space.
		Where Space is sequence with a spatial component.

This is why Numbers are inherent in humanity's endeavor to understand reality. 
	Because our reality is understood through its inherent "space" (i.e. position/location/sequence).
##### Numbers as Representing Time (i.e. Change: "Before" and "After) 
Because Numbers represent order and sequence, the notion of "before" and "after" can be derived.
	**Time** is also a type of space, but for **events**. 
		Numbers allow us to describe the **sequence of events**—the order in which things happen and how they are causally related.
			 This connection between sequence and time forms the basis for our understanding of **causality**.
##### Numbers Through Representing Quantity, Facilitate Logic
Our logic used to understand our reality space is dependent on sequence.
	Humans define Logic as a sequence of events that we call causality.

**Causality** is a sequence of events where one event leads to another. 
	This chain of cause and effect can be modeled using numbers or sequences (e.g., event A happens before event B, or event A causes event B).

**Logic** follows **sequenced steps**—premises lead to conclusions, just as numbers in a sequence follow one another in a structured order. 
	The **order** of logical steps mirrors the order of numbers in a sequence. 
		This order is necessary for logic to function.

This is why they are inherent in humanity's endeavor to understand reality. 
	Because our reality, as space, is understood through its logic.

Numbers are not just abstract; they are the foundation for describing the **relational structure** of reality, both spatially (in terms of where things are) and temporally (in terms of when things happen).

In the broadest context, **numbers** represent **the structure of reality** itself because they allow us to describe:
- **Position** in space (coordinates),
- **Order** in time (sequence of events),
- **Relations** between quantities (through operations like addition, subtraction, multiplication),
- **Change** and **transformation** (through functions and mappings between sets).

They are the **symbolic language** that allows us to describe and engage with the world in a structured, logical way. 
	In the context of **space**, **order**, and **sequence**, numbers serve as the tools that encode the relationships and positions that define reality.
#### Numbers Represent Change (therefore Comparison and Relationships)
Another important aspect of numbers is their ability to describe **relationships** between quantities, particularly through **operations** like **addition** and **subtraction**. 
	These operations allow us to compare quantities and establish:
		- **Equalities**: For example, 2+3=52 + 3 = 52+3=5 describes how two quantities (2 and 3) combine to give a third quantity (5). This equality shows the **relationship** between these numbers.
		- **Inequalities**: Numbers also allow us to describe **comparisons** through inequalities, such as 4<54 < 54<5, meaning "4 is less than 5." This relational comparison is central to understanding differences in quantity, magnitude, and position.

These operations and comparisons form the **basis** of understanding **how values relate to each other** in both a mathematical and real-world sense. 
	Addition, subtraction, multiplication, and division all describe **transformations** between values, showing how one quantity can be related to another.

- - -
## Quantity in $\mathbb{R}^1$
### Understanding $\mathbb{R}^1$ as a Set of Possibilities
In $\mathbb{R}^1$, is a **one-dimensional** set of quantities. 
	This means that it has a single axis (the **x-axis**), and every possible value of $x$ exists on this line.

In **$\mathbb{R}^1$**, there is no other dimension to give any spatial orientation or "height."
	The $x$-axis is everything in this space, as there’s no $y$-axis or $z$-axis to move along.
		There's no "thickness" or "height" in a second dimension to create spatial depth or orientation.
### No True Spatial Orientation in $\mathbb{R}^1$
In $\mathbb{R}^1$, the concept of **forward** and **backward** does exist in a **conceptual sense** (you can say that $x=5$ is "after" $x=3$ in a sequence), but this is not **spatial** in the way we usually think about position or movement. 
	There's no **physical or visual** reference point to describe **bigness** or **smallness** graphically, because $\mathbb{R}^1$ represents only a **single dimension** with no orientation.
		You can still describe whether a number is **greater or smaller** than another (e.g., 5 is larger than 3), but this is just a comparison of **quantities**, not something you can **graphically visualize** with position or direction.
			There's no second dimension (like the $y$-axis in $\mathbb{R}^2$) to give you a sense of **relative spatial orientation**, such as **up** or **down**, **left** or **right**, or even a sense of **distance** between points.
#### Intuitive (Non)-Spatial Reasoning in $\mathbb{R}^1$
You can think of $\mathbb{R}^1$ as being "everything" in the sense that there’s no other dimension for orientation. 
	It’s like standing on an infinite, flat path that extends forever in both directions, but you can’t see or move up, down, left, or right.
		 You are bound to this one-dimensional path, so all solutions to equations in this space are just points **along** that path.
##### The $\mathbb{R}^1$ Axis as "Everything" or the Entire Set of Possibilities 
Since there’s no other dimension, the x-axis **is** the space, and there’s no concept of "thinness" or "thickness" because there’s no second dimension to compare it to.
	It’s everything you can see, and it contains all the possible values for the variable $x$.

In $\mathbb{R}^1$, points like $\LARGE x=5$ are represented by **quantities** (or scalars), but they are **not visible** in a **spatial sense**. 
	This is because:
		**A line**, as we usually think of it in everyday geometry, **implies the existence of a second dimension** or a plane that gives **spatial orientation** to that line.
			Without another dimension, the "line" in $\mathbb{R}^1$ doesn’t exist as a physical object but rather as a conceptual **sequence** of values.
				You’re just picking a point from the sequence, but you can’t **see** it spatially on a **line** because there’s no second axis (like a **y-axis**) to give that point any **visual or spatial context**. 
					There is no "above" or "below" in $\mathbb{R}^1$; there is only the non-physical notion of "before" and "after" within the sequence.
#### Sequence in $\mathbb{R}^1$
Sequence Exists, but It's Conceptual in $\mathbb{R}^1$.
In $\mathbb{R}^1$, you still have a **sequence** of values, and you can talk about **order** (e.g., x=1x = 1x=1 comes before x=2x = 2x=2), but this is only **conceptual**:
	You don’t get a sense of **distance** or **space** between the points.
		There’s no **visual reference** for the relationship between points.
##### No "Graphical" Representation of "Size" of a Magnitude in $\mathbb{R}^1$
In $\mathbb{R}^1$, you can say that **$5$** is larger than **$3$**, but there's no way to visualize this **graphically** as you might in a 2D plane (where you could plot points and **see** the spatial distance between $3$ and $5$).
	**Magnitude** exists, but it's purely a matter of comparison between scalar values along the number line, without any **visual or spatial** representation. 
		You understand "larger" or "smaller" based on sequence, but you can't **see** the "bigness" in terms of a point’s **position** relative to another point in a visual space.
			To describe **bigness** or **smallness** graphically, you need **multiple dimensions** to represent **spatial relations**.
### $\mathbb{R}^1$ is Not a Vector Space but a Scalar Field
##### Scalar Field
In $\mathbb{R}^1$, every point corresponds to a **single number**, which we call a **scalar**. 
	There’s no notion of **direction** in this space, only **magnitude**. 
		When you talk about points you're just referring to scalar values along the $x$-axis.
###### Vector Space
A **vector** has both **magnitude** and **direction**.
	To have direction, you need at least **two dimensions** to compare movement in one direction versus another.
		 In $\mathbb{R}^2$, a vector can point anywhere in the plane, and in $\mathbb{R}^3$, a vector can point anywhere in 3D space.

- - -
## Raising the Dimensionality: Facilitates "Spatiality"
The transition from $\mathbb{R}^1$ to $\mathbb{R}^2$ can be understood as the shift from thinking about **quantities as sequence** (in $\mathbb{R}^1$) to thinking about **quantities as positions** (in $\mathbb{R}^2$). 
### Adding a Second Axis (i.e. Set of Possible Values)
In $\mathbb{R}^2$, the introduction of a second axis (the **y-axis**) adds a new **dimension of differentiation**. 
	Now, you can place quantities not just along one axis but in relation to a second axis. 
		This new axis gives you a **reference point**, allowing for **location** and **spatial orientation**.
			The introduction of the second axis adds the necessary **spatial context** that allows points to have a **location** rather than just being values along a line.
				This transition marks the emergence of **space** and **positioning** from what was previously just a **sequence of quantities**, and it forms the foundation for how we think about coordinates, geometry, and spatial structures in mathematics.
### $\mathbb{R}^2$ as an Emergence of Spatial Structure from $\mathbb{R}^1$
The transition from $\mathbb{R}^1$ to $\mathbb{R}^2$ can be thought of as the emergence of **spatial structure** from a purely **linear sequence** of values:

In $\mathbb{R}^1$, all you have is **quantities** arranged in a **sequence**. 
	There’s no notion of **relative position** because everything exists along a single axis, and there's no spatial frame of reference.

In $\mathbb{R}^2$, you add another degree of freedom (the y-axis), and this creates a **space** where points can now be defined not just by a single quantity but by a pair of values. 
	The **introduction of a second axis** gives rise to the idea of **position** because it allows you to describe where points are located relative to both axes.

In a sense, the addition of the y-axis is like adding a **reference frame** that gives the x-axis **context**. 
	Points can now be described in terms of their **position** on this plane, and this is the essential difference between $\mathbb{R}^1$ and $\mathbb{R}^2$.
### The Intuitive Transition from $\mathbb{R}^1$ to $\mathbb{R}^2$
The transition from $\mathbb{R}^1$ to $\mathbb{R}^2$ is essentially the introduction of a second **dimension** that enables us to start thinking of points as having **location** or **position** in a **spatial sense**.

In $\mathbb{R}^1$, you have only one **degree of freedom** (the x-axis), and you can only move **along** that axis. 
	You’re in a purely **linear** world, where quantities are represented as scalars.

- - -
## Quantity in $\mathbb{R}^2$

Quantity in $\mathbb{R}^2$, is **two-dimensional** plane. 
### Understanding $\mathbb{R}^2$ as a Plane of Possibilities
### Sequence in $\mathbb{R}^2$
### $\mathbb{R}^2$ as a Vector Space

- - -
## Quantity in $\mathbb{R}^3$

Quantity in $\mathbb{R}^3$, is **three-dimensional** space. 
### Understanding $\mathbb{R}^3$ as a Space of Possibilities
### Sequence in $\mathbb{R}^3$
### $\mathbb{R}^3$ as a Vector Space


- - - 
## Dimensions and Axes as Sets of Possible Values (Domains and Codomains)
Each axis in a coordinate system (whether it's 1D, 2D, 3D, or higher-dimensional) corresponds to a **range of values** that a variable can take. 
	These sets of possible values are often described as the **codomain** or **domain** of a function.
		Where $x$ and $y$ represent individual, variable values corresponding to a $x$ or $y$ domain or codomain (i.e. axis/set of all possible values).
### Dimension/Axis
Each **axis** represents a **set of possible values**. 
	Moving along the xxx-axis is like exploring all possible values of xxx; the same is true for yyy and zzz.
###### Domain
If we think abstractly, each axis is really a **domain**, which is the set of all values that the independent variable (i.e. independent set of possible values) could map to. 
	For example, in $\LARGE y=f(x)$, the set of all possible $x$-values forms the **domain** of the function $f$.
###### Codomain
If we think abstractly, each axis is really a **codomain**, which is the set of all values that the dependent variable (i.e. dependent set of possible values) could map to. 
	For example, in $\LARGE y=f(x)$, the set of all possible $y$-values forms the **codomain** of the function $f$.
#### Variables
##### Variable as a Selector of Values
A **variable** is a **selector** that picks a specific value from the set of all possible values represented by an axis.

###### A Variable in 1D Space
there is just one axis (say, the xxx-axis), and the variable xxx selects a single point from this axis. 
	The value of xxx can vary freely, so you can think of the variable xxx as "moving" along the xxx-axis, selecting different values from its set of possibilities.
###### A Variable in 2D Space
(with xxx- and yyy-axes), the variables xxx and yyy select values from two independent sets of possible values.
	Together, these two variables select a specific point on the plane, defined by their respective values on the xxx-axis and yyy-axis.
##### Variable as a Coordinate
In the abstract sense, a variable is like a **coordinate** that marks where you are on an axis. 
	It tells you **which value** you are selecting from the set of possibilities that the axis represents.
		For instance, in 2D space, a point (x,y)(x, y)(x,y) is defined by its **coordinates** xxx and yyy. 
			These coordinates are the values chosen from the xxx-axis and yyy-axis, respectively.
				 The variable xxx selects a value from the xxx-axis, and yyy selects a value from the yyy-axis, together specifying a point in 2D space.
##### Variable as a Degree of Freedom
A variable represents a **degree of freedom** when no constraints are imposed on it. 
	Each variable corresponds to an axis along which you are free to move and select different values.
		In a system with nnn independent variables, you have nnn degrees of freedom, meaning you can move freely along each axis independently. Each variable represents one of these freedoms — an independent choice of value from a set of possibilities.

If you impose constraints (like through an equation), the variable may no longer be completely independent, and its value may become dependent on the values of other variables.

- - -
#### Dimensions in $\mathbb{R}^1$
**In one dimension**, such as a simple number line, the $x$-axis is a set of all possible values that $x$ can take.
	When you have a **single axis**, like the $x$-axis in $\mathbb{R}^1$, the numbers on the axis represent **positions** or **possible values** that a variable can take.
		 For instance, if you think of the $x$-axis as representing real numbers, each number (like $1, 2, 3$) marks a specific **point** or **position** along the axis.
#### [[Degrees of Freedom#Solution Sets of Equations in $ LARGE mathbb{R} 1$|Solutions in]] $\mathbb{R}^1$
#### Dimensions in $\mathbb{R}^2$
- Now, when you introduce a **second axis**, like the yyy-axis, you have a more complex **space of possibilities**. In R2\mathbb{R}^2R2, each point is not just a single number but a **pair of numbers** (x,y)(x, y)(x,y), where:
    
    - xxx is a value selected from the **set of possible values** on the xxx-axis,
    - yyy is a value selected from the **set of possible values** on the yyy-axis.

In a Cartesian plane, each axis (e.g., $x$-axis, $y$-axis, etc.) represents the set of all possible values that the corresponding variable can take.
	
		**In two dimensions**, the Cartesian plane has an $x$-axis and a $y$-axis. Each of these axes represents the range of values that the variables $x$ and $y$ can independently take.
			So, dimensions or axes are essentially **possibilities** — they define the **space** or **range** in which variables can exist.

- - -
## Equations Constrain the Axes (i.e. the Sets of Possible Values aka Domain and Codomain of a Space)
##### The resulting, constrained Subsets of Values (from the Parent Sets/Axes) is called the Range of Solutions (i.e. the Subset of Solutions).

##### The resulting, constrained Subsets of Values (from the Parent Sets/Axes) is called the Range of Solutions (i.e. the Subset of Solutions).
Domain and Codomain
### Solutions and Constraints in $\mathbb{R}^2$ and Beyond
In higher-dimensional spaces, such as R2\mathbb{R}^2R2 or R3\mathbb{R}^3R3, the **spatial aspect** becomes clearer:

- **R2\mathbb{R}^2R2**: Here, equations like y=mx+by = mx + by=mx+b describe **lines**, which are sets of solutions. These lines exist because there’s a second axis (the yyy-axis) that allows us to relate the values of xxx and yyy. Now, when you solve an equation, you can visualize a **line** because there’s a second dimension in which the solutions "spread out."
    
- **R3\mathbb{R}^3R3**: In 3D space, equations can describe **planes** or **curves**. For example, the equation z=2x+3yz = 2x + 3yz=2x+3y describes a plane in 3D space, where both xxx and yyy can vary independently to produce a set of solutions that form a plane.
    

In these higher-dimensional spaces, equations **constrain** the possible values by linking the variables, creating **solution sets** like lines, planes, or curves. These sets of solutions are visible because of the additional axes that give the system structure.

Since R1\mathbb{R}^1R1 only has one dimension, there’s no concept of **directionality**. You can only move forward or backward along the xxx-axis, so there’s no true "vector" with direction, just a **scalar** that represents the value at each point along the axis.
#### Degrees of Freedom as the Number of Independent Axes
The **degrees of freedom** are directly tied to the number of **independent axes** in the system.
	Each degree of freedom corresponds to an axis along which a variable can change freely and independently of other variables. In the absence of constraints.
		Thus, **degrees of freedom** represent how many axes are available for independent variation. 
			Each axis is like an open dimension that offers a full range of values, and having multiple degrees of freedom means you can explore these axes without restrictions.
###### Degrees of Freedom in a 1D system
There is **1 degree of freedom** because there is only one axis (the xxx-axis), and the system can move freely along it.
    The possible values of xxx form the **set of possible values** along the xxx-axis.
###### Degrees of Freedom in a 2D system
There are **2 degrees of freedom** because there are two independent axes (the xxx-axis and the yyy-axis). The system can move freely along both axes, meaning you can vary both xxx and yyy independently.
	The combination of xxx and yyy values forms a **plane** of possibilities, and the degrees of freedom represent the freedom to move along both axes.
###### Degrees of Freedom in a 3D system
There are **3 degrees of freedom** because the system can vary along the xxx-axis, yyy-axis, and zzz-axis. 
	You have full freedom to move in three independent directions, and each degree of freedom corresponds to a set of possible values along one of the axes.
#### Degrees of Freedom as Choices on Axes
You can also think of degrees of freedom in terms of **choices** you can make:
- If you have **one degree of freedom**, you can make a free choice about the value on one axis (say, the xxx-axis).
- With **two degrees of freedom**, you have two independent choices: one for xxx (along the xxx-axis) and one for yyy (along the yyy-axis).
- As you add more degrees of freedom, you’re adding more independent choices for values along additional axes.

So, each degree of freedom corresponds to an independent **choice** you can make about the value of a variable, and these choices are mapped onto the possible values represented by the axes.
#### Degrees of Freedom as Dimensions of Possibilities
In an abstract sense, each degree of freedom adds a new **dimension** to the set of possibilities:
- **1 degree of freedom** gives you a 1D space (a line), where your only choice is where to move along a single axis.
- **2 degrees of freedom** give you a 2D space (a plane), where you can move independently along both the xxx-axis and yyy-axis.
- **3 degrees of freedom** give you a 3D space (a volume), where you can vary independently along three axes.
#### Equations as Constraints on Those Possibilities (Codomains, i.e. Axes)
Think of each **axis** as representing the **entire range of possible values** a variable can take. 
	For example, the $x$-axis contains all the possible values that $x$ could assume. 
		Without any constraints, $x$ is free to roam anywhere on its axis, meaning you have **complete freedom** in choosing its value.
			The same goes for any other axis, like $y$, $z$, or even higher-dimensional axes.
				Now, an **equation** acts like a **rule** or a **restriction** on this freedom.
					 The equation tells you that **not all combinations** of values along these axes are valid — only the combinations that **satisfy the equation**.

Equations serve to **constrain** or **limit** the possibilities defined by the axes. 
	When you have multiple dimensions (e.g., $x$-axis and $y$-axis in a plane), the equation introduces a **relationship** between those dimensions.

When an equation or a relationship between variables is introduced, it typically **reduces the number of degrees of freedom** by constraining the possible values of one variable based on the values of others.
	Without constraints, you can move freely along all the axes, corresponding to **full degrees of freedom**.
		When a constraint (equation) is introduced, it effectively "ties" one variable to another, reducing your freedom to move independently.
			 The degrees of freedom are reduced because some variables are no longer free to vary independently — they are now dependent on other variables.

In a 2D space, you have two degrees of freedom: xxx and yyy can vary independently.
	If you impose a constraint like y=2xy = 2xy=2x, the equation restricts yyy to depend on xxx, so you lose one degree of freedom. Now, you only have **1 degree of freedom**, because once you choose a value for xxx, yyy is no longer free — it's determined by xxx.

For instance:
	In the equation of a circle $\LARGE x^2 + y^2 = r^2$, both $x$ and $y$ can take on any values from their respective axes (dimensions), but the **equation** constrains the possible pairs $(x,y)$ that satisfy this condition. 
		The equation restricts the values of $x$ and $y$ so that they must lie on the circle.

In this sense, **equations** are rules or conditions that **carve out specific subsets** of possibilities from the larger set of potential values on the axes. 
	They act like **filters** that limit what combinations of variables are allowed.
#### How Equations Reduce Degrees of Freedom
The number of **degrees of freedom** corresponds to the directions in which you can move independently. You can walk along the xxx-axis, the yyy-axis, and the zzz-axis without being forced to change direction on any other axis.

Initially, in an unconstrained system, each variable corresponds to an independent axis, and each axis represents a full **degree of freedom**. You can vary xxx, yyy, and zzz independently in 3D space. But when an **equation** is introduced, it imposes a relationship between variables, which effectively **reduces the degrees of freedom**.

- **Without the equation**, all points in the space are possible — you can move freely along all axes.
- **With the equation**, the movement is **restricted** to only those points that satisfy the equation. This filtering process reduces the dimensionality of the system, reducing the **degrees of freedom**.
- 
- **Before the equation**: Both xxx and yyy are free to vary independently, meaning you have 2 degrees of freedom. You could move anywhere along the xxx-axis and yyy-axis without restriction.
    
- **After the equation**: The equation forces xxx and yyy to satisfy the relationship x2+y2=r2x^2 + y^2 = r^2x2+y2=r2, meaning they can’t vary independently anymore. For any xxx you choose, yyy must be constrained to a specific value to satisfy the equation. Therefore, the equation reduces the system’s degrees of freedom from 2 to **1**. You are now constrained to move along a circle, not the entire xyxyxy-plane.
- In this case, you are left with **one degree of freedom** — the angle ttt that parameterizes the position on the circle (often expressed as parametric equations: x(t)=rcos⁡(t)x(t) = r\cos(t)x(t)=rcos(t) and y(t)=rsin⁡(t)y(t) = r\sin(t)y(t)=rsin(t)).
#### How Constraints Influence Parameters
A **parameter** is often introduced to describe the remaining freedom in a constrained system.
	Once an equation has reduced the degrees of freedom, the parameter provides a way to describe the **dependent relationships** between the remaining variables.
		In systems with constraints, parameters are used to capture the **remaining freedom** after equations have reduced the degrees of freedom.
			 When equations restrict movement along certain axes, parameters emerge as a way to describe **how the remaining variables move together**.

**After imposing constraints** through equations, the parameters allow you to **track the behavior** of the system as it moves within the constrained space.

In the circle example, after the equation $x^2 + y^2 = r^2$ has constrained the system, you’re left with one degree of freedom, which can be described by the parameter $t$ (the angle):
$$x(t) = r \cos(t), \quad y(t) = r \sin(t)$$
Here, $t$ acts as a **parameter** that governs the values of $x$ and $y$. 
	The equation constrains the relationship between $x$ and $y$, and the **parameter $t$** provides the **single degree of freedom** that allows you to move around the circle.
#### Parameters as Controllers of Axes
**Parameters** are values or variables that **control** the system’s behavior by influencing other variables. 
	They often act as **hidden dimensions** or **inputs** that affect the output of the system.
		**Parameters** are like hidden levers that influence how you move along these axes. 
			For example, if you are on a train moving along a track that weaves in all three directions (a parametric curve), you are following a specific path through the room, controlled by a parameter like $t$, even though the room itself has three dimensions.

Think of parameters as variables that define how the system's **axes** or **degrees of freedom** behave:
	In a parametric system, instead of having direct control over variables like $x$ and $y$, you introduce a **parameter** (say, $y$) that controls them.
		For instance, in parametric equations like: $x(t) = t, \quad y(t) = t + 5$ $t$ is the **parameter** that defines how both $x$ and $y$ change. 
			As t varies, it controls the values of xxx and yyy, giving you a way to describe their relationship through a **single degree of freedom**.
				Here, $t$ represents an **axis of control** — even though $x$ and $y$ vary, they are **dependent** on $t$, so we describe the system as having **one degree of freedom**.
#### Parameters and Degrees of Freedom
In parametric systems, a **parameter** represents the **freedom** remaining after constraints have been applied.

- For example, in a system constrained by an equation like x2+y2=r2x^2 + y^2 = r^2x2+y2=r2 (a circle), you no longer have two degrees of freedom because xxx and yyy are related by the equation.
- Instead, you introduce a **parameter** like ttt (which could represent an angle) to describe the remaining degree of freedom. The parameter ttt controls how both xxx and yyy vary together along the circle.
#### Converting Equations into Functions to Define Relationships
Once you have an equation that **constrains** the possible values of variables (i.e., the possibilities on the axes), you can often (but not always) **convert that equation into a function**. 
	When you do this, you're essentially **isolating** one variable (say, $y$) and expressing it as a function of another variable (say, $x$).

- For example, from the equation of a line $\LARGE y=2x+5$, you're expressing $y$ as a function of $x$, which establishes a direct **relationship** between the variables.

In this process, you're not just identifying a set of possibilities (as the equation does) — you're making **explicit the relationship** between those possibilities. 
	The function defines how, for any given value of $x$, there is a corresponding value of $y$, effectively defining the **mapping** between the dimensions (axes).

In parametric design, this is especially powerful because functions allow you to:
1. **Explore** the behavior of systems by varying inputs (independent variables).
2. **Understand** how changes in one variable affect others (dependent variables).
3. **Model** complex relationships in a more dynamic and manipulable way than with equations alone.
#### Equations and Functions in the Context of Axes (Possibilities/Codomains/Axes)
Equations are **static** constraints that describe a condition (like a circle, ellipse, or line) on the possible values of variables in different dimensions. 
	Functions, on the other hand, provide a **dynamic** description of how one dimension varies with another, defining the precise **relationship** between the variables.

So, to summarize the sequence you're describing:
1. **Axes** (or dimensions) are sets of possible values, defining the range of possibilities for each variable.
2. **Equations** impose **constraints** on those possibilities, limiting the combinations of values that can exist together.
3. **Functions** (derived from equations) express the **relationships** between variables, describing how one variable depends on another.







### **Domain and Codomain as All Possible Values**

In the context of functions or equations:

- The **domain** represents the set of all **possible input values** a variable can take. If you’re working with a function f(x)f(x)f(x), the domain is the set of all xxx-values that the function can accept.
- The **codomain** represents the set of all **possible output values** that the function might map to. It’s essentially the "target" space where the output could land.

Together, the domain and codomain form the **complete set of possibilities** for the function: the domain is where the inputs come from, and the codomain is where the outputs could potentially go.

However, this is still very **abstract** — it’s just the space of all possible values, and the actual relationship between inputs and outputs hasn't yet been defined.

### 2. **The Range: Differentiating Possible Values**

Once you introduce an **equation** or **function**, you **constrain** the values in the domain and codomain by establishing a relationship between them. This constraint is what **selects** the actual points that are part of the **range**.

- The **range** is the set of all **actual outputs** (or **solutions**) that come from applying the function or equation to the inputs from the domain. The range is a **subset** of the codomain — it’s the values the function actually "hits" based on the domain inputs.
    
    For example, consider the function f(x)=x2f(x) = x^2f(x)=x2 with a domain of all real numbers R\mathbb{R}R. The codomain might also be all real numbers R\mathbb{R}R, but the **range** of the function is actually the non-negative real numbers R≥0\mathbb{R}_{\geq 0}R≥0​, because x2x^2x2 can never be negative.
    

This differentiation happens because the **equation or function** imposes a rule on how the values from the domain are mapped to the codomain, and only a **subset of the codomain** will be valid outputs (the range).

### 3. **Equations as Constraints that Create Sets of Solutions**

When you introduce an **equation** or a **function**, it’s like imposing a **constraint** on the domain and codomain that **filters out** the impossible or invalid combinations, leaving only the valid combinations that satisfy the equation.

- For example, take the equation of a line in R2\mathbb{R}^2R2: y=mx+by = mx + by=mx+b. Before this equation is introduced, xxx and yyy could take any values from their domains and codomains (the entire R2\mathbb{R}^2R2 plane).
- However, once the equation y=mx+by = mx + by=mx+b is applied, the set of valid points where xxx and yyy satisfy the equation is constrained to a **line** in R2\mathbb{R}^2R2. This line represents the **set of solutions**, and the points on the line are the values that belong to the range of the function.

The equation is what **filters** the domain and codomain to create this set of solutions, often represented as a **curve** or **line** on a graph.

### 4. **Graphing Sets of Solutions in R2\mathbb{R}^2R2 and R3\mathbb{R}^3R3**

In R2\mathbb{R}^2R2, equations typically describe **curves** or **lines** because they create relationships between two variables (e.g., xxx and yyy).

- When you graph a function or equation, what you’re seeing is the **visual representation** of the set of solutions — the points that satisfy the equation. For example, in y=x2y = x^2y=x2, the set of points where yyy equals the square of xxx forms a **parabolic curve** in R2\mathbb{R}^2R2.

In R3\mathbb{R}^3R3, the solutions might form more complex structures, such as **surfaces** or **curves** in 3D space.

- For example, the equation z=x2+y2z = x^2 + y^2z=x2+y2 describes a surface (a **paraboloid**) in R3\mathbb{R}^3R3, where each pair of xxx and yyy values gives you a corresponding value of zzz.

In both cases, the **equation** or **function** imposes a constraint on the set of possible values, leaving only the valid **solution set** (whether a curve, line, or surface) that you can visualize.

### 5. **Equations Filter the Domain and Codomain to Create the Range**

The key idea is that **equations** or **functions** **filter** the domain and codomain to produce the **range**:

- Before applying the equation, the domain and codomain together represent all **possible input-output combinations**.
- Once the equation is applied, the set of valid input-output pairs is narrowed down to a specific **set of solutions**.
- This set of solutions is what you see **graphed** as a curve, line, or surface. The curve or line represents the actual **range** of the function — the subset of the codomain that is hit by the function given the inputs from the domain.

### 6. **Visualizing the Process**

Let’s break this process down with an example:

- **Step 1: Define the domain and codomain**. In a 2D graph, the xxx-axis represents the **domain** (all possible input values for xxx), and the yyy-axis represents the **codomain** (all possible output values for yyy).
    
- **Step 2: Introduce the equation**. Let’s say we introduce the equation y=x2y = x^2y=x2. This equation constrains the possible xxx and yyy values: for every value of xxx, yyy must equal x2x^2x2.
    
- **Step 3: Filter to find the range**. The equation selects a **subset** of valid points from the domain and codomain — the points that satisfy y=x2y = x^2y=x2. These points form a **parabola** in R2\mathbb{R}^2R2. The parabola is the set of **solutions** to the equation, and its points form the **range** of the function.
    
- **Step 4: Visualize the set of solutions**. The graph of the parabola is the visual representation of the **set of solutions** — the actual pairs of xxx and yyy values that satisfy the equation. The curve itself is a subset of the plane, filtered by the equation.
    

### 7. **Why R1\mathbb{R}^1R1 Can’t Form Sets of Solutions**

In our previous discussions, we explored how equations in R1\mathbb{R}^1R1 only yield individual points as solutions because there is only one axis (one degree of freedom). To form a **curve** or **line** as a set of solutions, you need at least two dimensions — you need a relationship between multiple variables.

- In R2\mathbb{R}^2R2, the introduction of a second dimension (the yyy-axis) allows for equations like y=mx+by = mx + by=mx+b, which can describe a line — a set of solutions rather than just isolated points.