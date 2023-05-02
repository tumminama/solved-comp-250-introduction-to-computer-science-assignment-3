Download Link: https://assignmentchef.com/product/solved-comp-250-introduction-to-computer-science-assignment-3
<br>
<strong><u>Submission Instructions:</u></strong>




<strong>Submit a single zipped file A3.zip</strong> which contains the modified <strong><em>WordTree.java</em></strong> file, to the myCourses assignment A3 folder. Include your name and student ID number in the comment at the top of the <strong><em>WordTree.java</em></strong> file.  <strong> </strong>

In this assignment, you will work on the problem of storing a set of <em>n</em> words in a tree data structure, and a method for efficiently finding all the words that have a given prefix.  You should be familiar with the latter problem through the autocomplete feature found on cell phones, web forms, Eclipse. For instance, if you type in “<em>aar</em>“, then the autocomplete feature may suggest <em>aardvark, aardvarks, aardwolf, aardwolves, aargh</em>.




By <em>word</em>, we mean a string formed from the set of ASCII characters, specifically alphanumeric characters a-zA-Z.      See <a href="http://www.asciitable.com/">http://www.asciitable.com/</a> for a list of all ASCII characters.   Note that ASCII encodes text using one byte or 8 bits per character.







<h2>WordTree Data Structure</h2>




Here we define a special kind of rooted tree that we use to efficiently index words by storing their prefixes. The main property of this tree is that <em>each edge corresponds to a character</em>.   Thus the path from the root of the tree to any node in the tree defines a string.  The string defined by each node is a prefix of all strings defined by the descendents of that node.




Below is an example tree. It contains the following words: <em>a, and, ax, dog, door, dot.</em>  You will note that the dashed nodes correspond to prefixes in the tree (<em>an, d, do, doo</em>) that are not in our list of words. The tree must also keep track of this distinction by storing for each node whether it corresponds to a word or not.




Note that if <em>C</em> is the set of all possible characters defined at the edges, then each node can have at most  <em>k = | C |</em> children,  where the | C |  notation just means the number of elements in set C.







<h2>What You Need To Do</h2>

<strong> </strong>

Read the provided code (<strong><em>WordTree.java, A3TesterPosted.java</em></strong>), including the comments which explain what the various methods do.     <em>This will take you some time, so go slow and read the code carefully. </em>   Note that the <strong><em>WordTree</em></strong> class has a private inner class <strong><em>TreeNode</em></strong>.




For the <strong><em>WordTree</em></strong> class, fill in the missing code for the following methods:




<ul>

 <li><em>createChild(), toString() </em>for the inner class<strong><em> TreeNode</em></strong>    <em> </em></li>

 <li><em>getPrefixNode(), insert(),  contains(),  getListPrefixMatches() </em></li>

</ul>




We suggest you implement them in the order listed above.    To get started, you may wish to add a main() method to the <strong><em>WordTree</em></strong> class.   Eventually you should move on to using the Tester file.   Don’t forget to delete the main method when you submit !




You may <u>only use </u>Java String methods <em>length()</em> and <em>charAt()</em>.  In particular, do <u>not </u>use String searching methods such as <em>String.startsWith(),  String.substring()</em>, etc.    The point of the assignment is for you to organize and compare strings using this tree data structure.




Only add code in the area where it says to add code.   The grader may be sensitive to any changes that you make outside that area.   Any helper methods that you wish to write should be added at the end of the <strong><em>WordTree.java</em></strong> file.




Note that all methods and also the inner class have been given the <em>public  </em>access modifier<em>.   </em>This was done to simplify grading.   As you will learn later in the course, typically one does not make all methods public.




Submit only the file <strong><em>WordTree.java</em></strong>  as a zip file.    Use the <strong><em>A3TesterPosted.java</em></strong>  file to test your code.  You do not need to submit this tester file.




Good luck and have fun!