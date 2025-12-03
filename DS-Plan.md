**Data Structure Planning Table:-**

| Operation | Data Structure Used | Reason for Choosing DS |
| :---- | :---- | :---- |
| Add a Note | **Linked List** | Easy to insert nodes at the end, dynamic size, good for sequential notes. |
| Display Notes | **Linked List Traversal** | Notes are stored sequentially, so traversal is simple. |
| Undo Action | **Stack** | Stack follows LIFO, which is perfect for undoing the last action. |
| Redo Action | **Stack** | Redo requires retrieving the last undone action, for which stack is ideal. |
| Categorize Notes | **Array** | Fixed 5 categories; an array is lightweight and fast for constant-size lists. |
| Search Notes | **HashMap (unordered\_map)** | Provides O(1) average-time search for keywords. |

