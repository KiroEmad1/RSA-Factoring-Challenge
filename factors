#!/usr/bin/env python

import sys

def factorize(num):
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            return i, num // i
    return None, None

def main():
    if len(sys.argv) != 2:
        print("Usage: factors <file>")
        return

    input_file = sys.argv[1]

    with open(input_file, 'r') as file:
        for line in file:
            num = int(line.strip())
            p, q = factorize(num)
            print(f"{num}={p}*{q}")

if __name__ == "__main__":
    main()
