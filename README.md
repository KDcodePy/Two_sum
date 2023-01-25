# Two_sum
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.


class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
          # create a dictionary that will store index as key and numbers as value
          map = {}
          
          # iterate through the list and store it in the dictionary and return if target - current number = is already in the dictionary
          for k, v in enumerate(nums):
              if target-v in map:
                  return [map[target-v], k]
              #store the index as key and number as value 
              map[v] = k
              
         
