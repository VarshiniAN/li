#!/bin/bash
# Simple Interest Calculator
echo "Enter principal amount:"
read principal
echo "Enter annual interest rate (in %):"
read rate
echo "Enter time period (in years):"
read time
interest=$(echo "scale=2; $principal * $rate * $time / 100" | bc)
echo "The simple interest is: $interest"
