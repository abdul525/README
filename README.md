# Tree Traversal
### What is Tree Traversal?
Traversal is a process to visit all the nodes of a tree and may print their values too. Because, all nodes are connected via edges (links) we always start from the root (head) node. That is, we cannot randomly access a node in a tree. There are three ways which we use to traverse a tree.
### Types of Tree Traversal
3 types of Tree Traversal
1. Pre order Tree Traversal
2. Post order Tree Traversal
3. In order Tree Traversal

There is one Node which is root and other are child elements.

- Pre order tree traversal --------> elements-----> root,left,right
- In order tree traversal  --------> elements-----> left,root,right
- Post order tree traversal--------> elements-----> left,right,root
 
 Project file directory:
 
 - Tree Traversal\JAVA files\src\main\java\Node.java
 - Tree Traversal\JAVA files\src\main\java\TreeTraversal.java
 
 Output Screenshot directory:
 
 Tree Traversal\JAVA files\OUTPUT
 
Classes which are used in this algorithm:

1. Main class BinaryTree 
2. class Node

// Root of Binary Tree 
   - Node root; 
    
* Given a binary tree, print its nodes according to the 
      "bottom-up" postorder traversal. */
   -  void printPostorder(Node node) 
    { 
        if (node == null) 
            return;
            
  // Driver method 
    - public void main(String[] args) 
    { 
        BinaryTree tree; 
        tree = new BinaryTree();
        tree.root = new Node(1); 
        tree.root.left = new Node(2); 
        tree.root.right = new Node(3); 
        tree.root.left.left = new Node(4); 
        tree.root.left.right = new Node(5); 
  
        System.out.println("Preorder traversal of binary tree is "); 
        tree.printPreorder(); 
  
        System.out.println("\nInorder traversal of binary tree is "); 
        tree.printInorder(); 
  
        System.out.println("\nPostorder traversal of binary tree is "); 
        tree.printPostorder(); 
    }            
