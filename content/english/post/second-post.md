---
author: "Kemtchouang Padjip"
title: "DataStructure notes"
date: 2022-03-09T18:17:08+01:00
draft: false
description: "Sample article showcasing basic Markdown syntax and formatting for HTML elements."
tags: ["school", "school-work", "notes"]
categories: [
    "school",
    "notes",
]
---

Notes on everything I learned on DS this day.
<!--more-->

So today I want to study DS. More so do my assignment due tomorrow and start to study hard.

## Assignment

- Single Link List
- Single Circular Link List
- Double Link List
- Double Circular Link List
- Write code in NetBeans with each of them to **INSERT**, **SEARCH** and **DELETE**.

## Single Link List

![Single Link List](https://i.postimg.cc/SQYkSSGz/Single-LL.png "Single List")




- *INSERT*

```java
public class SingleLL_insert {
    // reference to head / first node of the Singly Linked List
 public Node head = null;

 // class Node that hold data and a reference/link
 // to the next Node in the list
 class Node {
  private int data;
  private Node next;

  public Node(int data) {
   this.data = data;
   this.next = null;
  }
 }
  
    /*
  * Method to add a node at the beginning of the list
  */
 public void addNodeAtTheBeginning(int data) {
        System.out.println("Add a node with data " + data + " in the beginning.");
  // Create a new node
  Node newNode = new Node(data);

  // Check if the list is empty
  if (this.head == null) {
   // Make the new node as head
   this.head = newNode;
  } else {
   // Point the new node's next to head
   newNode.next = this.head;

   // Make the new node as head
   this.head = newNode;
  }
 }
  
    /*
  * Method to add a node at the end of the list
  */
 public void addNodeAtTheEnd(int data) {
        System.out.println("Add a node with data " + data + " at the end.");
  // Create a new node
  Node newNode = new Node(data);

  // Check if the list is empty
  if (this.head == null) {
   // Make the new node as head
   this.head = newNode;
  } else {
   Node cur = this.head;
   // traverse to the end of the list
   while (cur.next != null) {
    cur = cur.next;
   }
   cur.next = newNode;
  }
 }
  
  
 /*
  * Method to add a node at the specified position in the list
  */
 public void add(int position, int data) {
        System.out.println("Add a node with data " + data + " at the position " + position);
  // Create a new node
  Node newNode = new Node(data);

  // Init the cur and prev nodes to the head
  Node cur = this.head, prev = this.head;

  if (position == 1) {
   // Point the new node's next to head
   newNode.next = head;
   // Make the new node as head
   this.head = newNode;
   return;
  }

  // traverse to the end of the list and check positions moved
  while (cur.next != null && --position > 0) {
   // update the prev and cur references
   prev = cur;
   cur = cur.next;
  }

  // update prev to point to new node
  prev.next = newNode;

  // & new node to point to current node
  newNode.next = cur;
 }

   public void print() {
  if (this.head == null) {
   System.out.println("The List is empty.");
  } else {
   System.out.println("The contents of the Singly Linked List are : ");
   Node cur = this.head;
   while (cur != null) {
    System.out.print(cur.data + " -> ");
    cur = cur.next;
   }
   System.out.println("NULL\n");
  }
 }
        
        public static void main(String[] args) {
        SingleLL_insert list = new SingleLL_insert();
        System.out.println("Created a singly linked list .....");
 list.print();
 list.addNodeAtTheBeginning(100);
 list.print();
 list.addNodeAtTheBeginning(200);
 list.print();
       list.addNodeAtTheEnd(900);
 list.print();
 list.addNodeAtTheEnd(800);
 list.print();
        list.add(1,150);
        list.print();
        list.add(4,250);
        list.print();
        list.add(6,250);
        list.print();
    }
}
```

<https://octodex.github.com/images/yaktocat.png>  

## Single Circular Link List

- *DELETE*

```java
/* ure for a node */
    static class Node {
        int data;
        Node next;
    };
 
    /* Function to insert a node at the beginning of
a Circular linked list */
    static Node push(Node head_ref, int data)
    {
        // Create a new node and make head as next
        // of it.
        Node ptr1 = new Node();
        ptr1.data = data;
        ptr1.next = head_ref;
 
        /* If linked list is not null then set the
    next of last node */
        if (head_ref != null) {
            // Find the node before head and update
            // next of it.
            Node temp = head_ref;
            while (temp.next != head_ref)
                temp = temp.next;
            temp.next = ptr1;
        }
        else
            ptr1.next = ptr1; /*For the first node */
 
        head_ref = ptr1;
        return head_ref;
    }
 
    /* Function to print nodes in a given
circular linked list */
    static void printList(Node head)
    {
        Node temp = head;
        if (head != null) {
            do {
                System.out.printf("%d ", temp.data);
                temp = temp.next;
            } while (temp != head);
        }
 
        System.out.printf("\n");
    }
 
    /* Function to delete a given node from the list */
    static Node deleteNode(Node head, int key)
    {
        if (head == null)
            return null;
 
        // Find the required node
        Node curr = head, prev = new Node();
        while (curr.data != key) {
            if (curr.next == head) {
                System.out.printf("\nGiven node is not found"
                                  + " in the list!!!");
                break;
            }
 
            prev = curr;
            curr = curr.next;
        }
 
        // Check if node is only node
        if (curr == head && curr.next == head) {
            head = null;
            return head;
        }
 
        // If more than one node, check if
        // it is first node
        if (curr == head) {
            prev = head;
            while (prev.next != head)
                prev = prev.next;
            head = curr.next;
            prev.next = head;
        }
 
        // check if node is last node
        else if (curr.next == head) {
            prev.next = head;
        }
        else {
            prev.next = curr.next;
        }
        return head;
    }
 
    /* Driver code */
    public static void main(String args[])
    {
        /* Initialize lists as empty */
        Node head = null;
 
        /* Created linked list will be 2.5.7.8.10 */
        head = push(head, 2);
        head = push(head, 5);
        head = push(head, 7);
        head = push(head, 8);
        head = push(head, 10);
 
        System.out.printf("List Before Deletion: ");
        printList(head);
 
        head = deleteNode(head, 7);
 
        System.out.printf("List After Deletion: ");
        printList(head);
    }
```
