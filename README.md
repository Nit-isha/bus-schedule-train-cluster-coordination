#Transfer optimisation of inter-city trains with bus service by schedule clustering for developing city.

## bus-schedule-train-cluster-coordination

- This project is made by taking data from city bus seva and Rail schedule of Raipur capital city of Chhattisgarh, India.
- Rail schedule is clustered in 15 clusters starting from, 4:50 AM to 11:30PM. Each cluster is of nearly 1hour. Clustering is done simply the calculations.
- 5 bus routes Nandanvan, Urla, Silyari, Chandkhuri and Kharora are considered taking origin as Raipur railway station. Bus starts from Raipur railway station and ends at the same location.
- For each route there are different number of buses and travel distance. 

---

- When bus reach railway station bus stop, average walking time of passengers from railway station bus stop to platform is considered as 15 minutes. 
Also average waiting time at railway station for train is considered as 15 minutes.
- AIM: Set departure time of buses such that they reach within the time duration of any cluster making that co-ordination success.
- Strategies applied:
    - Strategy 1: Apply equal offset in the departure time of all buses.
    - Strategy 2: If strategy1 fails, apply offset for individual bus. Time offset must be less than 50% of original headway between buses.
    - Strategy 3: There is less traffic in early morning and late night, thus increasing velocity of buses is possible and time may be shifted
    accordingly. If both strategies fails, this strategy can be applied.
