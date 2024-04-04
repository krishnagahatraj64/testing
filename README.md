import numpy as np

rng = np.random.default_rng()  # create a random number generator object
rand = rng.random  # assign its uniform distribution method to rand

def coin_flip():
    # Generate a random number between 0 and 1
    result = rand()
    
    # Map numbers less than 0.5 to "Heads" and greater than or equal to 0.5 to "Tails"
    return "Heads" if result < 0.5 else "Tails"

# Perform 10 coin flips
for _ in range(20):
    print(coin_flip())
