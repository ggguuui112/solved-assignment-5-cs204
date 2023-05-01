Download Link: https://assignmentchef.com/product/solved-assignment-5-cs204
<br>
Creating a Tree Class, Building a Tree Converting Morse code to English characters

Samuel F. B. Morse produced the first working telegraph set in 1836. This made transmission possible over any distance. The first Morse Code message, “What hath God wrought?”, was sent from Washington to Baltimore.

Morse code was extensively used for early <a href="https://en.wikipedia.org/wiki/Radio">radio</a> communication beginning in the 1890s.

In the early part of the twentieth century, the majority of high-speed international communication

was conducted in Morse code, using telegraph lines, undersea cables, and radio circuits.

Morse code can also be transmitted using light which sometimes happens between ships at sea. It is used in emergencies to transmit distress signals when no other form of communication is available. The standard international distress signal is •••—••• (SOS).

Your assignment is to write a generic TreeNode class, a MorseCodeTree class and a MorseCodeConverter class.  There is no GUI required for this assignment.  Your classes will be tested with Junit tests.

<strong> </strong><strong>TreeNode class</strong>

This generic class is used in the MorseCodeTree classes.  The class consists of a reference to the data and a reference to the left and right child.  Follow the Javadoc that is provided.  The Javadoc only lists those public methods that are required to pass the Junit tests.  You may add any private methods you need for your design.

<strong>MorseCodeTree class</strong>

A generic linked binary tree which inherits from the LinkedConverterTreeInterface.  The class uses an external generic TreeNode class parameterized as a String: TreeNode&lt;String&gt;.  This class uses the private member of root.  Nodes are added based on their morse code value.  A ‘.’ (dot) means to traverse left and a ‘-‘ (dash) means to traverse right. The constructor will “build the tree”.  Follow the Javadoc that is provided. The Javadoc only lists those public methods that are required to pass the Junit tests.  You may add any private methods you need for your design.

<strong>Building the Data Structure (buildTree)</strong>

Your MorseCodeTree is a tree 4 levels.  Insert a mapping for every letter of the alphabet into the tree map.  The root is a TreeNode with an empty string.  The left node at level 1 stores letter ‘e’ (code ‘.’) and the right node stores letter ‘t’ (code ‘-‘).  The 4 nodes at level 2 are ‘i’, ‘a’, ‘n’, ‘m’ (code ‘..’, ‘.-‘, ‘-.’, ‘—‘).  <strong>Insert</strong> into the tree by tree level from left to right.  A ‘.’ will take the branch to the left and a ‘-‘ will take the branch to the right.  This is the structure of the tree.

<strong>Using the Data Structure</strong>

Use the MorseCodeTree to convert Morse Code to English by taking the code and finding it’s corresponding English letter by traversing the MorseCodeTree, ‘.’ branches to the left and ‘-‘ branches to the right.  The code ‘.–.’ would branch to the left, then to the right, then to the right, then to the left to <strong>Fetch</strong> the letter ‘p’.  Each letter is delimited by a space (‘ ‘).  Each word is delimited by a ‘/’.

<strong>MorseCodeConverter – Utility Class</strong>

The MorseCodeConverter contains a static MorseCodeTree object and constructs (calls the constructor for) the MorseCodeTree.

This class has two static methods <em>convertToEnglish</em> to convert from morse code to English. One method is passed a string object (“.-.. — …- . / .-.. — — -.- …”).  The other method is passed a file to be converted.  These static methods use the MorseCodeTree to convert from morse code to English characters.  Each method returns a string object of English characters.

There is also a static printTree method that is used for testing purposed – to make sure the tree for MorseCodeTree was built properly.

Use the Javadoc provided to make sure that your MorseCodeConverter class follows the method headers so that the MorseCodeConverterTest will run correctly.

<strong>The JUnit Test Class</strong>

You must add at least 1 test for MorseCodeConverter.convertToEnglish(String) and at least 1 test for MorseCodeConverter.convertToEnglish(File) to the MorseCodeConverterTest class.  Include your test file with your code files.

<strong>Test Cases:</strong>

<strong> </strong>Hello World

How do I love thee let me count the ways

Some suggestions:

<ol>

 <li>There is a morse code translator at:</li>

</ol>

<a href="http://morsecode.scphillips.com/jtranslator.html">http://morsecode.scphillips.com/jtranslator.html</a>

it will help you make test cases