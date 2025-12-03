# **Pseudocode**

### **Function 1 — Add Note**

`FUNCTION addNote(text)`

    `CREATE newNode`

    `newNode.text = text`

    `newNode.next = NULL`

    

    `IF head IS NULL THEN`

        `head = newNode`

    `ELSE`

        `temp = head`

        `WHILE temp.next IS NOT NULL`

            `temp = temp.next`

        `END WHILE`

        `temp.next = newNode`

    `END IF`

    

    `PRINT "Note added"`

`END FUNCTION`

### **Function 2 — Display Notes**

`FUNCTION displayNotes()`

    `temp = head`

    `IF temp IS NULL THEN`

        `PRINT "No notes found"`

        `RETURN`

    `END IF`

    `index = 1`

    `WHILE temp IS NOT NULL`

        `PRINT index, temp.text`

        `temp = temp.next`

        `index++`

    `END WHILE`

`END FUNCTION`

### **Function 3 — Undo**

`FUNCTION undo()`

    `IF undoStack IS EMPTY THEN`

        `PRINT "Nothing to undo"`

        `RETURN`

    `END IF`

    `action = undoStack.top`

    `POP undoStack`

    `PUSH action INTO redoStack`

    `PRINT "Undo:", action`

`END FUNCTION`

### **Function 4 — Redo**

`FUNCTION redo()`

    `IF redoStack IS EMPTY THEN`

        `PRINT "Nothing to redo"`

        `RETURN`

    `END IF`

    `action = redoStack.top`

    `POP redoStack`

    `PUSH action INTO undoStack`

    `PRINT "Redo:", action`

`END FUNCTION`

### **Function 5 — Search Note**

`FUNCTION searchNote(keyword)`

    `IF keyword EXISTS IN searchMap THEN`

        `PRINT "Result:", searchMap[keyword]`

    `ELSE`

        `PRINT "No result found"`

    `END IF`

`END FUNCTION`