
# Distributed variable 

## what does this solve ?

query : Access a variable at a given point in time(T)
output : Gives you the latest value of the variable across all processes upto time T. (NOTE: Does not return the fresh value of that variable, meaning other process might change the variable value after time T)

## Properties

- manage time based value
- time of READ operation is important
- quick write
- slow read
- masterless

## who should use ?

- if your usecase needs - sync between multiple process on a variable which should have the lastest value till the time when you raised the request.

