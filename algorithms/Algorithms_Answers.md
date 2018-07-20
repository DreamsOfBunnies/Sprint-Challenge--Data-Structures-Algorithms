Matthew Tomas
AIMLDS1
July 20, 2018

Add your answers to the Algorithms exercises here.

EXERCISE I. Give an analysis of the running time with respect to the input size
      n of each of the following program fragments below:
  a)  O(n)
  b)  O(log n)
  c)  O(n^3)
  d)  O(n^2)
  e)  O(n^4)
  f)  O(n)
  g)  O(n)
  
EXERCISE II.
  a)  def biggest_gap(arr):
        import math
	    min = math.inf
	    max = -1 * math.inf
	    for i in arr:
	      if arr[i] < min:
		    min = arr[i]
		  if arr[i] > max:
		    max = arr[i]
	    return max - min
  b)  Start at the middle floor (i.e. floor 8 on a 16 floor building) and drop 
      the egg. If it breaks move to the halfway point below (floor 4) and
	  repeat. If it doesn't break move to the halfway point above (floor 12)
	  and repeat. Then continue halving the distance between tested spots with
	  opposite results until you find consecutive floors with different results
	  and that bottom of those two floors will be the highest floor the egg can
	  be safely dropped from.
	  
EXERCISE III.
  a)  Starting at either end of the array is the extreme and worst case
      scenario for quicksort, and has a time complexity of O(n^2) because the
	  function needs to loop through the array n times, each time peeling off
	  only one item from the end and placing it in a bin.
  b)  Starting in the median is the ideal situation and has a time complexity
      of O(n log(n)) because each recursion halves the respective bin. The n
	  multiplier comes from the fact that each of the n items needs to undergo
	  this process.