# Contact Management System

This Contact Management System is a simple application that allows users to store, view, edit, and delete contact information. The system is built with the implementation of several design patterns to ensure flexibility, efficiency, and maintainability. Key features include adding new contacts, editing existing ones, and browsing through the contact list. Additionally, changes to contacts can be tracked, and modifications can be reverted if necessary.

## Features
- **Add new contacts**: Users can create new contact records with essential details such as name, phone number, email, and address.
- **Edit contacts**: Existing contact details can be modified as needed.
- **Delete contacts**: Users can remove contacts from the system.
- **View contacts**: Users can browse through their contacts easily using an iterator for efficient navigation.
- **Undo changes**: Changes to contacts (additions, edits, deletions) can be tracked, and users can undo them using a command pattern.

## Design Patterns Used

1. **Prototype Pattern**:  
   The Prototype pattern is used to clone existing contact records efficiently. This allows for fast creation of new contacts based on existing ones, reducing the need for repeatedly filling out common information. For instance, if multiple contacts share similar details, users can create one contact and clone it to save time.

2. **Command Pattern**:  
   The Command pattern is implemented to track changes made to contacts. Every modification (add, update, or delete) is treated as a command, which can be recorded and rolled back if needed. This enables an "undo" feature, allowing users to revert any unintended modifications to their contacts.

3. **Iterator Pattern**:  
   The Iterator pattern is applied for navigating through the collection of contacts. This ensures that users can easily browse, search, and access contact records in an organized and sequential manner without directly exposing the underlying data structure.

