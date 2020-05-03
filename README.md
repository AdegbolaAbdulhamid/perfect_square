# perfect_square
This python program checks checks for the validity of a perfect square integer

def is_perfect_square(n):
	x = n // 2
	y = set([x])
	while x * x != n:
		x = (x + (n // x)) // 2
		if x in y: return False
		y.add(x)
	return True


print(is_perfect_square(8))
print(is_perfect_square(9))
print(is_perfect_square(100))
