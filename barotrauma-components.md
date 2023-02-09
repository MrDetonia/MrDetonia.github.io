---
layout: default
---

# Barotrauma Wiring Components

A brief guide to wiring components in Barotrauma, their inputs and outputs, and a few example circuits.

---

## Logic

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

### NOT

![NOT component](https://barotraumagame.com/baro-wiki/images/thumb/4/47/Not_Component.png/40px-Not_Component.png)

![NOT component IO](wiring/NOT.png)

Inverts a signal.

#### INPUTS:

| SIGNAL_IN | Input signal |

#### OUTPUTS:

| SIGNAL_OUT | Inverted SIGNAL_IN |

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
