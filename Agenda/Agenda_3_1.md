# Agenda 1.3.2026

Wednesday 11am in the teachers' room of Anlou building

## Mario
### Funding for Access of Weather Service
#### Current situation
Currently there is no connection between our database and any weather service

#### Target State
We should have some access to weather data.
Perferrably:
- Temperature
- Air Pressure
- Rain/Sun
- Humidity
- Wind Speed

##### Solution 1: We buy it
Two Services exist:
1. https://dev.qweather.com - 50.000 Requests per month
2. https://www.apispace.com/eolink/api/456456/introduction - 0.0008 RBB/API-Call

For both Services I would require some help with the Website.

##### Solution 2: We set it up by ourselves
We could set up our own sensors on the roof of Tongji using LoRA to provide our own weather station.
Costs: I have a list of items we require but struggle with the translation of TaoBao

### Funding for a better Server

#### Current Situation
I have accessed the server in the evening of the 30.3. when nobody was doing anything. 
Despite having nothing to do the Memory was already in the upper threshold area:
```                 total        used        free      shared  buff/cache   available
Mem:           7.1Gi       5.9Gi       370Mi        17Mi       1.2Gi       1.2Gi
Swap:             0B          0B          0B
```
Nothing in the Swap is usually a good sign

For some reason while I was on the server there was no running instance of MySQL (any more).
Therefor I can't do a proper examination of the current status.

But some selected information:


##### CPU
```
Model name:             Intel(R) Xeon(R) Platinum
cpu MHz		: 2499.998
cpu MHz		: 2499.998
cpu MHz		: 2499.998
cpu MHz		: 2499.998
```
Currently there's four cores with 2,5GHz each. Which is maybe a bit weak by today's standards...

##### Hard Drive
```
/dev/vda3        99G   54G   41G  57% /
```
For now we don't need to worry about space. But 100GB is not much at all.

### Prototype
