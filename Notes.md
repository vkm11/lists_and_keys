# Lists and Keys:-
## key Attribute:- 
:- common practice and also recommended to provide a key attribute with the v-for directive.

:- Key is a special attribute which is primarily used as a hint for vue's virtual DOM algorithm to identify nodes when diffing the new DOM tree with the old DOM tree.

:- The key attribute helps vue identify which items in a list have changed are added or removed and plays a crucial role in handling UI updates correctly and efficiently

:- when used with the v-for directive the key attribute should always have a unique value in each iteration.

:- Without keys, Vue uses an algorithm that minimizes element movement and tries to patch/reuse elements of the same type in-place as much as possible .

:-Not using keys is only suitable when your list remember output does not rely on tempirary DOM state or child component state.

:- Although the default behavior of patching is more efficient, it can lead to problems.

:- A typical value to provide to the key attribute is the property in an object. But any unique property will do as long as its not nom-primitive value like objects or arrays.
