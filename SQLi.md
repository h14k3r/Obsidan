# SQLi

### Risk
Not as common due to evolving blue team tools. Rare to find in the wild.

### Impact
All of the CIA 

## Types

#### inband
Attacker uses the same communication channels to launch the attack & gather the results of the attack.
If you launch an attack on the app & get the results back on the app, it is considered ( in band )

> Error-Based:
>
> Forces DB to generate an error, giving the attacker information upon which to refine their injection.

#### blind
 > no actual transfer of data ( no results are shown on the web-application. You rely on "behavior" of the application based on the kind of attack. For example: {SLEEP}
  
  - boolean
  - time    


#### out-of-band
> attacker is unable to use the same channel to launch the attack & gather the results of the attack. Relies on the ability for an application to make a network connection.
>
> Example: DNS or HTTP to deliever data to the attacker

 
