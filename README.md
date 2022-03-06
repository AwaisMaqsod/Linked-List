// Linked-List
//Simple creation of linked list , C++.
//creating linked list.
#include<iostream>
using namespace std;

class Node{
	public:
	//creating linked list structure.
		int value;
		Node*Next;
};
  void printlist(Node*n){
  	while(n!=NULL){
  	cout<<n->value<<endl;
  	n=n->Next;
	  }
  	 }

int main(){
	//creating 3 new nodes.
	Node*Head=new Node();
	Node*second=new Node();
	Node*third=new Node();
   //giving values to Head, second and third nodes.
   Head->value=1;
   second->value=2;
   third->value=3;
   //giving pointers to each nodes.
   Head->Next=second;
   second->Next=third;
   third->Next=NULL;
   //Printing values of each nodes of linked list.
   printlist(Head);
	return 0;
}
