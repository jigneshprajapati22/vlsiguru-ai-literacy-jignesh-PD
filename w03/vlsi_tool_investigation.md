
# Open-Source VLSI Tool Investigation: OpenROAD

## Track

**Physical Design (PD)**

**Official documentation:** https://openroad.readthedocs.io/en/latest/

## 1. What problem does the tool solve?

OpenROAD is an open-source electronic design automation (EDA) platform for digital integrated-circuit implementation. It helps automate physical-design operations that transform a synthesized circuit netlist into a physical layout.

## 2. Main inputs and outputs

| Category | Examples | Purpose |
|---|---|---|
| Design input | Synthesized Verilog netlist | Describes the logical circuit to implement |
| Technology data | LEF files and timing libraries | Describes physical cells, layers, and cell timing |
| Constraints | SDC timing constraints | Specifies clock and timing requirements |
| Configuration | Floorplan and flow settings | Controls implementation choices |
| Intermediate results | Placement and routing data | Captures stages of the implementation |
| Outputs | Layout data and reports | Supports review and downstream verification |

Exact input and output files depend on the platform and flow being used.

## 3. Basic workflow

1. **Floorplanning:** Define the chip area and organize major regions.
2. **Placement:** Choose locations for standard cells and blocks.
3. **Clock-tree synthesis:** Build a clock distribution network.
4. **Routing:** Create metal connections between components.
5. **Optimization and checks:** Evaluate timing and physical-design constraints, then repair supported violations where possible.
6. **Output generation:** Produce layout data and reports for downstream verification.

The process can be iterative; engineers may return to earlier steps when checks identify problems.

## 4. Small Verilog example

The following describes a two-input AND gate. It illustrates a simple digital design input; it is **not** evidence of a completed OpenROAD run.

```verilog
module and_gate (
    input  wire a,
    input  wire b,
    output wire y
);
    assign y = a & b;
endmodule
```

| A | B | Y |
|---:|---:|---:|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

## 5. What I learned

- OpenROAD supports important stages of digital physical design.
- A physical-design flow requires more than Verilog alone: technology data and design constraints are also important.
- Placement, clock-tree synthesis, and routing address different physical implementation problems.
- The final result must be checked against engineering constraints; a tool run is not automatically proof that a design meets every requirement.

## 6. Where AI/ML might help

| Engineering task | Potential AI/ML contribution | Caution |
|---|---|---|
| Placement exploration | Predict promising placement choices | Predictions require evaluation in the actual flow |
| Timing optimization | Rank paths or changes for investigation | Timing analysis must still verify the result |
| Congestion prediction | Flag areas likely to become congested | Predictions can be inaccurate for unfamiliar designs |
| Design-space exploration | Learn from previous run results | Training data may not represent a new design |

These are potential applications, not claims that every capability is built into OpenROAD.

## 7. Hands-on attempt log

Complete this section after trying the tool or an official tutorial.

- **Environment / operating system:**
- **Tutorial or flow used:**
- **Commands or steps performed:**
- **Inputs provided:**
- **Output produced:**
- **Error or obstacle, if any:**
- **What I learned from the result:**

If no hands-on run was possible, state that clearly rather than claiming successful execution.

## 8. Source

OpenROAD documentation: https://openroad.readthedocs.io/en/latest/
