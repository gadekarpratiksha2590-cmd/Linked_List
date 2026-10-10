Design and implement a Singly Linked List in C++ to simulate a Supply Chain Journey Tracker (Mini-Blockchain). The system tracks a high-value product (such as organic medicine or luxury electronics) from its manufacturing origin to the final customer. Each state transition is recorded as a "Block" (node) in the chain containing data like location, timestamp, custodian name, and verification state.

Flowchart:
<img width="896" height="1200" alt="image" src="https://github.com/user-attachments/assets/8b4d22f9-06b2-453d-859b-14635c021817" />

Output:
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/fa4b45db-0693-40db-ab4e-d2d18ab9282a" />

Objectives:
• To implement a dynamic singly linked list using pointers.
• To practice structural node insertion at the beginning and end positions.
• To implement list traversal and linear search operations.
• To simulate real-world ledger systems using data structures.

Algorithm:
Node Structure Initialization

1. Define a structure or class Block containing data fields (location, custodian, timestamp, isVerified) and a pointer next pointing to the next block.

Insert Block (At End)

1. Create a new node and populate its data fields.
2. Set the next pointer of the new node to NULL.
3. If the list (Head) is empty, make the new node the Head.
4. Otherwise, traverse the list using a temporary pointer until the last node is reached (where temp->next == NULL).
5. Link the last node's next pointer to the new node.

Track Journey (Display List)

1. If the list (Head) is empty, display "No journey records found."
2. Otherwise, initialize a temp pointer to Head.
3. Loop through the list while temp is not NULL.
4. Print the product details at each node (Location \(\rightarrow \) Custodian \(\rightarrow \) Time \(\rightarrow \) Status).
1. Move temp to temp->next.

Verify Product (Search)

1. Initialize a temp pointer to Head.
2. Accept a search keyword (e.g., location or custodian name) from the user.
3. Traverse the list, matching the keyword with node records.
4. If a match is found, display the block details and set a flag.
5. If the end of the list is reached without a match, print "Tamper warning or invalid block!"

 Conclusion:
Using a dynamic Singly Linked List, a decentralized-style product journey tracker was successfully engineered. Dynamic node insertion handles continuous real-time ledger updates, while sequential traversal allows verification audits across any step of the supply chain network seamlessly.




