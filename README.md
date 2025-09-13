# EX14-Inheritance


AIM:
    To study and implement Inheritance

SOFTWARE USED:
    VS Code

OBJECTIVE:
    1. Code Reusability
       - Inheritance allows the functionality of existing classes 
         to be reused in new classes without rewriting the same code.

    2. Data Hiding and Access Control
       - By using private, protected, and public modes, inheritance 
         provides controlled access to members.

    3. Extensibility
       - Existing classes can be extended with new features 
         without modifying the original class.

    4. Hierarchical Classification
       - Represents real-world IS-A relationships.
         Example: Student IS-A Person, Car IS-A Vehicle.

    5. Polymorphism
       - Supports runtime polymorphism using virtual functions 
         and method overriding.

    6. Maintainability
       - Changes in base class are automatically reflected 
         in derived classes.

    7. Readability & Organization
       - Improves logical program structure by separating 
         general and specific features.

------------------------------------------------------------
THEORY:

1) DEFINITION
   - Inheritance is an OOP mechanism where a class (derived) acquires 
     properties and behaviors from another class (base). 
     It represents the “IS-A” relationship and provides reusability, 
     extensibility, and polymorphism.

2) WHY USE INHERITANCE
   - Code Reusability: reuse base class implementation.
   - Extensibility: extend features without modifying original class.
   - Logical Modelling: represents hierarchical relationships.
   - Polymorphism: enables runtime binding using virtual functions.
   - Maintainability: changes in base reflect in all derived classes.

3) MAIN TYPES
   - Single        : Derived class inherits from one base class.
   - Multiple      : Derived class inherits from multiple base classes.
   - Multilevel    : A derived class acts as a base for another derived.
   - Hierarchical  : Several derived classes inherit from one base.
   - Hybrid        : Combination of two or more inheritance types.

4) MODES OF INHERITANCE
   - Public    : public in base -> public in derived, 
                 protected in base -> protected in derived.
   - Protected : public/protected in base -> protected in derived.
   - Private   : public/protected in base -> private in derived.

5) IMPORTANT CONCEPTS
   - Constructor/Destructor Order:
     Base constructors execute first, destructors in reverse order.
   - Name Hiding:
     Derived functions can hide base functions with the same name.
   - Virtual Functions:
     Enable runtime polymorphism through overriding.
   - Abstract Classes:
     Classes with pure virtual functions; cannot be instantiated.
   - Diamond Problem:
     Occurs in multiple inheritance, solved using virtual inheritance.

6) COMMON PITFALLS
   - Unintended access-level changes.
   - Ambiguity in multiple inheritance.
   - Overuse of inheritance instead of composition (HAS-A).
   - Object slicing when assigning derived to base by value.

7) PRACTICAL GUIDELINES
   - Use public inheritance only for IS-A relationships.
   - Use composition for HAS-A relationships.
   - Keep hierarchies shallow for clarity.
   - Make destructors virtual in polymorphic base classes.

8) FLOWCHART REPRESENTATION
   - Hierarchical:
       [Base] -> [D1], [D2], [D3]

   - Multilevel:
       [A] -> [B] -> [C]

   - Multiple:
       [B]   [C]
         \   /
          [D]

9) EXAMPLES
   - GUI frameworks: Widget -> Button, TextBox, CheckBox
   - File system: File -> TextFile -> LogFile
   - Multiple inheritance: Drawable + Serializable

------------------------------------------------------------
CONCLUSION:
   - Inheritance improves code reusability, extensibility, and structure. 
   - It models real-world IS-A relationships and enables polymorphism. 
   - Misuse can cause ambiguity, deep hierarchy problems, 
     and complexity (e.g., diamond problem).
   - Best practice: use inheritance for IS-A, composition for HAS-A, 
     and apply virtual inheritance or destructors where needed.
   - With careful design, inheritance leads to flexible, maintainable, 
     and scalable programs.
------------------------------------------------------------
*/
