# Vending Machine Controller using Verilog HDL

## Project Overview

This project implements a simple Vending Machine Controller using Verilog HDL. The vending machine accepts coins, checks whether the inserted amount is sufficient, dispenses the selected product, and returns any remaining change.

The controller is designed using a Finite State Machine (FSM) and can be simulated in Xilinx Vivado.

## Features

- Finite State Machine (FSM)
- Accepts Multiple Coins
- Product Dispensing
- Change Return
- Active-High Reset
- Easy to Simulate

## Coin Values

| Coin | Value |
|------|-------|
| 00 | No Coin |
| 01 | ₹5 |
| 10 | ₹10 |
| 11 | ₹20 |

## Product Price

Product Price = ₹20

## Inputs

- clk
- reset
- coin[1:0]

## Outputs

- dispense
- change

## Working Principle

1. Machine starts with ₹0 balance.
2. User inserts coins.
3. Balance is updated.
4. If balance ≥ ₹20:
   - Product is dispensed.
   - Extra amount is returned as change.
   - Balance resets to ₹0.

## Project Files

- `vending_machine.v`
- `vending_machine_tb.v`
- `simulation.png`

## Software Used

- Xilinx Vivado 2022.2
- Verilog HDL

## Applications

- Smart Vending Machines
- Ticket Machines
- Automated Payment Systems
- Embedded Controllers