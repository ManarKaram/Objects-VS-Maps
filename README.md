
# Objects vs Maps


## Table of content

- The concepts ( what's Map and Object? )
- Differences between Map and Object
- Usage of them

  - How to construct?
  - Accessing elements
  - Adding new elements
  - Checking if element is exist
  - Removing element
  - Checking the size
  - Iterating

- Conclusion


What's Map and Object?

Map:

- Map is a data collection type (_abstract data structure type_), in which, data is stored in a form of  **pairs** , which contains a  **unique**   **key**  and  **value mapped to that key**. And because of the uniqueness of each stored key, there is  **no duplicate**  pair stored.
- Map is mainly used for  **fast searching and looking up**  data.

Object:

- Object is object (_ **Regular** _** Object),** _type_ of data collection, which means it also  **follows key-value stored concept**  like Map. Each  **key**  in Object or we normally call it "property" which is also  **unique**  and  **associated with a single value**.
- Object in JavaScript has  **built-in prototype** and is used **to manipulate values an combine them into more complex objects**.

Differences between Map and Object

| Map | Object |
| --- | --- |
| the key-field can be of any data-type (integer, an array, even an object!) | the data-type of the key-field is restricted to integer, strings, and symbols |
| the original order of elements is preserved | the original order of elements isn't preserved |
| Map is an instance of an object | Object isn't an instance of map but is instance of classes |
| Json don't support maps | Json support objects |

Usage of them
How to construct?
**Map:**

Map is constructed and declared by using its built-in constructor and _new_ syntax.

![](RackMultipart20221031-1-i61x9w_html_cdabc9f6fc38203d.png)

**Object:**

Object has several ways to declare.

-Direct literal

![](RackMultipart20221031-1-i61x9w_html_e9335d1d360bd624.png)

-by constructor

![](RackMultipart20221031-1-i61x9w_html_d564cb73de8cd942.png)

-by using _ **Object.prototype.create** _

![](RackMultipart20221031-1-i61x9w_html_7171bb713a40c177.png)

-by using **built-in constructor**
 ![](RackMultipart20221031-1-i61x9w_html_c2b9dcf3a075e1ec.png)

Accessing elements

**Map:** Map uses its inbuilt **get() method** for accessing its elements.

![](RackMultipart20221031-1-i61x9w_html_685c423599ac5532.png)

**Object:** Objectsimply uses the _'key'_ name with a dot **(.) operator** to access its elements.
 ![](RackMultipart20221031-1-i61x9w_html_bad19fa37c3dbd9a.png)

Adding new elements

**Map:** Map uses **set() method** to add new element.

![](RackMultipart20221031-1-i61x9w_html_c8a1dd304050a16d.png)

**Object:**  it is done directly.

![](RackMultipart20221031-1-i61x9w_html_71dfc2fa95647ae1.png)

Checking if element is exist

**Map:** Map uses it's **inbuilt has() method** for this.

![](RackMultipart20221031-1-i61x9w_html_580cdada1b13d1ae.png)

**Object:**  Object uses **'===' operator** for performing the task.

![](RackMultipart20221031-1-i61x9w_html_b46344a1ad59e4c4.png)

Removing element

**Map:**

**-Delete item.**

Map uses it's **inbuilt** **delete()** that returns a Boolean value.

![](RackMultipart20221031-1-i61x9w_html_d3f9955a7b890b38.png)

**-Delete MapSet.**

Map uses it's **inbuilt** **clear()** that will remove all Map elements.

![](RackMultipart20221031-1-i61x9w_html_5c18d91f1d1bd80d.png)

**Object:**  there is no built-in method to delete a property from it. Instead, we can use the operator  **delete**.

![](RackMultipart20221031-1-i61x9w_html_aa15ceb0ac7d70d7.png)

![](RackMultipart20221031-1-i61x9w_html_618827ffad3b18a3.png)

Or we can **" undefine "** the element itself as follows:

![](RackMultipart20221031-1-i61x9w_html_24031f2c59700c47.png)

Checking the size

**Map:** Map automatically updates its size and get the easiest.

![](RackMultipart20221031-1-i61x9w_html_9919bfd08ede7efe.png)

**Object:**  it needs to be calculated manually, with the help of _**Object.keys()**_

![](RackMultipart20221031-1-i61x9w_html_7ecd7a9be078c03a.png)

Iterating

**Map:** is built-in iterable.

![](RackMultipart20221031-1-i61x9w_html_92c46c9d55c181c9.png)

**Object**** : **either we use**" **_** for… in **_**" **Or using ** Object.keys(obj)** to get all the keys and iterate

![](RackMultipart20221031-1-i61x9w_html_e169fb8dec229af3.png)

![](RackMultipart20221031-1-i61x9w_html_46477d01e5f4744.png)

Conclusion

Despite all the advantages  **Map**  can have against  **Object** , there is still cases  **Object**  will perform better. After all, Object is the most basic concept of Javascript.

- Objects are a great choice for situations where we need simple structure to store data and the type of keys needed is either an integer, strings or symbols.
- Scenarios which needs the application of separate logic to individual property element, the object is definitely the choice.
- Map is completely hash whereas Object is more than that.

Map tends to have more advantages over  **Object**  in scenarios when we just need a simple look-up structure for data storing, with all the basic operations it provided. However,  **Map**  can't never replace  **Object** , in any sense, because in Javascript,  **Object**  is — after all —  **more than just**  a normal hash table (_and therefore shouldn't be used as a normal hash table if there is alternative, it's just a waste of a great resource ;)_).

![Shape1](RackMultipart20221031-1-i61x9w_html_2a32c2bc2658c81d.gif)

C2 General
