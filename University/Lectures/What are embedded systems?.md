#embedded #pwr 

# Definition
![[embedded system]]

## Characteristics
- Performs specific task
- Performs task in specific time frame
- High efficiency
- Minimal user interface
- Less human intervention
- They do not change rapidly
- High reliability
- Can be optimised to:
  - Have low cost
  - Be simple
  - Be easy to develop
  - Have low heating

# Difference between requirements and specification
## Questions of requirements
- What we are building?
- How much will it cost?
- How fast it should work?
- How big it will be?
- How much it will weight?
- What is the energy consumption of it?

## Questions of specification
- What is frequency of receiving/sending data?
- Where data will be send?
- Will it be in parallel or in series?

Specification ask more detali question about implementation.

# State charts
They extends finite state machines by:
- hierarchy of processes
- parallelism
- complex variables
- non determinism
- information broadcasting

## Basics
Every edge have label `j/k`, you can think about it like:

```c++
if (i) {
    do(k);
    go_to_next_state();    
}
```

![[state_chart_1.png]]

They can be run in parallel.

![[state_chart_2.png]]

You can make a hirerhy to better organise things.

![[state_chart_3.png]]

Starting points are marked by black dots.

![[state_chart_4.png]]

Additionally we can have variables.

![[state_chart_5.png]]
