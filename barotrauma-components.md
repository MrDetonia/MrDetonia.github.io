---
layout: default
---

# Barotrauma Wiring Components

A brief guide to wiring components in Barotrauma, their inputs and outputs, and a few example circuits.

---

## Logic

### NOT

![NOT component](https://barotraumagame.com/baro-wiki/images/thumb/4/47/Not_Component.png/40px-Not_Component.png)

![NOT component IO](wiring/NOT.png)

Inverts a signal.

#### INPUTS:

| SIGNAL_IN | Input signal |

#### OUTPUTS:

| SIGNAL_OUT | Inverted SIGNAL_IN |

---

### AND

![AND component](https://barotraumagame.com/baro-wiki/images/thumb/c/cd/And_Component.png/40px-And_Component.png)

![AND component IO](wiring/AND.png)

Performs a logical AND on both of its inputs and outputs only if both inputs are receiving a signal.

#### INPUTS:

| SIGNAL_IN_1 | Input of first signal |
| SIGNAL_IN_2 | Input of second signal |
| SET_OUTPUT | Signal to output when true |

#### OUTPUTS:

| SIGNAL_OUT | Output signal |

---

### OR

![OR component](https://barotraumagame.com/baro-wiki/images/thumb/2/29/Or_Component.png/40px-Or_Component.png)

![OR component IO](wiring/EQUALS.png)

Checks if either input is receiving signal and outputs only if true.

#### INPUTS:

| SIGNAL_IN_1 | Input of first signal |
| SIGNAL_IN_2 | Input of second signal |
| SET_OUTPUT | Signal to output when true |

#### OUTPUTS:

| SIGNAL_OUT | Output signal |

---

### XOR

![XOR component](https://barotraumagame.com/baro-wiki/images/thumb/5/54/Xor_Component.png/40px-Xor_Component.png)

![XOR component IO](wiring/EQUALS.png)

Checks if *only one* input is receiving a signal and outputs only if true.

#### INPUTS:

| SIGNAL_IN_1 | Input of first signal |
| SIGNAL_IN_2 | Input of second signal |
| SET_OUTPUT | Signal to output when true |

#### OUTPUTS:

| SIGNAL_OUT | Output signal |

---

### Equals

![Equals component](https://barotraumagame.com/baro-wiki/images/thumb/9/9e/Equals_Component.png/40px-Equals_Component.png)

![Equals component IO](wiring/EQUALS.png)

Checks if both inputs are the same and outputs only if true.

#### INPUTS:

| SIGNAL_IN_1 | Input of first signal |
| SIGNAL_IN_2 | Input of second signal |
| SET_OUTPUT | Signal to output when equal |

#### OUTPUTS:

| SIGNAL_OUT | Output signal |

---

### Greater

![Greater component](https://barotraumagame.com/baro-wiki/images/thumb/2/28/Greater_Component.png/40px-Greater_Component.png)

![Greater component IO](wiring/EQUALS.png)

Check if the first input is higher than the other and outputs only if true.

#### INPUTS:

| SIGNAL_IN_1 | Input of first signal |
| SIGNAL_IN_2 | Input of second signal |
| SET_OUTPUT | Signal to output when 1 > 2 |

#### OUTPUTS:

| SIGNAL_OUT | Output signal |

---

### RegEx Find

![RegEx Find component](https://barotraumagame.com/baro-wiki/images/thumb/b/b7/RegEx_Find_Component.png/40px-RegEx_Find_Component.png)

![RegEx Find component IO](wiring/regex-find.png)

Checks if a signal in matches a regular expression string and outputs only if true. Commonly used with a Terminal.

[Regular Expression tool](https://regexr.com/)

#### INPUTS:

| SIGNAL_IN | Input signal to test against |
| SET_OUTPUT | Signal to output when true |

#### OUTPUTS:

| SIGNAL_OUT | Output signal |

---

### Signal Check

![Signal Check component](https://barotraumagame.com/baro-wiki/images/thumb/5/5f/Signal_Check_Component.png/40px-Signal_Check_Component.png)

![Signal Check component IO](wiring/sgn.png)

Checks if a signal in matches a target signal and outputs either a true / false output signal. True output signal can be set via SET_OUTPUT. Typically used to switch between a normal and "override" state.

#### INPUTS:

| SIGNAL_IN | Input signal to test with SET_TARGETSIGNAL |
| SET_OUPUT | Signal to output when true |
| SET_TARGETSIGNAL | Target signal to test SIGNAL_IN against |

#### OUTPUTS:
| SIGNAL_OUT | False output when signals don't match. True output when signals match. |

---
