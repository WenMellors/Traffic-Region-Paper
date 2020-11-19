## Traffic State Time Series Prediction

**Traffic State**: Traffic state is the characteristic of the traffic system, such as **traffic density**, **traffic speed, traffic flow, traffic service demand**. And traffic state at time $t$ can be described as the matrix $S_t$.
$$
S_t = \{s^1_t, s^2_t,...,s^N_t \} \in R^{N \times D}\\ where\ N\ denotes\ the\ number\ of\ the\ nodes(like\ sensor\ point,\ station,\ and\ grid)\\ D\ denotes\ the\ state\ features\ dimension \\
s^k_t\ denotes\ k^{th}\ node's\ traffic\ state\ at\ time\ t 
$$
**Task Definition**:
$$
Input: S^{in} = \{S^{in}_{t-T_{in} +1}, S^{in}_{t-T_{in}+2}, ..., S^{in}_{t}\} \in R^{T_{in}\times N\times D_{in}} \\
Output: S^{out} = \{S^{out}_{t+1}, S^{out}_{t+2}, ..., S^{out}_{t+T_{out}}\} \in R^{T_{out}\times N\times D_{out}} \\
$$
where $D_{in}$ and $D_{out}$ may be the same or not. For example, in traffic flow prediction, $D_{in}$ and $D_{out}$ should all include flow-in and flow-out amount. And in some models, $D_{in}$ can also include other auxiliary features like node POI type.

In addition, the task definition is the **simplest definition**. In some cases, additional information can be included in the task input. For example, when you use road segment based dataset to predict traffic speed or flow, road adjacent matrix $A$ may be needed to provide additional road network topology information. 

## Traffic Location Prediction

**Spatiotemporal Point**: Spatiotemporal point can be denoted as a tuple of time stamp $t$ , location $l$, i.e., $q = (t, l)$.  In some cases, spatiotemporal point may include some auxiliary information like POI type.

**Trajectory**: Given a specific user $u$, the trajectory of the user $S^u$ is a spatiotemporal point sequence, i.e., $S^u = \{q_1,q_2,...,q_n\}$.

**Session/Trajectory Subsequence**: Given a time interval, the trajectory $S^u$ can be cut into a group of sessions $\{S^u_1, S^u_2, ...,S^u_t\}$.

**Task Definition**:
$$
Input: S^u_t = \{q_1,q_2,...,q_n\} \\
Output: \{q_{n+1}, q_{n+2},..., q_{n+p}\} \\
where\ S^u_t\ denotes\ the\ current\ session\ and\ the\ output\ sequence\ is\ the\ future\ step\ of\ S^u_t
$$
In some cases, the history sessions may also be needed in the task input.