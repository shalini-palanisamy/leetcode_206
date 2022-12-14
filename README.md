# leetcode_206
Reverse Linked List

```ruby
/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     struct ListNode *next;
 * };
 */
struct ListNode* reverseList(struct ListNode* head){
    struct ListNode* th = head;
    struct ListNode* temp = NULL;
    head = NULL;
    while(th)
    {
      temp=th;
      th =th -> next;
      temp->next=head;
      head = temp;
    }   
    return head;
}
```
