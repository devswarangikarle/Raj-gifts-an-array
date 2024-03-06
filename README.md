# Raj-gifts-an-array
Raj wants to present his friend with an array a1, a2,. , an. He learned that his friend measures the attractiveness of the array by calculating the sum of the differences (ai - ai-1) for all integers i from 2 to n.  Raj needs assistance to determine the highest possible attractiveness of array a that he can achieve,

def max_beauty(n, array):
    array.sort()  
    beauty = sum(array[i] - array[i - 1] for i in range(1, n))
    return beauty


n = int(input())  
array = list(map(int, input().split()))  
result = max_beauty(n, array)
print(result)
