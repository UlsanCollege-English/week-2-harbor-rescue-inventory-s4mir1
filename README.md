# Week 2 README Template

## Summary
This assignment implements several helper functions to manage a Harbor Rescue Inventory system. The functions perform tasks like retrieving items from a list, searching for supplies, counting occurrences, and creating modified lists. It focuses on practicing list operations such as indexing, slicing, and iteration. The goal is to understand how to manipulate and analyze data stored in lists efficiently.

## Approach
Use bullets to explain how each function works.

- `mission_snapshot`:  
  Returns the first and last items in the list using indexing. If the list is empty, it returns `(None, None)`.

- `cargo_window`:  
  Uses slicing to return a portion of the list starting from a given index and up to a given size. Returns an empty list if the start index is invalid or size is not positive.

- `first_supply_index`:  
  Iterates through the list using a loop and returns the index of the first occurrence of the target. Returns `-1` if the target is not found.

- `supply_report`:  
  Loops through the list to count how many times the target appears and tracks the first index where it occurs. Returns `(count, first_index)`.

- `priority_load` (stretch):  
  Creates a new list by adding the urgent item at the beginning and keeping the original list unchanged.

## Complexity reasoning

| Function | Time complexity | Why |
|---|---|---|
| `mission_snapshot` | O(1) | Accessing first and last elements takes constant time |
| `cargo_window` | O(k) | Slicing copies up to `k` elements (size of slice) |
| `first_supply_index` | O(n) | May need to scan the entire list to find the target |
| `supply_report` | O(n) | Iterates through the entire list to count occurrences |
| `priority_load` (stretch) | O(n) | Creates a new list by copying all elements |

## Edge-case checklist
Mark the cases you tested.

- [x] empty list  
- [x] one-item list  
- [x] target missing  
- [x] repeated values  
- [x] slice goes past end  
- [x] size is zero  
- [x] size is negative  
- [x] original list unchanged in `priority_load`  

## Assistance / Sources
List any help you used and what kind of help it gave.

- Person / tool / website: ChatGPT  
  - Help received: Explained the functions, helped implement solutions, and assisted with Git commands  

- Person / tool / website: Course materials / lecture notes  
  - Help received: Provided understanding of list operations, slicing, and time complexity concepts  