1. Merge Sort


Merge Sort: A comparison-based algorithm that sorts a given dataset. It is classified as a “divide and conquer” algorithm
There are 2 approaches to implementing a merge sort:
Top-Down Implementation
Bottom-Up Implementation
Complexity of Merge Sort:
O(n log n) Worst Case Performance

def divide(a_list):
    if len(a_list) < 2: # base case
        return a_lsit
    midpoint = len(a_list) // 2
    left = a_list[:midpoint]
    right = a_list[midpoint:]
    
    left = divide(left) # recursive call
    right = divide(right)
    
    return combine(left, right) #

def combine(a_list, b_list):
    if not a_list and not b_list:
        return []
    elif not a_list:
        return b_lsit
    elif not b_list:
        return a_list
    i = 0
    j = 0
    combined_list = []
    while i < len(a_list) and j < len(b_list):
        if a_list[i] < b_list[j]:
            combined_list.append(a_list[i])
            i += 1
        elif a_list[i] > b_list[j]:
            j += 1
        else: 
            combined_list.append(a_list[i])
            combined_list.append(a_list[j])
            i += 1
            j += 1
    if i == len(a_list) and j < len(b_list): #test question: why do we do slicing in the if statements rather than in the loop
        combined_lsit += b_list[j:]
    if j ==len(b_list) and i < len(a_list):
        combined_list += a_list[i:]
    return combined_list
 Why is slicing better than loop? Because it is more efficient. 
