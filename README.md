Name: MD MOINUDDIN AHMED RAFAYET
ID: 1000054224
Section: 32
Assignment 02:

1)a):
class Node{
  int data;
  Node next;
  Node(int data){
    this.data=data;
    this.next=null;
  }
}
class LinkedList{
Node head;
public void addLast (int data){
    Node newNode=new Node(data);
    if (head==null){
    head= newNode;
    return;
    }
    Node current=head;
    while(current !=null){
      System.out.print(current.data+"->")
    }
    System.out.println("null");
  }
}

1)b):

public void removeFirst(){
  if(head==null){
    System.ou.print("List is empty. Nothing to remove.");
    return;
  }
  head=head.next;
}

1)c):

public void removeLast(){
  if(head == null){
    System.out.println("List is empty. Nothing to remove.");
  }
  if(head.next==null){
    head=null;
    return;
  }
  Node secondLast=head;
  Node lastNode=head.next;
}
secondLast.next=null;

1)d):
public void reverse(){
  Node prev=null;
  Node current=head;
  Node next=null;
  while(current!=null){
    next=current.next;
    current.next=prev;
    prev=current;
    current=next;
  }
  head=prev;
}

1)e):
public void removeKthElement(int k){
  if(head==null){
    System.out.println("List is empty.");
    return;
  }
  Node first;
  Node slow=head;
  for(int i=0;i<k;i++){
    if(fast==null){
      System.out.pirntln("k is greater than lenght");
      return;
    }
    fast=fast.next
  }
  if(fast==null){
    head=head.next;
    return;
  }
  while(fast.next!=null){
    fast=fast.next;
    slow=slow.next;
  }
  slow.next=slow.next.next;
}
