#include <stdio.h>
#include <stdlib.h>

typedef struct node Node;

struct node{
    Node* parent;
    Node* child1;
    Node* child2;
};

Node* scantree() {
    Node* tree = (Node*)malloc(sizeof(Node));
    (*tree).parent = NULL;
}

void stree(Node* tree){
    int a;
    scanf("%d", &a);
    if (a%2==0) (*tree).child1 = NULL;
    else {
        Node* new_tree = (Node*)malloc(sizeof(Node));
        (*tree).child1 = new_tree;
        stree(new_tree);
    }
    if (a/2==0) (*tree).child2 = NULL;
    else {
        Node* new_tree = (Node*)malloc(sizeof(Node));
        (*tree).child2 = new_tree;
        stree(new_tree);
    }
}

int main() {
    return 0;
}
