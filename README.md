# Sorting-Algorithms-Visualizer

in linux terminal
## Run defaults by 
>python3 ./graph_drawer.py

## Test your favorite Sorting Algorithms!
Create new python script inside `/Algorimhms` folder.  
Name your main function `sort`, the visualizer will call that and it will parse the shuffled array.
Every step of your algorithm must yield with the current state of the array to visualize it in the terminal.  

## Example
Bubble Sort
```py
def sort(arr):
    n=len(arr)
    fine = False
    while not fine:
        fine = True
        for i in range(n-1): 
            if arr[i] > arr[i+1]:
                temp = arr[i]
                arr[i] = arr[i+1]
                arr[i+1] = temp
                fine = False
        
            yield arr
```
## [optional] `--help`
`-a 1 3 4` choice what algorithms to use by its number found by `--help`  
`-t` specify frametime of Visualizer in seconds

