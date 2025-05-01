# Ex14 Heap Tree
## DATE:
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
1.Start the program.

2.Use recursion to handle each node with tree->d (data), tree->l (left), and tree->r (right).

3.In preorder, print node data first, then traverse left and right subtrees.

4.In inorder, traverse left subtree, print node data, then traverse right subtree.

5.In postorder, traverse left and right subtrees first, then print node data.

6.End the program.

## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by: Daniel C
RegisterNumber: 212223240023
struct n {
char d;
struct n*l;
struct n*r;
};*/
void preOrder(struct n*tree)
{
if(tree)
{
printf("%c",tree->d);
preOrder(tree->l);
preOrder(tree->r);
}
}
void inOrder(struct n*tree)
{
if(tree)
{
inOrder(tree->l);
printf("%c",tree->d);
inOrder(tree->r);
}
}
void postOrder(struct n*tree)
{
if(tree)
{
postOrder(tree->l);
postOrder(tree->r);
printf("%c",tree->d);
}
}
*/
```

## Output:
![image](https://github.com/user-attachments/assets/9483d972-04cf-494f-828a-762e0ad541f6)

## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
