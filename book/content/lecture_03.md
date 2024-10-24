# Lecture 3

In the previous lecture, we broadly discussed different types of problems. In this lecture, we will delve deeper into problem classification definitions along with relevant examples from Transportation Engineering.

## Types of Problems

### Functional Classification

- **Linear Problems**: A linear optimisation problem involves a linear objective function and a set of linear constraints, i.e., the objective function and constraints are expressed as linear combinations of decision variables.

  **Example**: Consider a textile firm operating in Kochi. This company needs to ship 100 tons of textile goods from Kanchipuram and can rent two types of trucks: T1 and T2. Each truck of type T1 can carry 10 tons of goods and costs ₹5000 per trip, while each truck of type T2 can carry 20 tons and costs ₹8000 per trip. Thus, how many T1 and T2 type trucks should the company deploy so as to minimize the total costs?

- **Non-linear Problems**: A non-linear optimisation problem involves an objective function or constraints (or both) that are non-linear in nature i.e., the objective function and constraints are expressed via complex interactions of decision variables, such as exponential, polynomial, etc.

  **Example**: Consider a highway management firm that operates and maintains the expressway connecting Chennai with Bangalore. The highway management firm wants to set toll price \( p_1 \) for private vehicles and \( p_2 \) for commercial vehicles, to collect toll revenue on this highway. However, the National Highways Authority of India (NHAI) wants to facilitate sufficient flow between Chennai and Bangalore, ensuring that at least 1000 private and 1500 commercial vehicles each use the expressway during the peak hour. Note, the peak hour expressway traffic for private and commercial vehicles is subject to respective toll prices, and is given by \( Q_1(p_1) \) and \( Q_2(p_2) \), respectively. Nonetheless, the NHAI also wants to ensure sufficient tax collection, requiring toll price to at least be ₹150. Considering these regulations, what toll prices should the firm set so as to maximize the toll revenue?

### Temporal Classification

- **Static Problem**: A static optimization problem involves decisions made at a single point in time without consideration for how the situation changes over time. The constraints and objectives are based on current conditions, and the optimization does not account for future periods or changing circumstances.
  
  **Example**: Refer to the example problems above; these are static in nature.

- **Dynamic Problem**: A dynamic optimization problem involves decision variables that evolve over time, where the objective function and constraints depend on the current state of the system and past decisions.

  **Example**: Consider a public bus operator (government-owned) providing service between Chennai and Tirumala. Owing to the variation of demand through the day, the operator requires a different number of buses during different time periods of the day (see table below). Further, due to congestion, the operational costs of a bus – which include driver, fuel, and maintenance costs, also vary through the day (see table below). Note, to maintain a minimum level of service, the operator is regulated to not reduce service by more than 3 buses between any two consecutive time periods. Thus, how many buses should the operator run during different time periods so as to minimize the costs?

  | Time-period   | Number of buses required | Operational cost |
  |---------------|--------------------------|------------------|
  | 06 AM – 09 AM | 20                       | ₹1500            |
  | 09 AM – 12 PM | 15                       | ₹900             |
  | 12 PM – 03 PM | 8                        | ₹600             |
  | 03 PM – 06 PM | 10                       | ₹800             |
  | 06 PM – 09 PM | 18                       | ₹1400            |
  | 09 PM – 12 AM | 4                        | ₹1000            |

### Certainty Classification

- **Deterministic Problem**: A deterministic optimization problem is one in which all of the variables and parameters involved are known with certainty. The outcome of the objective function and constraints is entirely predictable based on the input values. There is no randomness or uncertainty in the system.

  **Example**: Refer to the example problems above; these are deterministic in nature.

- **Stochastic Problem**: A stochastic optimization problem incorporates randomness or uncertainty in either the objective function, the constraints, or both. Variables or parameters could be uncertain, and the optimization problem must consider different possible outcomes. The solutions typically aim to perform well on average or under uncertainty.

  **Example**: The Southern Railways wants to start a new daily Vande-Bharat (VB) service between Chennai and Rameshwaram. However, the daily passenger demand is stochastic (uncertain) and follows a normal distribution – with a mean of 900 and standard deviation of 100 for the economy class, and a mean of 30 and standard deviation of 10 for the executive class. Note, the standard 78-capacity economy class coach amounts to ₹50,000 in daily operational costs and generates an average revenue of ₹750 per seat. On the other hand, the standard 52-capacity executive class coach amounts to ₹55,000 in daily operational costs and generates an average revenue of ₹2000 per seat. Assuming that a minimum of 16 coaches must be deployed, how many economy and executive coaches should the Southern Railways deploy in the VB so as to maximize the profits while maintaining a 95% service level (satisfying passenger demand on 95% of the days)?
