# code challenges
#challenge 1
# function that reverses a string
def reverseString(s):
    return s[::-1]
reverseString(s)

# challenge 2
# given list of nums
# return unequal indices of the two numbers that add up to target.
def twoSum(nums, target):
    for i in range(len(nums)):
        difference= target - nums[i]
        if difference in nums:
            differenceIn= nums.index(difference)
            if i!=differenceIn:
                return[i, differenceIn]
twoSum(nums, target)

#challenge 3
# rotates that number's digits by one place.
# return the rotated number
def rotateNumber(x):
    startNum= removeLeftkDigits(x, sizeof(x)-1)
    restNum= getLeftkDigits(x,sizeof(x)-1)
    finalNum= restNum + (startNum*10**(sizeof(x)-1))
    return finalNum
rotateNumber(x)

