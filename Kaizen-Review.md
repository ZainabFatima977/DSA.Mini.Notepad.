# Kaizen Improvement Review – Mini Notepad Project

**Project:** Mini Notepad – Data Structures Edition  
**Objective:** Identify problems in implemented features and suggest improvements to enhance functionality.

| Feature Built | Problem / Limitation | Improvement Idea | Team Member Responsible | Expected Impact |
|---------------|-------------------|-----------------|------------------------|----------------|
| Linked List – Notes Add/Delete | Deleting many notes sequentially is slow; navigation one-way only | Convert to Doubly Linked List for faster deletion and bi-directional navigation | Alizah | Faster deletion and easier navigation between notes |
| Stack – Undo Action | Only Undo supported; no Redo option | Implement Redo stack to allow full Undo/Redo | Asad | Users can undo and redo actions freely; better user experience |
| Map / HashMap – Search Notes | Search is case-sensitive; keyword mismatch fails | Implement case-insensitive search | Zainab | Users can find notes regardless of case; improves search accuracy |
| Notes Organization – Categories | All notes in one list; difficult to find notes by section | Use Node Array to organize notes into categories/sections | Anila | Notes are easier to access; system becomes organized |
| Menu / Console Interaction | Menu may be confusing; input errors possible | Provide clear numbered menu with instructions | Team | Easier navigation for users; reduces mistakes |
| Undo/Redo Tracking | Only last few actions stored | Extend stack memory to store more actions | Asad | Users can perform multiple undos/redos without limit |
| Search Efficiency | Searching large number of notes may be slow | Use HashMap / key-value indexing | Zainab | Faster search for keywords; improved performance |
| Error Handling | No warning for empty input | Add input validation & error messages | Team | Prevents invalid entries and improves user experience |
