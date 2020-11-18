#### Traffic State Time Series Prediction

**Traffic State**: Traffic state is the characteristic of the traffic system, such as **traffic density**, **traffic speed, traffic flow, traffic service demand**. And traffic state at time $t$ can be described as the matrix $S_t$.
$$
S_t = \{s^1_t, s^2_t,...,s^N_t \} \in R^{N \times D}\\ where\ N\ denotes\ the\ number\ of\ the\ nodes(like\ sensor\ point,\ station,\ and\ grid)\\ D\ denotes\ the\ state\ features\ dimension
$$
**Task definition**:
$$
Input: S^{in} = \{S^{in}_{t-T_{in} +1}, S^{in}_{t-T_{in}+2}, ..., S^{in}_{t}\} \in R^{T_{in}\times N\times D_{in}} \\
Output: S^{out} = \{S^{out}_{t+1}, S^{out}_{t+2}, ..., S^{out}_{t+T_{out}}\} \in R^{T_{out}\times N\times D_{out}} \\
$$
where $D_{in}$ and $D_{out}$ may be the same or not. For example, in traffic flow prediction, $D_{in}$ and $D_{out}$ should all include flow-in and flow-out amount. And in some models, $D_{in}$ can also include other auxiliary features like node POI type.